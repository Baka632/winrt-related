---
description: Provides details for each element, attribute, and data type that defines the schema for the bundle manifest for UWP apps.
Search.Product: eADQiWindows 10XVcnh
title: Bundle manifest schema reference
ms.assetid: 20fba0dd-b7d6-47c8-9d9f-a8831bda627c

keywords: windows 10, uwp, schema, bundle manifest


ms.topic: reference
ms.date: 04/05/2017
---

# Bundle manifest schema reference


This reference provides details for each element, attribute, and data type that defines the schema for the bundle manifest for UWP apps. The schema definition file is BundleManifestSchema.xsd.

The following table lists all of the elements in this schema, sorted alphabetically by name.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><a href="element-bundle.md">Bundle</a> </td>
<td><p>Defines the root element of a bundle manifest. The manifest describes the structure and capabilities of the software to the system.</p></td>
</tr>
<tr class="even">
<td><a href="element-identity.md">Identity</a> </td>
<td><p>Defines a globally unique identifier for a bundle. A bundle identity is represented as a tuple of attributes of the bundle.</p></td>
</tr>
<tr class="odd">
<td><a href="element-package.md">Package</a> </td>
<td><p>Defines one of the app packages or resource packages in the bundle.</p></td>
</tr>
<tr class="even">
<td><a href="element-packages.md">Packages</a> </td>
<td><p>Defines the app packages and resource packages that are contained in the bundle.</p></td>
</tr>
<tr class="odd">
<td><a href="element-resource.md">Resource</a> </td>
<td><p>Declares language, resolution scale, and DirectX feature level for a resource in the package.</p></td>
</tr>
<tr class="even">
<td><a href="element-resources.md">Resources</a> </td>
<td><p>Declares languages, resolution scales, and DirectX feature levels for the resources that the package contains.</p></td>
</tr>
<tr class="even">
<td><a href="element-dependencies.md">Dependencies</a> </td>
<td><p>Declares dependencies that will be installed if required.</p></td>
</tr>
</tbody>
</table>

 

 

 



