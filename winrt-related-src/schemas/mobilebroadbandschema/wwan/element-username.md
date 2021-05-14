---
description: Defines the user name for logon.
Search.Product: eADQiWindows 10XVcnh
title: UserName (WWAN schema, descendant of DefaultProfile)
ms.assetid: 5c377a0a-ca24-4a24-85c0-79d5bc6af8ef

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# UserName (WWAN schema, descendant of DefaultProfile)


Defines the user name for logon. Must be less than 256 characters.

## Element hierarchy

<dl>
<dt><a href="element-defaultprofile.md">&lt;DefaultProfile&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-context.md">&lt;Context&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-userlogoncred.md">&lt;UserLogonCred&gt;</a></dt>
<dd><b>&lt;UserName&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>
<dl>
<dt><a href="element-purchaseprofile.md">&lt;PurchaseProfile&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-1-context.md">&lt;Context&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-1-userlogoncred.md">&lt;UserLogonCred&gt;</a></dt>
<dd><b>&lt;UserName&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<UserName>

  NameType

</UserName>
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
<td><a href="element-userlogoncred.md">UserLogonCred</a> </td>
<td><p>Defines logon credentials for a connection.</p></td>
</tr>
</tbody>
</table>

 

## Requirements

|          | Value |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControl/WWAN/v1` |

 

 



