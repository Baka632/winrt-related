---
Description: Defines the context of a Packet Data Protocol (PDP) context policy in a subscriber's carrier provisioning file.
Search.Product: eADQiWindows 10XVcnh
title: Context
ms.assetid: ddf2b145-59b3-46bf-a297-6992f00a06e0

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# Context


Defines the context of a Packet Data Protocol (PDP) context policy in a subscriber's carrier provisioning file.

## Element hierarchy

<dl>
<dt><a href="element-extensions-v2.md">&lt;Extensions_v2&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-additionalpdpcontexts.md">&lt;AdditionalPDPContexts&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-multiplepdpcontextpolicies.md">&lt;MultiplePDPContextPolicies&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-pdpcontextpolicy.md">&lt;PDPContextPolicy&gt;</a></dt>
<dd><b>&lt;Context&gt;</b></dd>
</dl>
</dd>
</dl>
<dl>
<dt><a href="element-tetheringsettings.md">&lt;TetheringSettings&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-tetheringprofile.md">&lt;TetheringProfile&gt;</a></dt>
<dd><b>&lt;Context&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<Context>

  <!-- Child elements -->
  AccessString?,
  UserLogonCred?,
  Compression?,
  AuthProtocol?

</Context>
```

### Key

`?`   optional (zero or one)

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
<td><a href="element-accessstring.md">AccessString</a> </td>
<td><p>Defines the access string for a context in the Packet Data Protocol (PDP) context policy.</p></td>
</tr>
<tr class="even">
<td><a href="element-authprotocol.md">AuthProtocol</a> </td>
<td><p>Defines the authentication protocol to use for a context in the Packet Data Protocol (PDP) context policy.</p></td>
</tr>
<tr class="odd">
<td><a href="element-compression.md">Compression</a> </td>
<td><p>Defines whether compression is enabled for a context in the Packet Data Protocol (PDP) context policy.</p></td>
</tr>
<tr class="even">
<td><a href="element-userlogoncred.md">UserLogonCred</a> </td>
<td><p>Defines the user login credentials for a context in the Packet Data Protocol (PDP) context policy.</p></td>
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
<td><a href="element-pdpcontextpolicy.md">PDPContextPolicy</a> </td>
<td><p>Defines a Packet Data Protocol (PDP) context policy in a subscriber's carrier provisioning file.</p></td>
</tr>
<tr class="even">
<td><a href="element-tetheringprofile.md">TetheringProfile</a> </td>
<td><p>Defines the tethering profile in a subscriber's carrier provisioning file.</p></td>
</tr>
</tbody>
</table>

 

## See also


[**AdditionalPDPContexts**](element-additionalpdpcontexts.md)

[CarrierControlSchema schema](../carriercontrolschema/schema-root.md)

[CarrierControlSchema\_v2 schema](schema-root.md)

[**MultiplePDPContextPolicies**](element-multiplepdpcontextpolicies.md)

[**PDPContextPolicy**](element-pdpcontextpolicy.md)

## Requirements

|          |         |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControl/v2` |

 

 