---
description: Contains any errors from processing a TetheringProfile element from the last provisioning attempt.
Search.Product: eADQiWindows 10XVcnh
title: TetheringProfile (ResultsSchema_v2 schema)
ms.assetid: fa2708f2-2200-46ac-b6cd-97d1a51cc867

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# TetheringProfile (ResultsSchema_v2 schema)


Contains any errors from processing a [**TetheringProfile**](../carriercontrolschema-v2/element-tetheringprofile.md) element from the last provisioning attempt.

## Element hierarchy

<dl>
<dt><a href="element-carrierprovisioningresult.md">&lt;CarrierProvisioningResult&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-additionalpdpcontexts.md">&lt;AdditionalPDPContexts&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-tetheringsettings.md">&lt;TetheringSettings&gt;</a></dt>
<dd><b>&lt;TetheringProfile&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<TetheringProfile errorCode = token
                  name      = string />
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
<td><strong>errorCode</strong></td>
<td><p>S_OK if schema processed successfully. Otherwise, the HRESULT returned during the provisioning attempt formatted as eight hexadecimal characters [0-9a-f].</p></td>
<td>token</td>
<td>Yes</td>
<td></td>
</tr>
<tr class="even">
<td><strong>name</strong></td>
<td><p>The name of a Packet Data Protocol (PDP) context policy in a subscriber's carrier provisioning file.</p></td>
<td>string</td>
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
<td><a href="element-tetheringsettings.md">TetheringSettings</a> </td>
<td><p>Contains any errors from processing the <a href="/uwp/schemas/mobilebroadbandschema/carriercontrolschema-v2/element-tetheringsettings"><strong>TetheringSettings</strong></a>  element from the last provisioning attempt.</p></td>
</tr>
</tbody>
</table>

 

## Requirements

|          |         |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControlResults/v2` |

 

 
