---
title: Data Conversions
layout: guide
---

# Overview
"Automation Tasks" are tasks that can be registered with the Proteus Framework for automated execution under certain conditions.  One example is `StaticKeyUpdateTask`, which updates database localizations for static keys defined in `.l10n.xml` files.

Another example is a "data conversion".  Sometimes we need to make changes to the database in parallel with Proteus Framework code releases.  For example, if a new Hibernate entity is introduced, we need to add a corresponding table when upgrading to a version of code that uses the entity.  when upgrading and skipping one or more versions, there may be a list of necessary database changes.  These changes are most easily managed if each one is encapsulated and registered as a data conversion task.  A data conversion could include SQL, schema changes, database functions, or indices---anything you might want to run in the databse.

Data conversions can be run using Spring Shell.  First we describe how to write a data conversion, then we cover how to run them in Spring Shell.  But note that (by default) data conversions are executed when you start your server in your dev environment, so normally you only need to use Spring Shell for debugging or testing data conversions.

## Automation Tasks
TODO
Tasks are registered for use as Spring beans. If a Task / DataConversion is registered via a Java config, a [@Profile] (http://docs.spring.io/spring/docs/3.1.4.RELEASE/javadoc-api/org/springframework/context/annotation/Profile.html) referencing the version number of the software should be used.

Automation tasks are routine tasks that implement the net.proteusframework.core.automation.Task interface. In order for a task to be made available for users managing automation, you will need to make it a spring bring with the appropriate net.proteusframework.core.automation.TaskQualifier. See the com.i2rd.lib.automation.StaticKeyUpdateTask for an example.

## Data Conversions
TODO


# Writing Data Conversions
TODO - process, example

DataConversions should be registered with a @Profile for the version of the software that the data conversions belong. This version number should only include the major version number of the software. Java configurations should be placed in an automation package under the base package for the API group in the case of Proteus or the Application.

Examples

* com.example.config.automation
* net.proteusframework.cms.config.automation

Example Profile Annotation

* The versioned profile name should correspond to the artifact name of the project. This is what you set in the gradle.properties file for your project.
* @Profile({“net.proteusframework.1”, “automation”})
You should always include a version specific profile and a generic profile. This way we can easily load all data conversions or just the last few versions.


# Running Data Conversions
TODO - auto run, Spring Shell
