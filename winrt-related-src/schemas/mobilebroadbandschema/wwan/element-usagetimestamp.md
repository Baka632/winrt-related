---
description: Defines a validity date and time of the usage information
Search.Product: eADQiWindows 10XVcnh
title: UsageTimestamp
ms.assetid: 413a560b-8635-4fec-b0f8-e479cf421eef

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# UsageTimestamp


Defines a validity date and time of the usage information.

## Element hierarchy

<dl>
<dt><a href="element-messages.md">&lt;Messages&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-message.md">&lt;Message&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-fields.md">&lt;Fields&gt;</a></dt>
<dd><b>&lt;UsageTimestamp&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<UsageTimestamp Format   = string
                Group    = positiveInteger
                AmToken? = string
                PmToken? = string />
```

### Key

`?`   optional (zero or one)

## Attributes and Elements


### Attributes

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Attribute</th>
<th>Description</th>
<th>Data type</th>
<th>Required</th>
<th>Default value</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong>AmToken</strong></td>
<td><p>AM token matched against an occurrence of %p in <strong>Format</strong>.</p></td>
<td>string</td>
<td>No</td>
<td></td>
</tr>
<tr class="even">
<td><strong>Format</strong></td>
<td><p>Defines a format string used to parse <strong>Group</strong>. It contains a subset of the <a href="https://msdn.microsoft.com/library/fe06s4ak(VS.71">strftime</a> .aspx) format codes:</p>
%d Day of month as decimal number (01 – 31)
%H Hour in 24-hour format (00 – 23)
%I Hour in 12-hour format (01 – 12)
%m Month as decimal number (01 – 12)
%M Minute as decimal number (00 – 59)
%S Second as decimal number (00 – 59)
%y Year without century, as decimal number (00 – 99)
%Y Year with century, as decimal number (0000-9999)
%p AM/PM indicator
%#d, %#H, %#I, %#m, %#M, %#S, %#y, %#Y -- Same as above but with no leading zeros</td>
<td>string</td>
<td>Yes</td>
<td></td>
</tr>
<tr class="odd">
<td><strong>Group</strong></td>
<td><p>Defines the group which contains a date and time whose format is defined in <strong>Format</strong>. Month and day are required; if no year is provided, the most recent occurrence of that date is assumed.</p></td>
<td>positiveInteger</td>
<td>Yes</td>
<td></td>
</tr>
<tr class="even">
<td><strong>PmToken</strong></td>
<td><p>PM token matched against an occurrence of %p in <strong>Format</strong>.</p></td>
<td>string</td>
<td>No</td>
<td></td>
</tr>
</tbody>
</table>

 

### Child Elements

None.

### Parent Elements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parent Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><a href="element-fields.md">Fields</a> </td>
<td><p>Defines values that describe the subscriber's plan and data usage.</p></td>
</tr>
</tbody>
</table>

 

## Remarks

The **UsageTimestamp** element must be included if any of the following elements are included in the schema:

-   **Usage**
-   **UsagePercentage**
-   **UsageOverage**
-   **UsageOveragePercentage**

The **UsageTimestamp** element must not be included if none of the following elements are included in the schema:

-   **Usage**
-   **UsagePercentage**
-   **UsageOverage**
-   **UsageOveragePercentage**

## Requirements

|          | Value |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControl/WWAN/v1` |

 

 



