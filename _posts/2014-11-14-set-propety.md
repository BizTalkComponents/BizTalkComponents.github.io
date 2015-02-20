---
layout: page
title: "Set Property"
source: "https://github.com/BizTalkComponents/SetProperty"
nuget: "https://www.nuget.org/packages/BizTalkComponents.PipelineComponents.SetProperty/"
installer: "https://biztalkcomponentsstorage.blob.core.windows.net/deployments/Build/BizTalkComponents.PipelineComponents.SetProperty_1.0.6.msi"
category: ref
date: 2014-11-14 12:00:00
---

## Usage ##
Promotes a specified value to a specified property.

This component is useful when you need to promote a hard coded value.

## Properties ##
<table class="properties">
    <tr>
        <td>PropertyPath</td>
        <td>Required</td>
        td>Namespace and value of the context property to promote to.
Should be in format <code>http://foo.bar#value</code>.</td>
    </tr>
	<tr>
        <td>Value</td>
        <td>Required</td>
        td>The value to promote.</td>
    </tr>
</table>

## Remarks ##
Throws ArgumentException if any of the required parameters is not specified.
