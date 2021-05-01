---
description: The minimum version of the operating system that the package requires.
Search.Product: eADQiWindows 10XVcnh
title: OSMinVersion (Windows 8 package schema)
ms.assetid: 18c045dd-7e8c-431c-b3d8-bc3056575632


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# OSMinVersion (package schema for Windows 8)


The minimum version of the operating system that the package requires.

## Element hierarchy

<dl>
<dt><a href="element-package.md">&lt;Package&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-prerequisites.md">&lt;Prerequisites&gt;</a></dt>
<dd><b>&lt;OSMinVersion&gt;</b></dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<OSMinVersion>

  A version string in duo notation (major.minor) or trio notation (major.minor.appversion).

</OSMinVersion>
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
<td><a href="element-prerequisites.md">Prerequisites</a> </td>
<td><p>Declares the minimum operating system and software requirements that must exist for the package to be applicable to the system.</p></td>
</tr>
</tbody>
</table>

 

## Remarks

The system blocks install or update of an app on a computer if the value of **OSMinVersion** specified in the package manifest is greater than the version of the operating system.

In the version string, *major*.*minor*.*appversion*, the first two fields represent the operating system version. The third field is optional and defaults to the app version of the operating system.

## Requirements

|               |                                                             |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2010/manifest` |

 

 



