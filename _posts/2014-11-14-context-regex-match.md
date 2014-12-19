---
layout: page
title: "Context RegEx Match component"
category: ref
date: 2014-11-14 12:00:00
---

Source code and issues: https://github.com/BizTalkComponents/ContextRegExMatch

NuGet package:
Pipeline stage: Any
MSI installer:
Streaming: N/A
Pipeline direction: Receive

# Usage #
The Context RegEx Match component contains functionality to read a specific value in the context of a message, 
perform a regular expression match on that value and in case of a successful match promote a fixed value 
to another part of the message context. 

The component is useful when receiving a message with a promoted value in its context that one then want to evaluate rules against to for example simplify filtering in routing of messages. 

# Configuration & Properties ##
## Pattern To Match (Required) ##
The RegEx pattern used to match the specific context value against.

## Context Property To Match (Required) ##
Namespace and value of the context property that the match should execute against. 
Should be in format `http://foo.bar#value`.

## Context Property To Set (Required) ##
Namespace and value of the context property that should be used to the set the value. 
Should be in format `http://foo.bar#value`.

## Value To Set (Required) ##
The value to set if the match is successful.

# Remarks #
If the component receives null when trying to reading the value that the match should be performed against an exception will occur. 

If the message context that the components is trying to promote is not found, if for example that schema is not deployed, an exception will occur.


In a scenario with the message context shown below.

Name | Value | Namespace
---- | ----- | ---------
Test | 752368 |  http://acmeset1.com/prop

First set the `Pattern To Match` property to `^.{2}23` to match `23` in the third and forth position of the context value. Then set the  `Context Property To Match` property to `http://acmeset1.com/prop#test` to point to the correct context property to match against.

Secondly one has to set the `Context Property To Set` to something like `http://acmeset2.com/prop#test2` to point to the new context property one want to set. Finally one has to set the `Value To Set` property to the value to set in case of a successful match. In this example we will set the value to `OK`.

Name | Value | Namespace
---- | ----- | ---------
Test | 752368 |  http://acmeset1.com/prop
Test | OK |  http://acmeset2.com/prop