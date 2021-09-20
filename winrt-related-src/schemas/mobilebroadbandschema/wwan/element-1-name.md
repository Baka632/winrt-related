---
description: Defines the profile name (child of DefaultProfile).
Search.Product: eADQiWindows 10XVcnh
title: 'Name (WWAN schema, child of DefaultProfile)'
ms.assetid: 9eab41c7-29ff-42aa-9647-f18ff72b3faf

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# Name (WWAN schema, child of DefaultProfile)


Defines the profile name. Must be 64 characters or less.

## Element hierarchy

<dl>
<dt><a href="element-defaultprofile.md">&lt;DefaultProfile&gt;</a></dt>
<dd><b>&lt;Name&gt;</b></dd>
</dl>
<dl>
<dt><a href="element-purchaseprofile.md">&lt;PurchaseProfile&gt;</a></dt>
<dd><b>&lt;Name&gt;</b></dd>
</dl>

## Syntax

``` syntax
<Name>

  NameType

</Name>
```

## Attributes and Elements


### Attributes

None.

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
<td><a href="element-defaultprofile.md">DefaultProfile</a> </td>
<td><p>Defines the default connection profile used by a subscriber to connect to a MNO. The Mobile Broadband service will use these connection settings without prompting the user for details.</p></td>
</tr>
<tr class="even">
<td><a href="element-purchaseprofile.md">PurchaseProfile</a> </td>
<td><p>Defines a purchase connection profile used by a subscriber to connect to a MNO.</p></td>
</tr>
</tbody>
</table>

 

## Related elements


The following elements have the same name as this one, but different content or attributes:

-   **[Name (in type: Branding)](element-name.md)**

## Remarks

**name** is formed as *Issuer-Customer-Name*, where *Issuer* and *Customer* are strings from the root of the provisioning file, and *Name* is the value for *Name* supplied by the MNO.

## Requirements

|          | Value |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControl/WWAN/v1` |

 

 



