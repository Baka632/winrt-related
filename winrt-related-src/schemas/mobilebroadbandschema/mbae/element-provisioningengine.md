---
description: Defines the trusted certificate values for Subject Name and Issuer Name required for provisioning on the mobile network.
Search.Product: eADQiWindows 10XVcnh
title: ProvisioningEngine
ms.assetid: 5ed0a32d-3a5b-4834-929a-d7b9ee3f1371

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# ProvisioningEngine


Defines the trusted certificate values for Subject Name and Issuer Name required for provisioning on the mobile network.

## Element hierarchy

<dl>
<dt><a href="element-mobilebroadbandinfo.md">&lt;MobileBroadbandInfo&gt;</a></dt>
<dd><b>&lt;ProvisioningEngine&gt;</b></dd>
</dl>

## Syntax

``` syntax
<ProvisioningEngine>

  <!-- Child elements -->
  TrustedCertificates?,
  any element in a non-schema namespace*

</ProvisioningEngine>
```

### Key

`?`   optional (zero or one)
`*`   optional (zero or more)

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
<td><a href="element-trustedcertificates.md">TrustedCertificates</a> </td>
<td><p>Defines the list of trusted security certificates required for provisioning on the mobile network.</p></td>
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
<td><a href="element-mobilebroadbandinfo.md">MobileBroadbandInfo</a> </td>
<td><p>Defines mobile broadband information required for provisioning on the mobile network.</p></td>
</tr>
</tbody>
</table>

 

## See also


[**MobileBroadbandInfo**](element-mobilebroadbandinfo.md)

[MBAE schema](schema-root.md)

## Requirements

|          |         |
|----------|--------------|
| **Namespace** | `http://schemas.microsoft.com/windows/2010/12/DeviceMetadata/MobileBroadbandInfo` |

 

 



