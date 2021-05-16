---
description: Defines selection criteria for the certificates defined for the package.
Search.Product: eADQiWindows 10XVcnh
title: SelectionCriteria (Windows 8 package schema)
ms.assetid: 5f3d9db3-5b2d-44ec-9607-dcc15f0854b5


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# SelectionCriteria (package schema for Windows 8)


Defines selection criteria for the certificates defined for the package.

## Element hierarchy

<dl>
<dt><a href="element-package.md">&lt;Package&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-extensions.md">&lt;Extensions&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-extension.md">&lt;Extension&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-certificates.md">&lt;Certificates&gt;</a></dt>
<dd><b>&lt;SelectionCriteria&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<SelectionCriteria HardwareOnly? = boolean
                   AutoSelect?   = boolean />
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
<td><strong>AutoSelect</strong></td>
<td><p><strong>true</strong> if the certificates are selected automatically; otherwise, <strong>false</strong>.</p></td>
<td>boolean</td>
<td>No</td>
<td></td>
</tr>
<tr class="even">
<td><strong>HardwareOnly</strong></td>
<td><p><strong>true</strong> if the specified certificates are hardware-specific; otherwise, <strong>false</strong>.</p></td>
<td>boolean</td>
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
<td><a href="element-certificates.md">Certificates</a> </td>
<td><p>Declares a package extensibility point of type <strong>windows.certificates</strong>. The app requires one or more certificates from the specified certificate stores.</p></td>
</tr>
</tbody>
</table>

 

## Requirements

|               |   Value                                                          |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2010/manifest` |

 

 



