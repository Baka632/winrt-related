---
description: Declares a function for a device that is associated with the DeviceCapability (in DeviceCapability/Device).
Search.Product: eADQiWindows 10XVcnh
title: Device
ms.assetid: 1e9e699f-bbd9-4d15-95ea-207ec495c46e


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# Device




Declares a function for a device that is associated with the [**DeviceCapability**](element-devicecapability.md).

## Element hierarchy

<dl>
<dt><a href="element-devicecapability.md">&lt;DeviceCapability&gt;</a></dt>
<dd><b>&lt;Device&gt;</b></dd>
</dl>

## Syntax

``` syntax
<Device Id = A string between 1 and 512 characters in length. >

  <!-- Child elements -->
  Function{1,100}

</Device>
```

### Key

`{}`   specific range of occurrences
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
<td><p>The identifier of the device.</p></td>
<td>A string between 1 and 512 characters in length.</td>
<td>Yes</td>
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
<td><a href="element-function.md">Function</a> </td>
<td><p>Declares the function for the device.</p></td>
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
<td><a href="element-devicecapability.md">DeviceCapability</a> </td>
<td><p>Declares a device capability required by a package.</p></td>
</tr>
</tbody>
</table>

 

## Requirements

|               |        Value                                                     |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2013/manifest` |

 

 



