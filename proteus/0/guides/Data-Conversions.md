---
title: Data Conversions
layout: guide
---

# Overview
"Automation Tasks" are tasks that can be registered with the Proteus Framework for automated execution under certain conditions.  One example is `com.i2rd.lib.automation.StaticKeyUpdateTask`, which updates database localizations for static keys defined in `.l10n.xml` files.

Another example is a "data conversion".  Sometimes we need to make changes to the database in parallel with Proteus Framework code releases.  For example, if a new Hibernate entity is introduced, we need to add a corresponding table when upgrading to a version of code that uses the entity.  when upgrading and skipping one or more versions, there may be a list of necessary database changes.  These changes are most easily managed if each one is encapsulated and registered as a data conversion task.  A data conversion could include SQL, schema changes, database functions, or indices---anything you might want to run in the databse.

Data conversions can be run using Spring Shell.  First we describe how to write a data conversion, then we cover how to run them in Spring Shell.  But note that (by default) data conversions are executed when you start your server in your dev environment, so normally you only need to use Spring Shell for debugging or testing data conversions.

Tasks implement `net.proteusframework.core.automation.Task` and are are registered for use as Spring beans.  Tasks should be annotated with `@TaskQualifier`.

# Writing Data Conversions
A data conversion is just some DDL and/or SQL that is registered with Proteus & Spring in a specific way.
The preferred way to register a data conversion is this:

1. Pick or create a Java (or Groovy) class to hold your data conversion(s).  Examples: `ProteusDataConversionsVersion0`, `UtilityFunctionsDataConversionsVersion0`, `TextFunctionsDataConversionsVersion0`; you may have an application-specific one.
2. Register the class with Spring using these class-level annotations:
    * `@Configuration`: Allows you to register methods as Spring beans using `@Bean`
    * `@Profile({"automation", "net.proteusframework.0"})`: The [@Profile] (http://docs.spring.io/spring/docs/3.1.4.RELEASE/javadoc-api/org/springframework/context/annotation/Profile.html) annotation registers the class with one or more Spring Profiles.  Always register the "automation" profile *and* 
a profile for the version of the software that the data conversions belong. This version number should only include the *major* version number of the software. (The versioned profile name should correspond to the artifact name of the project. This is what you set in the gradle.properties file for your project.) Java configurations should be placed in an "automation" package under the base package.  For example:
    * `com.example.config.automation`
    * `net.proteusframework.cms.config.automation`
    We include both a specific (`net.proteusframework.0`) and a generic (`automation`) profile so that we can easily load *either* all data conversions or just the last few versions.
3. The class should have a unique, private String `IDENTIFIER`.
4. Each data conversion is a no-argument method returning a DataConversion.  Method names should end in consecutive numbers starting from 1, with the highest-numbered method (most recent) at the top.  For example, you might have these methods:
    * `DataConversion myConversion2()`
    * `DataConversion theFirstOne1()`
    Note that the data conversion number should be used to construct the data conversion object. See the example below, where "9" is the number of the data conversion.
5.  Each method should have these annotations: 
    * `@TaskQualifier(TaskQualifier.Type.data_conversion)`: Marks the method as a data conversion
    * `@Bean`: Registers the method as returning a Spring bean
6.  Use the static methods on `SQLDataConversion` and `DatabaseObjectConversion` to help with implementation.

The following example is a Groovy data conversion that creates a database function.  Creating a function uses DDL, so we use the `withPostDDL` method.  We would use `withPreDDL` for destructive DDL (like dropping functions or tables).  See the next example for an SQL-only conversion.

```Groovy
    /**
     * Create procedure.
     * @return Bean.
     */
    @Bean
    @TaskQualifier(TaskQualifier.Type.data_conversion)
    DataConversion myFunction9()
    {
        return DatabaseObjectConversion.create(DatabaseObjectType.procedure, IDENTIFIER, 'TODO data conversion description', 9, false)
            .withPostDDL('''CREATE OR REPLACE FUNCTION myFunction(bigint) RETURNS bigint AS
$$select $1 $$ LANGUAGE SQL STABLE;''', 'Create procedure')
    }
```


# Running Data Conversions
TODO - auto run, Spring Shell


# Exercises
1. Write a data conversion that creates a table in the database and inserts some values.
