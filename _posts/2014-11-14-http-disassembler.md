---
layout: page
title: "Http Disassembler"
category: ref
date: 2014-12-22 12:00:00
---

Source code and issues: https://github.com/BizTalkComponents/ContextRegExMatch

NuGet package:
Pipeline stage: Any
MSI installer:
Streaming: N/A
Pipeline direction: Receive

## Usage ##
The HttpDisassembler component is used to create a message body from the URL in a HTTP GET request. More info available at: 
http://blog.ibiz-solutions.se/integration/exposing-a-rest-get-endpoint-using-biztalk-server-2013/

## Configuration & Properties ###
### DocumentSpecName (Required) ###
The document spec name of the schema to create a message from.

## Remarks ##
If the component receives null when trying to reading the value that the match should be performed against an exception will occur. 

