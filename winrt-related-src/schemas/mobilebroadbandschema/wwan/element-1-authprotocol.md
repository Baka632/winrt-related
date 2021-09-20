---
description: Defines the authentication protocol to be used for activating a Packet Data Protocol (PDP) context (in PurchaseProfile/Context).
Search.Product: eADQiWindows 10XVcnh
title: AuthProtocol (descendant of PurchaseProfile)
ms.assetid: 24272c9d-966a-4f02-a64b-6e7116131ba7

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# AuthProtocol (descendant of PurchaseProfile)


Defines the authentication protocol to be used for activating a Packet Data Protocol (PDP) context:

-   **NONE** - No authentication protocol.
-   **PAP** - Unencrypted password authentication.
-   **CHAP** - Challenge Handshake Authentication Protocol(CHAP).
-   **MsCHAPv2** - Microsoft’s Challenge Handshake Authentication Protocol(CHAP) v2.0.

## Element hierarchy

<dl>
<dt><a href="element-purchaseprofile.md">&lt;PurchaseProfile&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-1-context.md">&lt;Context&gt;</a></dt>
<dd><b>&lt;AuthProtocol&gt;</b></dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<AuthProtocol>

  "NONE" | "PAP" | "CHAP" | "MsCHAPv2"

</AuthProtocol>
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
<td><a href="element-1-context.md">Context</a> </td>
<td><p>Defines the parameters required to setup a data connection.</p></td>
</tr>
</tbody>
</table>

 

## Requirements

|          | Value |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControl/WWAN/v1` |

 

 



