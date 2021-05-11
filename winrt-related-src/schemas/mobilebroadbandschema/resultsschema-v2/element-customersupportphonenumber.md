---
description: Contains any errors from processing the CustomerSupportPhoneNumber element from the last provisioning attempt.
Search.Product: eADQiWindows 10XVcnh
title: CustomerSupportPhoneNumber (ResultsSchema_v2 schema)
ms.assetid: a5fefff4-22ce-4219-be12-4db9520cfa47

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# CustomerSupportPhoneNumber (ResultsSchema_v2 schema)


Contains any errors from processing the [**CustomerSupportPhoneNumber**](../carriercontrolschema-v2/element-customersupportphonenumber.md) element from the last provisioning attempt.

## Element hierarchy

<dl>
<dt><a href="element-carrierprovisioningresult.md">&lt;CarrierProvisioningResult&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-carriernetworkmetadata.md">&lt;CarrierNetworkMetadata&gt;</a></dt>
<dd><b>&lt;CustomerSupportPhoneNumber&gt;</b></dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<CustomerSupportPhoneNumber errorCode = token />
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
<td><a href="element-carriernetworkmetadata.md">CarrierNetworkMetadata</a> </td>
<td><p>Contains any errors from processing the <a href="/uwp/schemas/mobilebroadbandschema/carriercontrolschema-v2/element-carriernetworkmetadata"><strong>CarrierNetworkMetadata</strong></a>  element from the last provisioning attempt.</p></td>
</tr>
</tbody>
</table>

 

## Requirements

|          | Value        |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControlResults/v2` |

 

 
