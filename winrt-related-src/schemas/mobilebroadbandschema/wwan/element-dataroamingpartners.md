---
description: Defines the list of preferred network providers for roaming.
Search.Product: eADQiWindows 10XVcnh
title: DataRoamingPartners (child of DefaultProfile)
ms.assetid: c29edf9c-4e70-4b8f-8c71-0ec8a9fad60d

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# DataRoamingPartners (child of DefaultProfile)


Defines the list of preferred network providers for roaming.

## Element hierarchy

<dl>
<dt><a href="element-defaultprofile.md">&lt;DefaultProfile&gt;</a></dt>
<dd><b>&lt;DataRoamingPartners&gt;</b></dd>
</dl>

## Syntax

``` syntax
<DataRoamingPartners>

  <!-- Child elements -->
  Provider+

</DataRoamingPartners>
```

### Key

`+`   required (one or more)

## Attributes and Elements


### Attributes

None.

### Child Elements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Child Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><a href="element-provider.md">Provider</a> </td>
<td><p>Defines the name and provider ID of a cellular network.</p></td>
</tr>
</tbody>
</table>

 

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
<td><a href="element-defaultprofile.md">DefaultProfile</a> </td>
<td><p>Defines the default connection profile used by a subscriber to connect to a MNO. The Mobile Broadband service will use these connection settings without prompting the user for details.</p></td>
</tr>
</tbody>
</table>

 

## Remarks

The Mobile Broadband service uses this element to select the preferred network provide while roaming.

## Requirements

|          | Value |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControl/WWAN/v1` |

 

 



