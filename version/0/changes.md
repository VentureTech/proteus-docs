---
title: Changes
layout: default
---

# Version 0 of the Proteus Framework

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


