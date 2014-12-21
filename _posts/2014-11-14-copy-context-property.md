---
layout: page
title: "Copy Context Property"
category: ref
date: 2014-12-21 12:00:00
---

Source code and issues: https://github.com/BizTalkComponents/CopyContextProperty

NuGet package: https://www.nuget.org/packages/BizTalkComponents.PipelineComponents.CopyContextProperty/
Pipeline stage: Any
MSI installer: Not available
Streaming: N/A
Pipeline direction: Both

# Usage #
Copies a value from a specified context property to another context property.

This component is useful when you need to promote a hard coded value.

# Configuration & Properties ##
## Source Property (Required) ##
The property path of the property to copy from.

## DestinationProperty (Required) ##
The property path of the property to copy to.

# Remarks #
Throws ArgumentException if any of the required parameters is not specified.

If the message context that the components is trying to promote is not found, if for example that schema is not deployed, an exception will occur.

## Scenario ##

### Pre execution ###
Component configured with SourceProperty = http://tempuri.org#MyProperty
Component configured with DestinationProperty = "http://mynamespace#MyOtherProperty"

### Post execution ###
http://mynamespace#MyOtherProperty  is propmoted with the value of http://tempuri.org#MyProperty

