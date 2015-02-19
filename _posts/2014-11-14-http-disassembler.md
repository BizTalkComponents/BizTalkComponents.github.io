---
layout: page
title: "Http Disassembler"
source: "https://github.com/BizTalkComponents/HttpDisassembler"
nuget: "https://www.nuget.org/packages/BizTalkComponents.PipelineComponents.HttpDisassembler/"
installer: "https://biztalkcomponentsstorage.blob.core.windows.net/deployments/Build/BizTalkComponents.PipelineComponents.HttpDisassembler_1.0.3.msi"
category: ref
date: 2014-11-14 12:00:00
---

## Usage ##
The HttpDisassembler component is used to create a message body from the URL in a HTTP GET request. More info available at: 
http://blog.ibiz-solutions.se/integration/exposing-a-rest-get-endpoint-using-biztalk-server-2013/

## Properties ##
<table class="properties">
    <tr>
        <td>DocumentSpecName</td>
        <td>Required</td>
        <td>The fully qualified name of the schema to create an instance from.</td>
    </tr>
</table>

## Remarks ##
If the DocumentSpecName is not set an ArgumentException will be thrown. If the specified schema does not exist in GAC an exception will be thrown.

