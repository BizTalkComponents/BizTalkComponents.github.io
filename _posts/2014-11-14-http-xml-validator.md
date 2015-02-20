---
layout: page
title: "Http Xml Validator"
source: "https://github.com/BizTalkComponents/HttpXmlValidator"
nuget: "https://www.nuget.org/packages/BizTalkComponents.PipelineComponents.HttpXmlValidator/"
installer: "https://biztalkcomponentsstorage.blob.core.windows.net/deployments/Build/BizTalkComponents.PipelineComponents.HttpXmlValidator_1.0.13.msi"
category: ref
date: 2014-11-14 12:00:00
---

## Usage ##
Intended to be used together with the WebHttp adapter. Uses XmlValidator component to validate the XML instance and return HTTP 400 to the client if the message is not valid. 

This component is useful when you need to reject invalid XML messages received via HTTP.

## Properties ##
<table class="properties">
    <tr>
        <td>RecoverableInterchangeProcessing </td>
        <td>Optional</td>
        <td>Exposes XmlValidator components RecoverableInterchangeProcessing parameter. 
			http://msdn.microsoft.com/en-us/library/dd224149.aspx</td>
    </tr>
</table>

## Remarks ##
Throws InvalidOperation if receive port is not Request Response.