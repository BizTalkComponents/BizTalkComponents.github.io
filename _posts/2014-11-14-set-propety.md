---
layout: page
title: "Set Property"
category: ref
date: 2014-11-14 12:00:00
---

Source code and issues: https://github.com/BizTalkComponents/SetProperty

NuGet package: https://www.nuget.org/packages/BizTalkComponents.PipelineComponents.SetProperty/
Pipeline stage: Any
MSI installer: Not available
Streaming: N/A
Pipeline direction: Both

# Usage #
Promotes a specified value to a specified property.

This component is useful when you need to promote a hard coded value.

# Configuration & Properties ##
## Property Path (Required) ##
The path to the context property in the form of namespace#propertyname.

## Value (Required) ##
The value to promote.

# Remarks #
Throws ArgumentException if any of the required parameters is not specified.

If the message context that the components is trying to promote is not found, if for example that schema is not deployed, an exception will occur.

## Scenario ##

### Pre execution ###
Component configured with PropertyPath = http://tempuri.org#MyProperty and Value = Test

### Post execution ###
Message context will contain 

Name: MyProperty

Value: Test

Namespace: http://tempuri.org

Type: Promoted

