---
description: Defines the network settings for DNS retries in a subscriber's carrier provisioning file.
Search.Product: eADQiWindows 10XVcnh
title: DNSRetrySettings
ms.assetid: 2749204f-5d80-4b44-9c65-b0d62931e269

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# DNSRetrySettings


Defines the network settings for DNS retries in a subscriber's carrier provisioning file.

## Element hierarchy

<dl>
<dt><a href="element-extensions-v2.md">&lt;Extensions_v2&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-carriernetworkmetadata.md">&lt;CarrierNetworkMetadata&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-networksettings.md">&lt;NetworkSettings&gt;</a></dt>
<dd><b>&lt;DNSRetrySettings&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<DNSRetrySettings>

  <!-- Child elements -->
  DNSRetryIntervalInSeconds,
  DNSRetryCount

</DNSRetrySettings>
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
<td><a href="element-dnsretrycount.md">DNSRetryCount</a> </td>
<td><p>Defines the DNS retry count. It must be a positive integer between 1 and 4.</p></td>
</tr>
<tr class="even">
<td><a href="element-dnsretryintervalinseconds.md">DNSRetryIntervalInSeconds</a> </td>
<td><p>Defines the DNS retry interval in seconds. It must be a positive integer between 1 and 4.</p></td>
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
<td><a href="element-networksettings.md">NetworkSettings</a> </td>
<td><p>Defines the network settings in a subscriber's carrier provisioning file.</p></td>
</tr>
</tbody>
</table>

 

## See also


[CarrierControlSchema schema](../carriercontrolschema/schema-root.md)

[CarrierControlSchema\_v2 schema](schema-root.md)

[**NetworkSettings**](element-networksettings.md)

## Requirements

|          |         |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControl/v2` |

 

 
