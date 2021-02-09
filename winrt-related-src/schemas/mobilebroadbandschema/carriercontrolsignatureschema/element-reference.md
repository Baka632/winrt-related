---
description: efines a digest value, digest method, and transforms as specified in XML DSIG.
Search.Product: eADQiWindows 10XVcnh
title: Reference
ms.assetid: 4a15880c-f401-4056-943c-33e6729b13cd

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# Reference


Defines a digest value, digest method, and transforms as specified in [XML DSIG](https://www.w3.org/TR/xmldsig-core/).

## Element hierarchy

<dl>
<dt><a href="element-signature.md">&lt;Signature&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-signedinfo.md">&lt;SignedInfo&gt;</a></dt>
<dd><b>&lt;Reference&gt;</b></dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<Reference Id?  = ID
           URI? = anyURI >

  <!-- Child elements -->
  Transforms,
  DigestMethod,
  DigestValue

</Reference>
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
<td><p>A unique element identifier to be used as a reference to <a href="element-reference.md"><strong>Reference</strong></a> .</p></td>
<td>ID</td>
<td>No</td>
<td></td>
</tr>
<tr class="even">
<td><strong>URI</strong></td>
<td><p>Defines the Uniform Resource Locator (URI) of the digested data object.</p></td>
<td>anyURI</td>
<td>No</td>
<td></td>
</tr>
</tbody>
</table>

 

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
<td><a href="element-digestmethod.md">DigestMethod</a> </td>
<td><p>Defines the algorithm used to generate <a href="element-digestvalue.md"><strong>DigestValue</strong></a>  as specified in <a href="https://www.w3.org/TR/xmldsig-core/">XML DSIG</a>.</p></td>
</tr>
<tr class="even">
<td><a href="element-digestvalue.md">DigestValue</a> </td>
<td><p>Defines the digest value as specified in <a href="https://www.w3.org/TR/xmldsig-core/">XML DSIG</a> . The algorithm used to generate <a href="element-digestvalue.md"><strong>DigestValue</strong></a> is defined in <a href="element-digestmethod.md"><strong>DigestMethod</strong></a>.</p></td>
</tr>
<tr class="odd">
<td><a href="element-transforms.md">Transforms</a> </td>
<td><p>Defines a an ordered list of transforms applied to the digested data object as specified in <a href="https://www.w3.org/TR/xmldsig-core/">XML DSIG</a> .</p></td>
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
<td><a href="element-signedinfo.md">SignedInfo</a> </td>
<td><p>Defines all signed content within the signature as specified in <a href="https://www.w3.org/TR/xmldsig-core/">XML DSIG</a> .</p></td>
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

 

 



