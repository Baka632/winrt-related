---
description: Defines which key index should be used to encrypt wireless traffic.
Search.Product: eADQiWindows 10XVcnh
title: keyIndex
ms.assetid: 0d8686f8-8dfa-4677-9a6d-c59e18d8ef59

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# keyIndex


Defines which key index should be used to encrypt wireless traffic. [**keyIndex**](element-keyindex.md) is only used when [**keyType**](element-keytype.md) is **networkKey**. The default value is 0 when [**sharedKey**](element-sharedkey.md) is present. Must be a value between 0 and 3 inclusive.

## Element hierarchy

<dl>
<dt><a href="element-wlanprofile.md">&lt;WLANProfile&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-msm.md">&lt;MSM&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-security.md">&lt;security&gt;</a></dt>
<dd><b>&lt;keyIndex&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<keyIndex>

  integer

</keyIndex>
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
<td><a href="element-security.md">security</a> </td>
<td><p>Defines various security settings for this profile on a WLAN.</p></td>
</tr>
</tbody>
</table>

 

## Requirements

|          |         |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControl/WLAN/v1` |

 

 



