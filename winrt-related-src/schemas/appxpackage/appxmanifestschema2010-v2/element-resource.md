---
description: Declares a language for the resource contained in the package.
Search.Product: eADQiWindows 10XVcnh
title: Resource (Windows 8.1 extensions schema)
ms.assetid: 445e7de7-e778-4666-b099-3d7f6f0125c7


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# Resource (extensions schema for Windows 8.1)




Declares a language for the resource contained in the package. The scale and DirectX feature level attributes are common for all resources in the package.

## Element hierarchy

<dl>
<dt><a href="element-package.md">&lt;Package&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-resources.md">&lt;Resources&gt;</a></dt>
<dd><b>&lt;Resource&gt;</b></dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<Resource Language?         = language
          m:Scale?          = "100" | "120" | "140" | "150" | "160" | ...
          m:DXFeatureLevel? = "dx9" | "dx10" | "dx11" />
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
<td><strong>Language</strong></td>
<td><p>The language for the resource contained in the package. The syntax of this attribute is defined by the IETF's <a href="https://www.rfc-editor.org/rfc/bcp/bcp47.txt">BCP47: Tags for Identifying Languages</a> .</p></td>
<td>language</td>
<td>No</td>
<td></td>
</tr>
<tr class="even">
<td><strong>m:DXFeatureLevel</strong></td>
<td><p>The DirectX <a href="/windows/win32/direct3d11/overviews-direct3d-11-devices-downlevel-intro#overview">feature level</a>  of the resource from the manifest's Resources\Resource field.</p></td>
<td><p>This attribute can have one of the following values:</p>
<ul>
<li>dx9</li>
<li>dx10</li>
<li>dx11</li>
</ul></td>
<td>No</td>
<td></td>
</tr>
<tr class="odd">
<td><strong>m:Scale</strong></td>
<td><p>The <a href="/uwp/api/Windows.Graphics.Display.ResolutionScale"><strong>resolution scale</strong></a>  of the resource.</p></td>
<td><p>This attribute can have one of the following values:</p>
<ul>
<li>100</li>
<li>120</li>
<li>140</li>
<li>150</li>
<li>160</li>
<li>180</li>
<li>225</li>
</ul></td>
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
<td><a href="element-resources.md">Resources</a> </td>
<td><p>Declares languages for the resources that the package contains. Every package must declare at least one language for resources. The scale and DirectX feature level attributes are common for all resources in the package.</p></td>
</tr>
</tbody>
</table>

 

## Requirements

|               |      Value                                                       |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2010/manifest` |

 

 
