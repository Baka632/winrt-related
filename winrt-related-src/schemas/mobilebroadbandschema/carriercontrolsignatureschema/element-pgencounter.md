---
description: efines a Digital Signature Algorithm (DSA) prime generation counter.
Search.Product: eADQiWindows 10XVcnh
title: PgenCounter
ms.assetid: 46445ef4-1aaf-43cf-9ce2-f6a587a425fe

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# PgenCounter


Defines a Digital Signature Algorithm (DSA) prime generation counter as specified in [XML DSIG](https://www.w3.org/TR/xmldsig-core/).

## Element hierarchy

<dl>
<dt><a href="element-signature.md">&lt;Signature&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-keyinfo.md">&lt;KeyInfo&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-keyvalue.md">&lt;KeyValue&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-dsakeyvalue.md">&lt;DSAKeyValue&gt;</a></dt>
<dd><b>&lt;PgenCounter&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<PgenCounter>

  base64Binary

</PgenCounter>
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
<td><a href="element-dsakeyvalue.md">DSAKeyValue</a> </td>
<td><p>Defines a Digital Signature Algorithm (DSA) public key as specified in <a href="https://www.w3.org/TR/xmldsig-core/">XML DSIG</a> .</p></td>
</tr>
</tbody>
</table>

 

## Requirements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Namespace</p></td>
<td><p>http://www.w3.org/2000/09/xmldsig#</p></td>
</tr>
</tbody>
</table>

 

 



