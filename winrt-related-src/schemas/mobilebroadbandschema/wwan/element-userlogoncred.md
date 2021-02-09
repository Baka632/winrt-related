---
description: Defines logon credentials for a connection.
Search.Product: eADQiWindows 10XVcnh
title: UserLogonCred
ms.assetid: 0d8748d5-a1e7-4535-a5cc-9c9f380eed32

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# UserLogonCred


Defines logon credentials for a connection.

## Element hierarchy

<dl>
<dt><a href="element-defaultprofile.md">&lt;DefaultProfile&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-context.md">&lt;Context&gt;</a></dt>
<dd><b>&lt;UserLogonCred&gt;</b></dd>
</dl>
</dd>
</dl>
<dl>
<dt><a href="element-purchaseprofile.md">&lt;PurchaseProfile&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-1-context.md">&lt;Context&gt;</a></dt>
<dd><b>&lt;UserLogonCred&gt;</b></dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<UserLogonCred>

  <!-- Child elements -->
  UserName,
  Password?

</UserLogonCred>
```

### Key

`?`   optional (zero or one)

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
<td><a href="element-password.md">Password</a> </td>
<td><p>Defines the password used to authenticate a user. Must be less than 256 characters.</p></td>
</tr>
<tr class="even">
<td><a href="element-username.md">UserName</a> </td>
<td><p>Defines the user name for logon. Must be less than 256 characters.</p></td>
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
<td><a href="element-context.md">Context</a> </td>
<td><p>Defines the parameters required to setup a data connection.</p></td>
</tr>
</tbody>
</table>

 

## Requirements

|          |         |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControl/WWAN/v1` |

 

 



