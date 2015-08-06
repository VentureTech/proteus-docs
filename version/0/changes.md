---
title: Changes
layout: default
---

# Version 0 of the Proteus Framework

## Changes in v0.15.1

### Bug

- [PF-1153](https://agile.venturetech.net/browse/PF-1153) - @Email validation annotation doesn't work


## Changes in v0.15.0

### Summary

- Updated to Java 8.
- Updated groovy from 2.4.3 to 2.4.4.
- SeachUI API now allows search actions to be specified.
- Added doInTransaction(@FunctionalInterface) methods to HibernateSessionHelper.
- Improved CaptchaType#HARD so it is possible to solve.
- Added JDBC Interceptor to set the default trigram limit (PostgreSQL).
- Improved performance of retrieving image dimensions.
- Switched to a new set of ImageIO plugins to fix PF-1133. This provides greater support for JPEG images as well as some other less common images.
- Updated Spring configuration to delay initializing Spring Beans that require internet access until they are needed.


### Bug

- [PF-639](https://agile.venturetech.net/browse/PF-639) - JCaptcha does not work on Java 8
- [PF-1099](https://agile.venturetech.net/browse/PF-1099) - ITableScriptable.ATTRIBUTE_TABLE_SCHEMA and ATTRIBUTE_TABLE_NAME are not available
- [PF-1101](https://agile.venturetech.net/browse/PF-1101) - Fix limitedrecipientdomains regression.
- [PF-1106](https://agile.venturetech.net/browse/PF-1106) - Mail Processor "rate exceeded" error being thrown
- [PF-1110](https://agile.venturetech.net/browse/PF-1110) - Amazon Batch Scheduler / Error saying it is exceeding maximum number of entries per request
- [PF-1114](https://agile.venturetech.net/browse/PF-1114) - Email / Improve error message when sending test email
- [PF-1116](https://agile.venturetech.net/browse/PF-1116) - Amazon Verified Senders / Notification setup possible case sensitivity error
- [PF-1117](https://agile.venturetech.net/browse/PF-1117) - New page doesn't show up in page management navigation
- [PF-1124](https://agile.venturetech.net/browse/PF-1124) - AmazonServiceException in SESUtility
- [PF-1127](https://agile.venturetech.net/browse/PF-1127) - ProFTPropertyEditor does not handle property fields with multiple inputs (like a button group)
- [PF-1131](https://agile.venturetech.net/browse/PF-1131) - Issue Tracker / Updating form fields breaks the entire project
- [PF-1132](https://agile.venturetech.net/browse/PF-1132) - SES log errors non-stop when do not provide credentials
- [PF-1133](https://agile.venturetech.net/browse/PF-1133) - Error when viewing the attached JPEG image in File System
- [PF-1137](https://agile.venturetech.net/browse/PF-1137) - FileExtraValueRenderer unnecessarily copies file data into memory.

### Improvement

- [PF-1145](https://agile.venturetech.net/browse/PF-1145) - Freemarker Component / Increase height of freemarker template textarea

### Story

- [PF-964](https://agile.venturetech.net/browse/PF-964) - Port VipaSuite's backend theme to Proteus
- [PF-1111](https://agile.venturetech.net/browse/PF-1111) - Create GroovyValidator unit tests
- [PF-1112](https://agile.venturetech.net/browse/PF-1112) - Update file server to not log errors when client closes connection.
- [PF-1113](https://agile.venturetech.net/browse/PF-1113) - Make sure worker/server information is populated in spring scheduled tasks.
- [PF-1115](https://agile.venturetech.net/browse/PF-1115) - Cannot Configure User Group Visibility Condition
- [PF-1119](https://agile.venturetech.net/browse/PF-1119) - Add verbose logging option to ProFT
- [PF-1120](https://agile.venturetech.net/browse/PF-1120) - ProFTExcelReader can read "phantom" rows from an excel sheet sometimes
- [PF-1121](https://agile.venturetech.net/browse/PF-1121) - Add support for autowired ProFTBaseTest
- [PF-1123](https://agile.venturetech.net/browse/PF-1123) - Construct unit tests for ProFT
- [PF-1125](https://agile.venturetech.net/browse/PF-1125) - BaseProFTTestFace, ProFTBaseTest need to allow for custom subclassed Prefs
- [PF-1126](https://agile.venturetech.net/browse/PF-1126) - ProFTElement.setSelectOption does not work with combo boxes that have a custom renderer.
- [PF-1128](https://agile.venturetech.net/browse/PF-1128) - ProFT pre-built selector libraries need to be looked over.
- [PF-1130](https://agile.venturetech.net/browse/PF-1130) - Add database ID property
- [PF-1134](https://agile.venturetech.net/browse/PF-1134) - Update CKeditor to version 4.5 or better
- [PF-1135](https://agile.venturetech.net/browse/PF-1135) - MIWT / Create common interface for class nameable things
- [PF-1136](https://agile.venturetech.net/browse/PF-1136) - Improve email tracking search
- [PF-1138](https://agile.venturetech.net/browse/PF-1138) - Distributed Cache Invalidation Tool
- [PF-1139](https://agile.venturetech.net/browse/PF-1139) - Remove the Form Style Template Feature
- [PF-1140](https://agile.venturetech.net/browse/PF-1140) - Update CSS standard and ISearch UI with new wrapping div
- [PF-1141](https://agile.venturetech.net/browse/PF-1141) - HTML changes for the Update Login Bean
- [PF-1142](https://agile.venturetech.net/browse/PF-1142) - ServletSession - Expose CreateTime and LastAccessTime.
- [PF-1143](https://agile.venturetech.net/browse/PF-1143) - Move CleanupCruft related shell commands to Proteus if they belong there.
- [PF-1144](https://agile.venturetech.net/browse/PF-1144) - HTMLPageElementUtil.isUTF8Default is false for application/x-javascript
- [PF-1146](https://agile.venturetech.net/browse/PF-1146) - Add dc_reorderindexes to DB snapshot
- [PF-1147](https://agile.venturetech.net/browse/PF-1147) - Cleanup up corrupt EmailAddress data.


## Changes in v0.14.3


### Bug

- [PF-1105](https://agile.venturetech.net/browse/PF-1105) - Mail Processor is firing errors saying it is getting unexpected error counts
- [PF-1108](https://agile.venturetech.net/browse/PF-1108) - Form Submit Confirm Text on View Settings not actually setting confirm text
- [PF-1109](https://agile.venturetech.net/browse/PF-1109) - VerifiedSender SNS Topics can be overridden per Live/QA/Draft/etc

Other miscellaneous fixes related to tracking emails.


## Changes in v0.14.0

### Bug

- [PF-989](https://agile.venturetech.net/browse/PF-989) - Characters in HTML encoded that do not need to be
- [PF-996](https://agile.venturetech.net/browse/PF-996) - Forms / NonUniqueObjectException in FormProcessor#setChoicesAndReserveCapacity
- [PF-1033](https://agile.venturetech.net/browse/PF-1033) - Custom DB data breaks if schema name has uppercase letters in it
- [PF-1042](https://agile.venturetech.net/browse/PF-1042) - PageElementModelSupplier $Propery.join(..) causes infinite recursion
- [PF-1064](https://agile.venturetech.net/browse/PF-1064) - Exclude commons codec from birt runtime.
- [PF-1069](https://agile.venturetech.net/browse/PF-1069) - Reduce visibility of package-private members of Field
- [PF-1079](https://agile.venturetech.net/browse/PF-1079) - Forms / Can't configure Report View field
- [PF-1080](https://agile.venturetech.net/browse/PF-1080) - Make delete dialog message configurable for ActionColumn
- [PF-1082](https://agile.venturetech.net/browse/PF-1082) - ProFTExcelReader does not handle cell types that are not a string.
- [PF-1083](https://agile.venturetech.net/browse/PF-1083) - ProftExcelReader does not handle external file paths.
- [PF-1086](https://agile.venturetech.net/browse/PF-1086) - MailProcessor's email validation fails on valid case of A record with no MX
- [PF-1089](https://agile.venturetech.net/browse/PF-1089) - Email / EmailTemplateContext#withRecipientAttribute should not assume the Principal has an email address
- [PF-1097](https://agile.venturetech.net/browse/PF-1097) - Unpublished forms sending pages to 500 errors

### Improvement

- [PF-1052](https://agile.venturetech.net/browse/PF-1052) - Quiet logging in CompositeResource
- [PF-1078](https://agile.venturetech.net/browse/PF-1078) - Update Link to contain information on whether the link destination supports path info
- [PF-1092](https://agile.venturetech.net/browse/PF-1092) - Custom Content / Rich Text Configuration default type needs changed
- [PF-1094](https://agile.venturetech.net/browse/PF-1094) - Add DnD sorting to LabelCollectionEditor

### Story

- [PF-538](https://agile.venturetech.net/browse/PF-538) - Upgrade to version 5.x of CodeMirror
- [PF-895](https://agile.venturetech.net/browse/PF-895) - Quality Gate before email goes out via SES
- [PF-896](https://agile.venturetech.net/browse/PF-896) - Common API for Email Sending
- [PF-897](https://agile.venturetech.net/browse/PF-897) - Automate SES Sender Email Validation Process
- [PF-899](https://agile.venturetech.net/browse/PF-899) - Email Bounce and Complaint Tracking
- [PF-986](https://agile.venturetech.net/browse/PF-986) - Make Site available from DomainModelContext
- [PF-1043](https://agile.venturetech.net/browse/PF-1043) - PageElementModelSupplier / Add support for searching by ModelDataLabel
- [PF-1044](https://agile.venturetech.net/browse/PF-1044) - Custom Content / Import label fields doesn't work                                                                                                                                                                  
- [PF-1066](https://agile.venturetech.net/browse/PF-1066) - Objection to net.proteusframework.core.hibernate.model.AbstractEntity equals/hashCode                                                                                                                              
- [PF-1068](https://agile.venturetech.net/browse/PF-1068) - Page Registry                                                                                                                                                                                                      
- [PF-1076](https://agile.venturetech.net/browse/PF-1076) - URILink missing component id                                                                                                                                                                                       
- [PF-1085](https://agile.venturetech.net/browse/PF-1085) - Change the default validator URL                                                                                                                                                                                   
- [PF-1090](https://agile.venturetech.net/browse/PF-1090) - Create Login / Option to capture phone number                                                                                                                                                                      
- [PF-1093](https://agile.venturetech.net/browse/PF-1093) - Improve default tree display in some UIs                                                                                                                                                                           
- [PF-1098](https://agile.venturetech.net/browse/PF-1098) - Create Login / Add support for email=username 


## Changes in v0.13.2

### Bug

- [PF-1108](https://agile.venturetech.net/browse/PF-1108) - Form Submit Confirm Text on View Settings not actually setting confirm text


## Changes in v0.13.1

### Bug

- [PF-1002](https://agile.venturetech.net/browse/PF-1002) - MIWT / dnd.js / some code didn't get updated to not use prototype
- [PF-1049](https://agile.venturetech.net/browse/PF-1049) - FormRichAddAction / IllegalStateException in EventListenerList
- [PF-1051](https://agile.venturetech.net/browse/PF-1051) - ScheduledRequestImpl / BeanInfo issue
- [PF-1058](https://agile.venturetech.net/browse/PF-1058) - EmailTemplateEditor is parsing recipient, originator strings as HTML. It probably shouldn't.
- [PF-1059](https://agile.venturetech.net/browse/PF-1059) - Forms Data / enhance search model logging exception getting LocaleContext
- [PF-1060](https://agile.venturetech.net/browse/PF-1060) - Form Management / Form in use message has extra line break

### Improvement

- [PF-1054](https://agile.venturetech.net/browse/PF-1054) - Quiet MIWT DnD logging
- [PF-1056](https://agile.venturetech.net/browse/PF-1056) - DWExporter / Research if message needs logged at info level

## Story

- [PF-1006](https://agile.venturetech.net/browse/PF-1006) - Add status to PrincipalModelExtension


## Changes in v0.13.0

### Technical task

- [PF-1037](https://agile.venturetech.net/browse/PF-1037) - Configurable model field data capture UI
- [PF-1038](https://agile.venturetech.net/browse/PF-1038) - Configurable string editor
- [PF-1039](https://agile.venturetech.net/browse/PF-1039) - Configurable search constraints
- [PF-1040](https://agile.venturetech.net/browse/PF-1040) - Label field editor (Label data type, result columns, search constraints)

### Bug

- [PF-998](https://agile.venturetech.net/browse/PF-998) - Address Parts not accessible in Form Expressions
- [PF-1000](https://agile.venturetech.net/browse/PF-1000) - Update address related DomainModels to remove street name and other properties that no longer exist.
- [PF-1005](https://agile.venturetech.net/browse/PF-1005) - RecurrenceDefinitionQueryString serialization problem
- [PF-1008](https://agile.venturetech.net/browse/PF-1008) - Can't change order of name parts in a form
- [PF-1011](https://agile.venturetech.net/browse/PF-1011) - Need access to old form when copying definition
- [PF-1014](https://agile.venturetech.net/browse/PF-1014) - Closed SessionFactory being referenced by QLBuilder code
- [PF-1026](https://agile.venturetech.net/browse/PF-1026) - ImageComponent does not output HTML ID attribute
- [PF-1027](https://agile.venturetech.net/browse/PF-1027) - Invalidation of a Label without attributes is broken.
- [PF-1030](https://agile.venturetech.net/browse/PF-1030) - Freemarker Component / Model Settings / Custom DB and Custom Content supplier limit setting won't work if there is white space
- [PF-1034](https://agile.venturetech.net/browse/PF-1034) - MIWT / Label#render trims spaces
- [PF-1035](https://agile.venturetech.net/browse/PF-1035) - ListComponent loses selection when used in a TabbedContainer
- [PF-1046](https://agile.venturetech.net/browse/PF-1046) - DeploymentContext.getContext() always return unknown

### Improvement

- [PF-959](https://agile.venturetech.net/browse/PF-959) - Live Edit / Message notification in util.js needs to use the "home server" instead of hard coded

### Story

- [PF-840](https://agile.venturetech.net/browse/PF-840) - Live Edit / Render latest revision
- [PF-917](https://agile.venturetech.net/browse/PF-917) - Automated Browser Test - Component Mgt
- [PF-971](https://agile.venturetech.net/browse/PF-971) - Update CMS to generate a Request ID
- [PF-972](https://agile.venturetech.net/browse/PF-972) - Upgrade to Log4J 2.x
- [PF-973](https://agile.venturetech.net/browse/PF-973) - Update logs to include an installation name
- [PF-975](https://agile.venturetech.net/browse/PF-975) - Log statistics to logging server for trend research
- [PF-976](https://agile.venturetech.net/browse/PF-976) - Update Request Statistics to support logging to a log server
- [PF-999](https://agile.venturetech.net/browse/PF-999) - Release Version 0.13.0 Of Proteus
- [PF-1036](https://agile.venturetech.net/browse/PF-1036) - ModelField DataType / Add Label support
- [PF-1041](https://agile.venturetech.net/browse/PF-1041) - Page Permission / Apply to Folder



## Changes in v0.12.3

### Bug

- [PF-992](https://agile.venturetech.net/browse/PF-992) - Freemarker Component / Link Settings / Link's pathInfo is being cached across components
- [PF-993](https://agile.venturetech.net/browse/PF-993) - HTMLProcessingResolver / Use LinkExternalizer if Request is unavailable
- [PF-994](https://agile.venturetech.net/browse/PF-994) - FormController / Prohibit multiple calls to init
- [PF-995](https://agile.venturetech.net/browse/PF-995) - Form Visibility Condition bugs
- Some SessionFactory cleanup changes to prevent memory leaks.

## Changes in v0.12.2

### Bug

- [PF-903](https://agile.venturetech.net/browse/PF-903) - Fix database updates to NDEList on page render
- [PF-919](https://agile.venturetech.net/browse/PF-919) - VipaSolutions / HTML Component image not rendering width and height attributes
- [PF-927](https://agile.venturetech.net/browse/PF-927) - Component Management / Columns and Parameters for CC / Drop Target Problem

### Improvement

- [PF-920](https://agile.venturetech.net/browse/PF-920) - Page Management / Live Edit and Live View buttons have double "btn" class
- [PF-979](https://agile.venturetech.net/browse/PF-979) - Add CMS API to control session timeout

### Story

- [PF-921](https://agile.venturetech.net/browse/PF-921) - New Site Selector Component Updates for v2 for VIP
- [PF-982](https://agile.venturetech.net/browse/PF-982) - Capture additional text broken for Radio Button in Forms


## Changes in v0.12.1

### Bug

- [PF-911](https://agile.venturetech.net/browse/PF-911) - legacy conversion, run dynamic entity session factory rebuild, command didn't add back the FK.
- [PF-912](https://agile.venturetech.net/browse/PF-912) - legacy conversion, update statickeys gets errors
- [PF-913](https://agile.venturetech.net/browse/PF-913) - BIRT, grid contains a merged cell, engine fails to generate report document


## Changes in v0.12.0

### Bug

- [PF-691](https://agile.venturetech.net/browse/PF-691) - ZipException in XHTMLEditor.validate
- [PF-805](https://agile.venturetech.net/browse/PF-805) - Change content type .woff files are stored as
- [PF-871](https://agile.venturetech.net/browse/PF-871) - Can't Cast FileSystemEntity to FileEntity
- [PF-873](https://agile.venturetech.net/browse/PF-873) - ListSelectionModel maxSelectionIndex not equal to TableModel.getRowCount() when select all in SearchUI

- [PF-875](https://agile.venturetech.net/browse/PF-875) - Revert unintended HTML Component class name change
- [PF-877](https://agile.venturetech.net/browse/PF-877) - Unintended ID change for Tab Component
- [PF-878](https://agile.venturetech.net/browse/PF-878) - Error when trying to check if the request path is a wildcard path
- [PF-880](https://agile.venturetech.net/browse/PF-880) - PopUp windows missing interior content div
- [PF-888](https://agile.venturetech.net/browse/PF-888) - Guarded Action Permission Checks Throw Error
- [PF-890](https://agile.venturetech.net/browse/PF-890) - Ajax updates fail for Double Entry Field
- [PF-901](https://agile.venturetech.net/browse/PF-901) - BIRT Report can't be scheduled.

### Improvement

- [PF-874](https://agile.venturetech.net/browse/PF-874) - FileSystemMetadata / Update Principal properties to SET_NULL onDelete.

### Story

- [PF-89](https://agile.venturetech.net/browse/PF-89) - EHCache / Caching - Support multiple VMs
- [PF-842](https://agile.venturetech.net/browse/PF-842) - Component Management / Configurability
- [PF-843](https://agile.venturetech.net/browse/PF-843) - Component Management / Bulk Delete
- [PF-844](https://agile.venturetech.net/browse/PF-844) - Component Management / Columns and Parameters for Custom Content
- [PF-876](https://agile.venturetech.net/browse/PF-876) - Restore reset.css
- [PF-900](https://agile.venturetech.net/browse/PF-900) - ProteusShell / Change how the dynamic entity rebuild is triggered

## Changes in v0.11.0

### Bug

- [PF-808](https://agile.venturetech.net/browse/PF-808) - NPE in updating subtree state when a component has a visibility condition that isn't satisfied.
- [PF-860](https://agile.venturetech.net/browse/PF-860) - We wanted hash, but got string (Freemarker template error)
- [PF-864](https://agile.venturetech.net/browse/PF-864) - Parameter created by ParameterUtil#checkbox is not persisted or restored correctly

### Improvement

- [PF-866](https://agile.venturetech.net/browse/PF-866) - Update LocalizedNamedObject to extend NamedObject.
- [PF-867](https://agile.venturetech.net/browse/PF-867) - Create new LinkSelector UIs that implement ValueChooserEditor and ValueChooser
- [PF-868](https://agile.venturetech.net/browse/PF-868) - Create ConverterService
- [PF-869](https://agile.venturetech.net/browse/PF-869) - UI Component / Add setClassName method.
- [PF-870](https://agile.venturetech.net/browse/PF-870) - UI PropertyEditor / Create reusable PropertyEditor component that wraps a ValueEditor

### Story

- [PF-774](https://agile.venturetech.net/browse/PF-774) - Add com.i2rd.message API to proteus
- [PF-791](https://agile.venturetech.net/browse/PF-791) - Port Site Messaging Code to com.i2rd
- [PF-828](https://agile.venturetech.net/browse/PF-828) - Add support for ResourceServlet alias (additional mapping)
- [PF-833](https://agile.venturetech.net/browse/PF-833) - Support legacy URL file format based on path
- [PF-836](https://agile.venturetech.net/browse/PF-836) - WebDav support for tools that delete and add files by name
- [PF-841](https://agile.venturetech.net/browse/PF-841) - Component Mgt / Single Component Mode
- [PF-856](https://agile.venturetech.net/browse/PF-856) - Script Parameter / Add explicit collection support.
- [PF-861](https://agile.venturetech.net/browse/PF-861) - Create Rich Data Type (ModelField Data Type) API
- [PF-862](https://agile.venturetech.net/browse/PF-862) - Create default CmsModelDataSet data capture implementation
- [PF-863](https://agile.venturetech.net/browse/PF-863) - Create CmsModelDataSet Data Capture API
- [PF-865](https://agile.venturetech.net/browse/PF-865) - LocaleContext / Support comparison of NULL TextSources


## Changes in v0.10.2

### Bug

- [PF-808](https://agile.venturetech.net/browse/PF-808) - NPE in updating subtree state when a component has a visibility condition that isn't satisfied.

## Changes in v0.10.1

### Bug

- [PF-775](https://agile.venturetech.net/browse/PF-775) - Logic error in MIWTSessionLocatorImpl prevents LocaleContext from being set.

## Changes in v0.10.0

### Bug

- [PF-652](https://agile.venturetech.net/browse/PF-652) - Text link should be disabled if behind dialog
- [PF-734](https://agile.venturetech.net/browse/PF-734) - Custom DB Data / Importing a CSV does not assign a create or modify user to the records
- [PF-747](https://agile.venturetech.net/browse/PF-747) - Custom DB Data / Row expressions aren't rendering in related rows
- [PF-752](https://agile.venturetech.net/browse/PF-752) - Custom DB column plugins don't seem to be using the stored configurations
- [PF-764](https://agile.venturetech.net/browse/PF-764) - communicationContentElement.hbm.xml file not being picked up in scan

### Improvement

- [PF-748](https://agile.venturetech.net/browse/PF-748) - Custom DB / Column plugin needs ability to choose label domain from dropdown
- [PF-749](https://agile.venturetech.net/browse/PF-749) - Add static-* hostnames for Proteus QA site (Make configuration part of deployment)
- [PF-776](https://agile.venturetech.net/browse/PF-776) - Update MIWT popups to handle sizing when they contain rich text editors

### Story

- [PF-777](https://agile.venturetech.net/browse/PF-777) - Update RebuildableSessionFactoryBean so sessionFactoryBuilder is not hardcoded.


## Changes in v0.9.5

### Bug

- [PF-775](https://agile.venturetech.net/browse/PF-775) - Logic error in MIWTSessionLocatorImpl prevents LocaleContext from being set.


## Changes in v0.9.4

### Technical task

- [PF-757](https://agile.venturetech.net/browse/PF-757) - Convert CmsIconLibrary to spring configuration

### Bug

- [PF-764](https://agile.venturetech.net/browse/PF-764) - communicationContentElement.hbm.xml file not being picked up in scan

### Story

- [PF-767](https://agile.venturetech.net/browse/PF-767) - Need data conversion to rename custom database join tables


## Changes in v0.9.3

### Improvement

- Merge addition of default property to StringExtra and BooleanExtra from Vipa Suite.

## Changes in v0.9.2

### Bug

- [PF-735](https://agile.venturetech.net/browse/PF-735) - Error thrown for Data Provider extension selection popup when I have a DomainModel Extension library
- [PF-736](https://agile.venturetech.net/browse/PF-736) - Error thrown when trying to submit form via Form Data management
- [PF-742](https://agile.venturetech.net/browse/PF-742) - Custom DB Management / Error thrown when trying to edit a database
- [PF-743](https://agile.venturetech.net/browse/PF-743) - Custom DB Mgmt / Column plugin configuration data not saving
- [PF-744](https://agile.venturetech.net/browse/PF-744) - Form Package Reorg caused Discriminators in ContentElement Table to be wrong
- [PF-745](https://agile.venturetech.net/browse/PF-745) - Freemarker Custom DB extension search_count triggers error
- [PF-751](https://agile.venturetech.net/browse/PF-751) - Component identifiers are too long to be used as preference keys

### Improvement

- [PF-737](https://agile.venturetech.net/browse/PF-737) - Add new option to ParameterUtil.fieldConfigurationBuilder

### Story

- [PF-104](https://agile.venturetech.net/browse/PF-104) - MIWT-CMS integration improvement for creating MIWTApplications
- [PF-611](https://agile.venturetech.net/browse/PF-611) - Easier way to Integrate MIWT Components into CMS


## Changes in v0.9.1

### Bug

- [PF-721](https://agile.venturetech.net/browse/PF-721) - ProteusDataConfig.dataSource using wrong property for DB password

### Improvement

- [PF-713](https://agile.venturetech.net/browse/PF-713) - Update SummaryProvider.getSummary() method to return TextSource. This 
is an API breaking change.

### Story

- [PF-714](https://agile.venturetech.net/browse/PF-714) - Facebook Login Component doesn't support closed-site use case well

### Misc

- TruncatedTextSource and TextSources.createTruncated were added.
- Created a PropertyEditor for TextSource. This can be used to define TextSource property values as non-localized text or a 
LocalizedObjectKey symbol in a spring bean definition.
- ComboBox was updated to use the cell renderer when disabled.
- FormElementRegistrations can now make use of @FormElementRegistrationConfig (a spring Qualifier) for auto-wiring.

## Changes in v0.9.0

### Bug

- [PF-597](https://agile.venturetech.net/browse/PF-597) - LocalizedObjectKeyFieldComponent / rich editor HTML
- [PF-634](https://agile.venturetech.net/browse/PF-634) - Form Editor / Click To Edit UI not working in View Settings
- [PF-636](https://agile.venturetech.net/browse/PF-636) - Login component won't let you set new password for expired credentials
- [PF-647](https://agile.venturetech.net/browse/PF-647) - CmsURLModelExtension cannot locate URL to resolve values
- [PF-649](https://agile.venturetech.net/browse/PF-649) - Custom DB / NPE when searchable date field has no display name set
- [PF-651](https://agile.venturetech.net/browse/PF-651) - Reset password due to credentials expiration causes 3 failed login attempts
- [PF-657](https://agile.venturetech.net/browse/PF-657) - Condition entity uses Action's ID sequence
- [PF-678](https://agile.venturetech.net/browse/PF-678) - Forms / No feedback for errors in expressions
- [PF-689](https://agile.venturetech.net/browse/PF-689) - miwt-lib.js / IE7 querySelectorAll is being used for all IEs

### Improvement


- [PF-576](https://agile.venturetech.net/browse/PF-576) - Delete CurrentUserModelSupplier
- [PF-583](https://agile.venturetech.net/browse/PF-583) - EmailTemplateSelector / Poor usability
- [PF-596](https://agile.venturetech.net/browse/PF-596) - Rename CmsRequest.getBeanData
- [PF-616](https://agile.venturetech.net/browse/PF-616) - Make CMS components assigned by default

### Story

- [PF-141](https://agile.venturetech.net/browse/PF-141) - Move the proteus themes into a separate repo (CSS/JS/Images)
- [PF-198](https://agile.venturetech.net/browse/PF-198) - Add a current working directory label to file upload UIs
- [PF-241](https://agile.venturetech.net/browse/PF-241) - Update PageElementModelSupplier for Hibernate update
- [PF-302](https://agile.venturetech.net/browse/PF-302) - Firefox Support for LiveEdit / Test and Fix Chrome Support
- [PF-370](https://agile.venturetech.net/browse/PF-370) - Automation / Data Conversion For Theme Updates
- [PF-397](https://agile.venturetech.net/browse/PF-397) - MIWT needs a way to make action links that do not have the "btn" class
- [PF-424](https://agile.venturetech.net/browse/PF-424) - Sending emails when form submitted
- [PF-432](https://agile.venturetech.net/browse/PF-432) - Change Order of generator calls
- [PF-567](https://agile.venturetech.net/browse/PF-567) - Article container component goes into "failsafe" when switching container style
- [PF-600](https://agile.venturetech.net/browse/PF-600) - Improve MTable API naming
- [PF-622](https://agile.venturetech.net/browse/PF-622) - SearchConstraints / API to provide constraint specific class names
- [PF-628](https://agile.venturetech.net/browse/PF-628) - Update MIWT error display for uncaught exception
- [PF-637](https://agile.venturetech.net/browse/PF-637) - Remove clearing div elements from output
- [PF-638](https://agile.venturetech.net/browse/PF-638) - Create MIWT Component that integrates XMLRenderer
- [PF-640](https://agile.venturetech.net/browse/PF-640) - Article Container Component Editor adds components directly to a HistoryContainer
- [PF-658](https://agile.venturetech.net/browse/PF-658) - IE Support for LiveEdit
- [PF-659](https://agile.venturetech.net/browse/PF-659) - Form visibility condition
- [PF-671](https://agile.venturetech.net/browse/PF-671) - Finish work for "Sending emails when form submitted"
- [PF-698](https://agile.venturetech.net/browse/PF-698) - Forms / Cannot use Template feature

## Changes in v0.8.7

### Bug

- [PF-721](https://agile.venturetech.net/browse/PF-721) - ProteusDataConfig.dataSource using wrong property for DB password

### Story

- [PF-714](https://agile.venturetech.net/browse/PF-714) - Facebook Login Component doesn't support closed-site use case well

### Misc

- Fixed issue that prevented data templates from showing up in the form editor.

## Changes in v0.8.6

### Story

- [PF-698](https://agile.venturetech.net/browse/PF-698) - Forms / Cannot use Template feature

## Changes in v0.8.5

### Bug

- [PF-689](https://agile.venturetech.net/browse/PF-689) - Fix IE7 specific polyfill to be IE7 specific.

## Changes in v0.8.4

### Bug

- Fixed a possible NPE in the FormConditionEditor.

## Changes in v0.8.3

### Bug

- [PF-645](https://agile.venturetech.net/browse/PF-645) - Fixed an issue with conditions not working in Forms.

## Changes in v0.8.2

### Bug

- Fixed an issue with duplicate port numbers being output on URLs.

## Changes in v0.8.1

### Bug

- [PF-647](https://agile.venturetech.net/browse/PF-647) - CmsURLModelExtension cannot locate URL to resolve values

## Changes in v0.8.0

### Bug

- [PF-614](https://agile.venturetech.net/browse/PF-614) - Port Vs to Proteus - Menu Component / Forward slash being double encoded in query parameters
- [PF-620](https://agile.venturetech.net/browse/PF-620) - Form submitted with invalid email cannot be resubmitted
- [PF-630](https://agile.venturetech.net/browse/PF-630) - File Permissions are not working

### Improvement

- [PF-598](https://agile.venturetech.net/browse/PF-598) - File Server Component - Add support for HEAD requests

### Story

- [PF-90](https://agile.venturetech.net/browse/PF-90) - Support new BIRT emitters
- [PF-91](https://agile.venturetech.net/browse/PF-91) - Google Analytics - Support Universal Analytics
- [PF-321](https://agile.venturetech.net/browse/PF-321) - Consider renaming com.i2rd.configuration.annotation.Configurable
- [PF-573](https://agile.venturetech.net/browse/PF-573) - Change default for update statickeys command
- [PF-591](https://agile.venturetech.net/browse/PF-591) - Replace MessageUtil with IntegrationHelper
- [PF-606](https://agile.venturetech.net/browse/PF-606) - Image Cropping JS Library
- [PF-608](https://agile.venturetech.net/browse/PF-608) - Image Resource Paths / Handle protected image resources in developer image completion helper
- [PF-617](https://agile.venturetech.net/browse/PF-617) - Port VS to Proteus - File System / Indicate if a file or a folder is secured
- [PF-621](https://agile.venturetech.net/browse/PF-621) - Update Search API to use TextSource


## Changes in v0.7.1

### Bug

- [PF-599](https://agile.venturetech.net/browse/PF-599) - Cannot open email template to edit it

## Changes in v0.7.0

### Bug

- [PF-361](https://agile.venturetech.net/browse/PF-361) - EmailTemplateSelector - returns modification state of UNCHANGED when expecting CHANGED
- [PF-430](https://agile.venturetech.net/browse/PF-430) - OnDelete Annotation causing Foreign Key problems with AbstractEmailConfiguration
- [PF-450](https://agile.venturetech.net/browse/PF-450) - Bad Generator Expression Crashes Form Data Submission
- [PF-451](https://agile.venturetech.net/browse/PF-451) - New Form Revision breaks the view to use in Form Data Mgt
- [PF-452](https://agile.venturetech.net/browse/PF-452) - MailTrackerResourceFactory doesn't set the factory ID on the resources it creates
- [PF-454](https://agile.venturetech.net/browse/PF-454) - Frontend User Management / Error getting domains that principal admins
- [PF-461](https://agile.venturetech.net/browse/PF-461) - Backend User Management / Web content permissions are not persisted
- [PF-463](https://agile.venturetech.net/browse/PF-463) - Label Management / Lazy init exception
- [PF-470](https://agile.venturetech.net/browse/PF-470) - Library Management / Changing library type or category doesn't change search results
- [PF-508](https://agile.venturetech.net/browse/PF-508) - Form Data Management / Can't add form data after switching forms
- [PF-512](https://agile.venturetech.net/browse/PF-512) - Form Management / Can't add items to Form Process Context
- [PF-513](https://agile.venturetech.net/browse/PF-513) - Form Management / Can't add action to form rules
- [PF-523](https://agile.venturetech.net/browse/PF-523) - Page Management / Flash bean doesn't show file selector
- [PF-525](https://agile.venturetech.net/browse/PF-525) - Page Management / URL field isn't shown when adding a menu item for an external URL
- [PF-528](https://agile.venturetech.net/browse/PF-528) - Default role selected by the Create Account component is the All Admin role
- [PF-541](https://agile.venturetech.net/browse/PF-541) - User Management / Editing password credentials silently fails
- [PF-588](https://agile.venturetech.net/browse/PF-588) - Email Template Management / Can't save email with content

### Story

- [PF-94](https://agile.venturetech.net/browse/PF-94) - Update dynamic entity manager to work with Hibernate 4
- [PF-119](https://agile.venturetech.net/browse/PF-119) - Port CustomDB
- [PF-238](https://agile.venturetech.net/browse/PF-238) - PrincipalAuthenticationDomainForm triggers clobber error
- [PF-421](https://agile.venturetech.net/browse/PF-421) - Reset Password Component Forms URL incorrectly
- [PF-501](https://agile.venturetech.net/browse/PF-501) - MIWT Field Component Async Input Listener
- [PF-562](https://agile.venturetech.net/browse/PF-562) - Update DomainModel API to use TextSource
- [PF-572](https://agile.venturetech.net/browse/PF-572) - In Page Management, removing components from a composite container then clicking undo to add them fails with error

## Changes in v0.6.1

### Bug

- [PF-588](https://agile.venturetech.net/browse/PF-588) - Email Template Management / Can't save email with content


## Changes in v0.6.0


This release includes API changes that are likely to affect most users.
For PF-540, we converted many APIs to use `TextSource` instead of `LocalizedText`
or `LocalizedObjectKey`. `LocalizedText` and `LocalizedObjectKey` are `TextSource`s.

The following methods have been deleted on UI components and related API:

- setTooltipKey
- setLabelKey
- setTextKey
- setConfirmTextKey
- setHintTextKey

You can use the following regular expressions to find and fix calls to those methods.

> Search  => set(Tooltip|Label|Text|ConfirmText)Key\s?[(]
>
> Replace => set$1(

and

> Search  => setHintTextKey\s?[(]
>
> Replace => setHint(


In addition to having a new API, `TextSource`, for referencing internationalized or 
non-internationalized text there is a utility class, 
[TextSources](http://docs.proteusframework.com/version/0/api/core/net/proteusframework/core/locale/TextSources.html), 
for creating text sources that handles null checks so you don't have to.

The default MIWT cell renderers now use `TextSources.createForAny(Object)`
and `TextSources.createForTooltip(Object)`.


### Technical task

[PF-483](https://agile.venturetech.net/browse/PF-483) - Update TextSource API


### Bug

[PF-347](https://agile.venturetech.net/browse/PF-347) - Text Editor : Unable to save text

[PF-358](https://agile.venturetech.net/browse/PF-358) - Error trying to move folder to disk file storage

[PF-375](https://agile.venturetech.net/browse/PF-375) - Frontend User Management / Edit Login Info / !L10N! Error for password verify

[PF-415](https://agile.venturetech.net/browse/PF-415) - Calendar ignores _includeTime etc. when disabled

[PF-460](https://agile.venturetech.net/browse/PF-460) - Backend User Management / !L10N! error when editing login info

[PF-482](https://agile.venturetech.net/browse/PF-482) - Form Entry CMS Component / 500 error when submitting a form

[PF-487](https://agile.venturetech.net/browse/PF-487) - Form Management / ClassCastException when adding a Likert

[PF-489](https://agile.venturetech.net/browse/PF-489) - Form Management / Selectable regions are not sorted correctly

[PF-490](https://agile.venturetech.net/browse/PF-490) - Form Management / NPE when setting the default country for an address field

[PF-499](https://agile.venturetech.net/browse/PF-499) - StringTextSource / We have things that depend on toString producing human-readable output

[PF-502](https://agile.venturetech.net/browse/PF-502) - FormDAO.getFormDefinitionQLBuilder() returns a broken QLBuilder

[PF-505](https://agile.venturetech.net/browse/PF-505) - Form Data Management / File fields are not working

[PF-507](https://agile.venturetech.net/browse/PF-507) - Form Management / Can't delete revisions

[PF-518](https://agile.venturetech.net/browse/PF-518) - Form Data Management / !L10N! placeholders in CSV headers

[PF-521](https://agile.venturetech.net/browse/PF-521) - Page Management / Map Bean is not working

[PF-522](https://agile.venturetech.net/browse/PF-522) - Page Management / !L10N! placeholders in editor for Audio and Video beans

[PF-524](https://agile.venturetech.net/browse/PF-524) - Page Management / !L10N! placeholders in editor for Conditional Redirect bean

[PF-530](https://agile.venturetech.net/browse/PF-530) - Proteus depends on an internet connection

[PF-539](https://agile.venturetech.net/browse/PF-539) - ExpressionEditor / Save-Exit doesn't call listener so it doesn't save


### Improvement

[PF-408](https://agile.venturetech.net/browse/PF-408) - HTML and Class Changes to MIWT tables


### Story

[PF-102](https://agile.venturetech.net/browse/PF-102) - MIWT - Update TH column names to have a SPAN or DIV wrapper

[PF-122](https://agile.venturetech.net/browse/PF-122) - Cache Invalidation support for administrators

[PF-366](https://agile.venturetech.net/browse/PF-366) - Login Component HTML Issue with EULA hidden input

[PF-399](https://agile.venturetech.net/browse/PF-399) - Updates to Pager HTML

[PF-400](https://agile.venturetech.net/browse/PF-400) - Updates to UI Task Manager HTML

[PF-401](https://agile.venturetech.net/browse/PF-401) - Update the site name CSS conversion to use dash instead of underscore

[PF-438](https://agile.venturetech.net/browse/PF-438) - Unit test for CKEditor

[PF-442](https://agile.venturetech.net/browse/PF-442) - Basic test for all Proteus Backend UI

[PF-540](https://agile.venturetech.net/browse/PF-540) - Convert core UI API to use TextSource




## Changes in v0.5.1

### Bug
[PF-482](https://agile.venturetech.net/browse/PF-482) - Form Entry CMS Component / 500 error when submitting a form

## Changes in v0.5.0

### Story

[PF-62](https://agile.venturetech.net/browse/PF-62) - Upgrade to Spring version 4 And Support Java 8


## Changes in v0.4.12

### Bug
[PF-482](https://agile.venturetech.net/browse/PF-482) - Form Entry CMS Component / 500 error when submitting a form


## Changes in v0.4.11

### Bug

[PF-418](https://agile.venturetech.net/browse/PF-418) - Form: no Submit Action
[PF-423](https://agile.venturetech.net/browse/PF-423) - SSL redirect is forced when configured not to

## Changes in v0.4.10

### Bug

[PF-383](https://agile.venturetech.net/browse/PF-383) - MessageContainer causes javascript error in latest firefox.

[PF-405](https://agile.venturetech.net/browse/PF-405) - LabelExtension behaves incorrectly when accessing name.

[PF-406](https://agile.venturetech.net/browse/PF-406) - Form : Unable to add generator.

[PF-402](https://agile.venturetech.net/browse/PF-402) - New pages do not show in page selector UI.

### Story

[PF-396](https://agile.venturetech.net/browse/PF-396) - Change the default renderer for Pagers

## Changes in v0.4.9

2014-03-11  Russ Tennant

        Fix orm2dc Java Identifier:
        Make sure beanName is also a valid Java identifier
        in com.i2rd.hibernate.task.SchemaUpdateHelper.createDataConversion
        Put the version number at the end of the beanName.

        PF-388 Remove exclude for xml-apis on hibernate dependency.
        We have to exclude xml-apis on all dependencies.

        PF-387 Fix BIRT Batik PDF class loading error. Related to https://bugs.eclipse.org/bugs/show_bug.cgi?id=344560

## Changes in v0.4.8

2014-03-05  Jonathan Crosmer

        Add missing annotation to FormEditor

2014-03-04  Russ Tennant 

        build.gradle: Update for hibernate enhancer. Commented out currently.
        ProteusWebAppConfig: Create a constant for the property source name.

## Changes in v0.4.7

2014-03-04  Russ Tennant 

    Fix NPE introduced in previous release.

## Changes in v0.4.6

2014-03-03  Russ Tennant 

    [PF #356] Component Mgt / Search by Page type doesn't work

    [PF #357] ComboBox action listener doesn't work on first event
    Fixes a regression from a previous change. Do not invalidate parent when used as a renderer.

    [PF #359] Blocking - Detaching CSS from page management doesn't work
    Remove delete cascade from many-to-many property.

    [PF #365] Removing components from page doesn't update UI correctly
    Fixed several queries that had old/incorrect syntax.

    [PF #367] Reset Password Component / Underscore in component class
    Updated other class names with underscores as well.

    [PF #368] Logout Component / Switching between options does not update UI
    Added call to watch for changes to RadioButtons.

    Port fixes from https://support.i2rd.com/view.php?id=59222 PageAccessCapabilityDAO.java, PageElementTreeModel.java, SiteElementRenderer.java, PagePathNode.java:
> Remove "revocation = false" from queries since the return value depends on it. Update path matching to match all paths, not just folders.


## Changes in v0.4.5

2014-02-28 Russ Tennant

    [PF #359] Blocking - Detaching CSS from page management doesn't work
    Remove delete-orphan cascade from many-to-many property.
	
    [PF #360] Blocking - Can't log in via token
    Added methods for obtaining a Hostname or Site without
    having the RenderContext initialized. This allows the authentication
    domain to be retrieved before the CMS RenderContext has been
    initialized.

    Moved FilterChainProxy registration.

## Changes in v0.4.4

2014-02-27  Russ Tennant 

        Create ProteusShell so we can bootstrap the shell ourselves.
        Initially, this just changes how the application context is created.
        It now reads the system property spring.config to obtain spring
        @Configurations due to the bean ordering/overriding issue with the
        shell bootstrap class.

        [PF #349] Page Editor / Error trying to edit a box to override contents
        The SQL generated by the HQL query in CmsBackendDAO.hasContentForBox
        is invalid in the new version of hibernate. Rewrote the HQL in order
        to get hibernate to generate valid SQL.

        [PF #230] Update to support null password.

        [PF #230] Add CliCommand annotation as an entry point.

        [PF #230] Workaround for IndexOutOfBoundsException.

        [PF #230] Process for adding users to a fresh Proteus db snapshot
        Add data conversion for renaming default admin group and role.

        [PF #230] Process for adding users to a fresh Proteus db snapshot
        Created command to add users to the backend.

        [PF #350] Remove spacer from actions div.


## Changes in v0.4.3

2014-02-25  Russ Tennant 

        [PF #343] Add StaticKeyDataConfig command to Proteus Shell

        StaticKeyDataConfig: 
         Add missing properties to copy constructor. Add scanPackage mutators.

        [PF #327] Error on attempt to reset password
        Added a data conversion to add an email template for the
        backend reset password component.

2014-02-24  Russ Tennant 

        [PF #173] CommunicationConfig - not sure if in good package
        Moved cache configs to net.proteusframework.$module.config package.

        [PF #330] Changing revision limit caused files to be lost
        Add back check for same stream storage when processing files. Appears to have been accidentally removed when the email notifications were removed.

        [PF #314] Incorrect usage of window.setTimeout  method

        [PF #299] RadioButtonComponent has seemingly incorrect id attribute
        When converting some code to use dashes into underscores for consistency,
        the radio button ID was missed in one place causing a mismatch between
        the label.for and the input.id.

        [PF #331 #240] Template Management / CSS bug when editing name
        Invalidate parent in setVisible, setEnabled, and setEditable.

        [PF #326] Styles in menu component are missing
        miwt_highlight class was missing some replacements with miwt-tree class.

        [PF #318] Page Management / Live Preview Button Opens In Window
        When rendering an external action link, do not include the submit
        feature. The submit feature causes JavaScript code to handle opening
        a new window and we do not want to do that in this case.

        [PF #199] SAF - add the ability to pick files independently


## Changes in v0.4.0


* 2014-02-19  Ken Logan

	Fix bugs from integration testing for #184. Add data conversion.

	[PF #184] Remove direct references to all admin perm
	closes #184

* 2014-02-19  Russ Tennant

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

	
* 2014-02-19  Jonathan Crosmer

	Make the data conversion call CREATE EXTENSION automatically and have a better comment that the contrib package is required.  Fixes #322

	Change existing functions in '05-cms-functions.sql' and '20-text-functions.sql' to the new data conversion format. Also modified DynamicTableDAO so that it will initialize properly by disambiguating the LocaleSource.

* 2014-02-19  Justin Piper

	Add method to display the name and ID of all hostnames for a site
	closes #294

* 2014-02-19  Jonathan Crosmer

	[PF #297] Rename IDataProvider to remove "I"
	closes #297


