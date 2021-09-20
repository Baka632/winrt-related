---
description: Contains the name of the subscriber's data plan (WWAN schema, descendant of DefaultProfile).
Search.Product: eADQiWindows 10XVcnh
title: AssociatedPlan (WWAN schema, descendant of DefaultProfile)
ms.assetid: fdfc0657-a653-4fed-b0ae-b60e94af03ee

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# AssociatedPlan (WWAN schema, descendant of DefaultProfile)


Contains the name of the subscriber's data plan. It must match the **Name** attribute of a [**Plan**](../plans/element-plan.md) in the same XML document.

## Element hierarchy

<dl>
<dt><a href="element-defaultprofile.md">&lt;DefaultProfile&gt;</a></dt>
<dd><b>&lt;AssociatedPlan&gt;</b></dd>
</dl>

## Syntax

``` syntax
<AssociatedPlan>

  string

</AssociatedPlan>
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

 

## Requirements

|          | Value |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControl/WWAN/v1` |

 

 
