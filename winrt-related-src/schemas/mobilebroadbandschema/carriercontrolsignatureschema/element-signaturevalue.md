---
description: Defines the signature thumbprint.
Search.Product: eADQiWindows 10XVcnh
title: SignatureValue
ms.assetid: 52ffacf0-920a-4bde-9b2e-9589161a57ff

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# SignatureValue


Defines the signature thumbprint as specified in [XML DSIG](https://www.w3.org/TR/xmldsig-core/). The algorithm used to generate [**SignatureValue**](element-signaturevalue.md) is defined in [**SignatureMethod**](element-signaturemethod.md).

## Element hierarchy

<dl>
<dt><a href="element-signature.md">&lt;Signature&gt;</a></dt>
<dd><b>&lt;SignatureValue&gt;</b></dd>
</dl>

## Syntax

``` syntax
<SignatureValue Id? = ID >

  base64Binary

</SignatureValue>
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
<td><strong>Id</strong></td>
<td><p>A unique element identifier to be used as a reference to <a href="element-signaturevalue.md"><strong>SignatureValue</strong></a> .</p></td>
<td>ID</td>
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
<td><a href="element-signature.md">Signature</a> </td>
<td><p>Defines the root element of an <a href="https://www.w3.org/TR/xmldsig-core/">XML DSIG</a>  compliant signature. <a href="element-signature.md"><strong>Signature</strong></a> is the unique root element for a provisioning file signature.</p></td>
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

 

 



