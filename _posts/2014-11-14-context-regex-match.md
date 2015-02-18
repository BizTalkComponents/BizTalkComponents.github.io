---
layout: page
title: "Context RegEx Match"
source: "https://github.com/BizTalkComponents/ContextRegExMatch"
nuget: "todo"
installer: "todo"
category: ref
date: 2014-11-14 12:00:00
---

## Usage ##
The Context RegEx Match component contains functionality to read a specific value in the context of a message, 
perform a regular expression match on that value and in case of a successful match promote a fixed value 
to another part of the message context. 

The component is useful when receiving a message with a promoted value in its context that one then want to evaluate rules against to for example simplify filtering in routing of messages. 

## Properties ##
<table>
    <tr>
        <td>Pattern To Match</td>
        <td>Required</td>
        <td>The RegEx pattern used to match the specific context value against.</td>
    </tr>
    <tr>
        <td>Context Property To Match</td>
        <td>Required</td>
        <td>Namespace and value of the context property that the match should execute against. 
Should be in format `http://foo.bar#value`. </td>
    </tr>
    <tr>
        <td>Context Property To Set</td>
        <td>Required</td>
        <td>Namespace and value of the context property that should be used to the set the value. 
Should be in format `http://foo.bar#value`. </td>
    </tr>
     <tr>
        <td>Value To Set</td>
        <td>Required</td>
        <td>The value to set if the match is successful.</td>
    </tr>
</table>

## Remarks ##
If the component receives null when trying to reading the value that the match should be performed against an exception will occur. 

If the message context that the components is trying to promote is not found, if for example that schema is not deployed, an exception will occur.