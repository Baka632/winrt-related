---
description: Declares a device capability required by a package.
Search.Product: eADQiWindows 10XVcnh
title: DeviceCapability (Windows 8.1 feature extensions schema)
ms.assetid: 4353c4fd-f038-4986-81ed-d2ec0c6235ef


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# DeviceCapability (feature extensions schema for Windows 8.1)




Declares a device capability required by a package.

## Element hierarchy

**&lt;DeviceCapability&gt;**

## Syntax

``` syntax
<DeviceCapability Name = A string between 1 and 50 characters in length or a GUID in the form xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx. >

  <!-- Child elements -->
  Device{1,100}

</DeviceCapability>
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
<td><strong>Name</strong></td>
<td><p>The name of the device capability, either specified as a friendly name or a device interface class GUID.</p></td>
<td>A string between 1 and 50 characters in length or a GUID in the form xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx.</td>
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
<td><a href="element-device.md">Device</a> </td>
<td><p>Declares a function for a device that is associated with the <a href="element-devicecapability.md"><strong>DeviceCapability</strong></a> .</p></td>
</tr>
</tbody>
</table>

 

### Parent Elements

This outermost (document) element may not be contained by any other elements.

## Remarks

This table lists device capabilities by name that are supported starting with the app package manifest for Windows 8.1 apps.

| Device capability | Description                                                                          |
|-------------------|--------------------------------------------------------------------------------------|
| **appointments**  | Provides access to the user's appointment store.                                     |
| **contacts**      | Provides access to the aggregated view of the contacts from various contacts stores. |

 

For info about device capabilities that are supported starting with the app package manifest for Windows 8 UWP apps, see [**DeviceCapability**](../appxmanifestschema2010-v2/element-devicecapability.md).

For more info about capability declarations, see [App capability declarations](/previous-versions/windows/apps/hh464936(v=win.10)).

## Requirements

|               |     Value                                                        |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2013/manifest` |

 

 
