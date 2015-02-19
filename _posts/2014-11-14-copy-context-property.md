---
layout: page
title: "Copy Context Property"
source: "https://github.com/BizTalkComponents/CopyContextProperty"
nuget: "https://www.nuget.org/packages/BizTalkComponents.PipelineComponents.CopyContextProperty/"
installer: "https://biztalkcomponentsstorage.blob.core.windows.net/deployments/Build/BizTalkComponents.PipelineComponents.CopyContextProperty_1.0.12.msi"
category: ref
date: 2014-11-14 12:00:00
---

## Usage ##
Copies a value from a specified context property to another context property.

This component is useful when you need to promote a property based on another property.

## Properties ##
<table class="properties">
    <tr>
        <td>SourceProperty</td>
        <td>Required</td>
        <td>Namespace and value of the context property to copy <b>from</b>.
Should be in format <code>http://foo.bar#value</code>.</td>
    </tr>
    <tr>
        <td>DestinationProperty</td>
        <td>Required</td>
        <td>Namespace and value of the context property to copy <b>to</b>.
Should be in format <code>http://foo.bar#value</code>. </td>
    </tr>
</table>

## Remarks ##
Throws ArgumentException if any of the required parameters is not specified.

If the message context property that the components is trying to promote is not found, if for example that schema is not deployed, an exception will occur.

