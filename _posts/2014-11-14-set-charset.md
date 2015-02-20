---
layout: page
title: "Set Charset
source: "https://github.com/BizTalkComponents/SetCharset"
nuget: "https://www.nuget.org/packages/BizTalkComponents.PipelineComponents.SetCharset/"
installer: "https://biztalkcomponentsstorage.blob.core.windows.net/deployments/Build/BizTalkComponents.PipelineComponents.SetCharset_1.0.5.msi"
category: ref
date: 2014-11-14 12:00:00
---

## Usage ##
Intended to be used on a ReceivePort to tell the disassembler what encoding is used. The component does this by setting the TargetCharset property of the body message part.


## Properties ##
<table class="properties">
    <tr>
        <td>TargetCharset</td>
        <td>Required</td>
        <td>The charset to be used.</td>
    </tr>
</table>

## Remarks ##
 Throws ArgumentException if a non existing charset is specified.

