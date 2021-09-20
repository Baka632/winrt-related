---
description: Describes whether Windows overlays the app’s name on top of the tile image that is shown on the Start screen (in VisualElements/DefaultTile).
Search.Product: eADQiWindows 10XVcnh
title: ShowOn
ms.assetid: bccecb2d-23f6-47ac-ae19-7969fb88cd3d


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# ShowOn

Describes whether Windows overlays the app’s name on top of the tile image that is shown on the Start screen.

## Element hierarchy

<dl>
<dt><a href="element-visualelements.md">&lt;VisualElements&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-defaulttile.md">&lt;DefaultTile&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-shownameontiles.md">&lt;ShowNameOnTiles&gt;</a></dt>
<dd><b>&lt;ShowOn&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<ShowOn Tile = "square150x150Logo" | "wide310x150Logo" | "square310x310Logo" />
```

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
<td><strong>Tile</strong></td>
<td><p>The tile size.</p></td>
<td><p>This attribute can have one of the following values:</p>
<ul>
<li>square150x150Logo</li>
<li>wide310x150Logo</li>
<li>square310x310Logo</li>
</ul></td>
<td>Yes</td>
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
<td><a href="element-shownameontiles.md">ShowNameOnTiles</a> </td>
<td><p>Describes whether Windows overlays the app’s name on top of the tile images that are shown on the Start screen.</p></td>
</tr>
</tbody>
</table>

 

## Remarks

This example shows how to use **ShowOn**:

``` syntax
            <m2:ShowOn Tile="wide310x150Logo"/> // Show app name on 310x150 Logo
```

## Requirements

|               |    Value                                                         |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2013/manifest` |

 

 



