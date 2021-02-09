---
description: Defines the subject name of the trusted certificate.
Search.Product: eADQiWindows 10XVcnh
title: SubjectName
ms.assetid: 63be4106-a116-40b7-9645-fcced74a01ac

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# SubjectName


Defines the subject name of the trusted certificate.

## Element hierarchy

<dl>
<dt><a href="element-mobilebroadbandinfo.md">&lt;MobileBroadbandInfo&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-provisioningengine.md">&lt;ProvisioningEngine&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-trustedcertificates.md">&lt;TrustedCertificates&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-trustedcertificate.md">&lt;TrustedCertificate&gt;</a></dt>
<dd><b>&lt;SubjectName&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<SubjectName>

  string

</SubjectName>
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
<td><a href="element-trustedcertificate.md">TrustedCertificate</a> </td>
<td><p>Defines the subject name and issuer name of a trusted certificate required for provisioning on the mobile network.</p></td>
</tr>
</tbody>
</table>

 

## See also


[MBAE schema](schema-root.md)

[**MobileBroadbandInfo**](element-mobilebroadbandinfo.md)

[**ProvisioningEngine**](element-provisioningengine.md)

[**TrustedCertificate**](element-trustedcertificate.md)

[**TrustedCertificates**](element-trustedcertificates.md)

## Requirements

|          |         |
|----------|--------------|
| **Namespace** | `http://schemas.microsoft.com/windows/2010/12/DeviceMetadata/MobileBroadbandInfo` |

 

 



