---
title: Changes
layout: default
---

# Changes in v0.4.0


* 2014-02-19  Ken Logan  <klogan@venturetech.net>

	Fix bugs from integration testing for #184. Add data conversion.

	[PF #184] Remove direct references to all admin perm
	closes #184

* 2014-02-19  Russ Tennant  <russ@venturetech.net>

	Remove unnecessary null argument from ReflectUtil.invokeMethod.

	Implement support for generating website javadoc.
	Merges pull request #312

	[PF #328] Setup JDBC Interceptor for connection pool.
	Setup interceptor to reset connection state to fix #328.
	Also set the default auto commit to true.

	Only clear volatile meta data for existing files.

	[PF #329] HTML Class updates.
	Replaced underscore separator with dash.
	Closes #329
	
	[PF #329] Change "miwt_form" HTML class to "miwt-form".
	
	For consistency always use the GroovyClassLoader for groovy.
	
	[PF #323] Rename RequestPath to PageElementPath in DAO.

	[PF #323] Fix references to renamed property.
	
	[PF #280] Remove ExpressionDAO.getInstance.

	Migrating function maintenance to data conversion. PF#88

	Improvements to the automation API for PF#88

	Update postgresql version in build.gradle.

	Add back the Log4JHandler to core and update for Log4J API differences.

	[PF #88] Update data conversion so that it doesn't leave a table around.
	Also, added an example of conversion validation.

	Added method toJavaIdentifier to StringFactory.

	Added JavaKeywords utility.

	[PF #88] Factored out schema update logic from DDLExportTask into SchemaUpdateHelper.
	Added main method to SchemaUpdateHelper to output a Spring bean for a data conversion based on the current status of the database <-> ORM.

	Update build to generate a ProjectInformation class.

	[PF #303] Javadoc for core.script classes
	closes #303

	CommandLineHelper: Add ability to specify a class to "run". Convenient if the class is a @Configurable.
	
	Update CmsFrontendDAO getSiteHostnames(CmsSite) to be getSiteHostnames(Site).

	
* 2014-02-19  Jonathan Crosmer  <jcrosmer@venturetech.net>

	Make the data conversion call CREATE EXTENSION automatically and have a better comment that the contrib package is required.  Fixes #322

	Change existing functions in '05-cms-functions.sql' and '20-text-functions.sql' to the new data conversion format. Also modified DynamicTableDAO so that it will initialize properly by disambiguating the LocaleSource.

* 2014-02-19  Justin Piper  <jpiper@i2rd.com>

	Add method to display the name and ID of all hostnames for a site
	closes #294

* 2014-02-19  Jonathan Crosmer  <jcrosmer@i2rd.com>

	[PF #297] Rename IDataProvider to remove "I"
	closes #297


