---
description: DThe DeviceCompanionApplication element contains all the configuration required to declare your app as a Microsoft Store device app.
Search.Product: eADQiWindows 10XVcnh
title: DeviceCompanionApplication (StoreManifest schema, Windows 8.1 and earlier)
ms.assetid: 302f6805-4684-4061-bb60-c0fcff710758


keywords: windows 10, uwp, schema, storemanifest


ms.topic: reference
ms.date: 04/05/2017
---

# DeviceCompanionApplication (StoreManifest schema for Windows 8.1 and earlier)


The DeviceCompanionApplication element contains all the configuration required to declare your app as a Microsoft Store device app.

## Element hierarchy

<dl>
<dt><a href="element-storemanifest.md">&lt;StoreManifest&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-productfeatures.md">&lt;ProductFeatures&gt;</a></dt>
<dd><b>&lt;DeviceCompanionApplication&gt;</b></dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<DeviceCompanionApplication>

  <!-- Child elements -->
  ExperienceIds

</DeviceCompanionApplication>
```

## Attributes and Elements


### Attributes

None.

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
<td><a href="element-experienceids.md">ExperienceIds</a> </td>
<td><p>The ExperienceIds element contains a list of one or more individual ExperienceId elements.</p></td>
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
<td><a href="element-productfeatures.md">ProductFeatures</a> </td>
<td><p>The ProductFeatures element is the container for all existing and future product features that will be configured through the StoreManifest XML file.</p></td>
</tr>
</tbody>
</table>

 

## Remarks

The term ‘Device Companion App’ has been deprecated. The DeviceCompanionApplication element name continues to exist in this Schema for backwards compatibility.

When present, the DeviceCompanionApplication element must contain an ExperienceIds element, which is described below.

**Important**  Using the DeviceCompanionApplication element in StoreManifest.xml and submitting it with your app will declare your app as a device app in the Microsoft Store. This action cannot be undone in the same product release. If you wish to release this app without the features and constraints that are applied to device apps, you will need to create and submit a new release with an updated StoreManifest.xml file.

 

## Examples

The following is an example of the ProductFeatures element that declares the app as a device app.

```XML
<ProductFeatures>     
    <DeviceCompanionApplication>
        <ExperienceIds>
            <ExperienceId>aeabdaa8-3bcd-4f03-a7f5-54647fd574c2</ExperienceId>
        </ExperienceIds>
    </DeviceCompanionApplication>   
</ProductFeatures>
```

## Requirements

|          | Value |
|----------|--------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2010/StoreManifest` |

 

 



