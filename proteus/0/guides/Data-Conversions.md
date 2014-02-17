---
title: Data Conversions
layout: guide
---

# Overview
TODO - why do we have them, what kinds of things can be in conversion (e.g., SQL, schema changes, functions, indices)

- mention Spring Shell

## Automation Tasks
TODO
Tasks are registered for use as Spring beans. If a Task / DataConversion is registered via a Java config, a @Profile referencing the version number of the software should be used.

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
