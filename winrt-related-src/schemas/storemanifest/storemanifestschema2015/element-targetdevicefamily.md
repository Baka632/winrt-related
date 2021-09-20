---
description: Identifies the device family that your package targets (in StoreManifest/Dependencies).
Search.Product: eADQiWindows 10XVcnh
title: TargetDeviceFamily
ms.assetid: 457745aa-bc12-427b-b1f1-74c1618753c0


keywords: windows 10, uwp, schema, storemanifest


ms.topic: reference
ms.date: 04/05/2017
---

# TargetDeviceFamily


Identifies the device family that your package targets.

**Important**  In most cases, you should simply specify your device families in the [**TargetDeviceFamily**](../../appxpackage/uapmanifestschema/element-targetdevicefamily.md) element of your AppxManifest. Values here should only be used if you need to override that info (using a subset of the values provided there).

 

## Element hierarchy

<dl>
<dt><a href="element-storemanifest.md">&lt;StoreManifest&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-dependencies.md">&lt;Dependencies&gt;</a></dt>
<dd><b>&lt;TargetDeviceFamily&gt;</b></dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<TargetDeviceFamily Name       = An alphanumeric string. May contain period and dash characters.
                    MinVersion = A version string in quad notation, "Major.Minor.Build.Revision". />
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
<td><strong>MinVersion</strong></td>
<td><p>The minimum version of the device family that your app is targeting. Used for applicability at deployment time. If the device family version of the system is lower than MinVersion, then the package is not considered applicable.</p></td>
<td>A version string in quad notation, &quot;Major.Minor.Build.Revision&quot;.</td>
<td>Yes</td>
<td></td>
</tr>
<tr class="even">
<td><strong>Name</strong></td>
<td><p>The name of the device family that your app is targeting.</p></td>
<td>An alphanumeric string. May contain period and dash characters.</td>
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
<td><a href="element-dependencies.md">Dependencies</a> </td>
<td><p>Declares requirements that a package depends on to be applicable to a device.</p></td>
</tr>
</tbody>
</table>

 

## Remarks

For more info about device families, see [Guide to Universal Windows Platform (UWP) apps](/windows/uwp/get-started/universal-application-platform-guide).

## Requirements

|          | Value |
|----------|--------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2015/StoreManifest` |

 

 
