---
layout: page
title: "Promote Db Query Result - xPath Value Exists"
source: "https://github.com/BizTalkComponents/PromoteDbQueryResult"
nuget: "https://www.nuget.org/packages/BizTalkComponents.PipelineComponents.PromoteDbQueryResult.XPathValueExists/"
installer: ""
category: ref
date: 2014-11-14 12:00:00
---

## Usage ##
Promotes <code>True</code> in the specified output context property if the input xPath value exists in the database, <code>False</code> otherwise.

This component is useful when you need to promote whether a value exists or not in a database.

## Properties ##
<table class="properties">
    <tr>
        <td>DbColumnName</td>
        <td>Required</td>
        <td>The name of the database column to check the input context property value against.</td>
    </tr>
    <tr>
        <td>DbColumnType</td>
        <td>Required</td>
        <td>The type of the database column, <code>Int/String</code>.</td>
    </tr>
	<tr>
        <td>DbConnectionString</td>
        <td>Required</td>
        <td>The database connection string.</td>
    </tr>
    <tr>
        <td>DbProvider</td>
        <td>Required</td>
        <td>The database provider.</td>
    </tr>
    <tr>
        <td>DbTableName</td>
        <td>Required</td>
        <td>The name of the database table.</td>
    </tr>
    <tr>
        <td>InputXPath</td>
        <td>Required</td>
        <td>The input xPath.</td>
    </tr>
    <tr>
        <td>OutputPropertyPath</td>
        <td>Required</td>
        <td>The output context property path holding the result from the database query.</td>
    </tr>
</table>

## Remarks ##
Throws ArgumentException if any of the required parameters is not specified.

