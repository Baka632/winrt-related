---
description: Defines a value representing the effective link speed of the subscriber’s connection specified in Kbps.
Search.Product: eADQiWindows 10XVcnh
title: BandwidthInKbps
ms.assetid: 404712b0-a232-4967-83ac-51fd35d0ef88

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# BandwidthInKbps


Defines a value representing the effective link speed of the subscriber’s connection specified in Kbps. Must be a value from 0 to 2<sup>32nd</sup>.

## Element hierarchy

<dl>
<dt><a href="element-cost.md">&lt;Cost&gt;</a></dt>
<dd><b>&lt;BandwidthInKbps&gt;</b></dd>
</dl>

## Syntax

``` syntax
<BandwidthInKbps>

  nonNegativeInteger

</BandwidthInKbps>
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
<td><a href="element-cost.md">Cost</a> </td>
<td><p>Defines a set of meter cost information that specifies the metered state of a subscriber's connection to a Mobile Network Operator (MNO). <a href="element-cost.md"><strong>Cost</strong></a>  is the unique root element for DUSM cost information.</p></td>
</tr>
</tbody>
</table>

 

## Requirements

|          | Value        |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControl/DUSM/v1` |

 

 



