---
description: Defines values that describe the subscriber's plan and data usage.
Search.Product: eADQiWindows 10XVcnh
title: Fields
ms.assetid: 18121e44-cd14-44f5-b36b-dc5d9fe3603c

keywords: windows 10, uwp, schema, mobile broadband schema


ms.topic: reference
ms.date: 04/05/2017
---

# Fields


Defines values that describe the subscriber's plan and data usage.

## Element hierarchy

<dl>
<dt><a href="element-messages.md">&lt;Messages&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-message.md">&lt;Message&gt;</a></dt>
<dd><b>&lt;Fields&gt;</b></dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<Fields>

  <!-- Child elements -->
  ( Usage
  | UsagePercentage
  | UsageOverage
  | UsageOveragePercentage
  | UsageTimestamp
  )?,
  DataLimit?,
  OverDataLimit?,
  Congested?,
  InboundBandwidth?,
  OutboundBandwidth?,
  PlanType?,
  RefreshProvisioning?,
  ActivationComplete?

</Fields>
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
<td><a href="element-activationcomplete.md">ActivationComplete</a> </td>
<td><p>If <strong>true</strong>, the subscription has been activated, and the machine should immediately attempt to connect. Otherwise, <strong>false</strong>.</p></td>
</tr>
<tr class="even">
<td><a href="element-congested.md">Congested</a> </td>
<td><p>If <strong>true</strong>, the subscriber's connection is in a state of congestion. Otherwise, it is either not supported by the MNO or <strong>false</strong>.</p></td>
</tr>
<tr class="odd">
<td><a href="element-datalimit.md">DataLimit</a> </td>
<td><p>Defines a value representing the data limit in MB for a capped plan. Must be a value from 0 to 2<sup>32nd</sup>.</p></td>
</tr>
<tr class="even">
<td><a href="element-inboundbandwidth.md">InboundBandwidth</a> </td>
<td><p>Defines a value representing the effective link speed of the subscriber’s inbound connection.</p></td>
</tr>
<tr class="odd">
<td><a href="element-outboundbandwidth.md">OutboundBandwidth</a> </td>
<td><p>Defines a value representing the effective link speed of the subscriber’s outbound connection.</p></td>
</tr>
<tr class="even">
<td><a href="element-overdatalimit.md">OverDataLimit</a> </td>
<td><p>Defines whether a subscriber has consumed more bytes than the data limit for their plan.</p></td>
</tr>
<tr class="odd">
<td><a href="element-plantype.md">PlanType</a> </td>
<td><p>Defines the type of plan currently in use by the subscriber.</p></td>
</tr>
<tr class="even">
<td><a href="element-refreshprovisioning.md">RefreshProvisioning</a> </td>
<td><p>If <strong>true</strong>, the network configuration has been updated, and the machine should attempt to retrieve a new provisioning file during the next available maintenance window. Otherwise, <strong>false</strong>.</p></td>
</tr>
<tr class="odd">
<td><a href="element-usage.md">Usage</a> </td>
<td><p>Defines the number of bytes the subscriber has consumed against their data limit. If absent, it is inferred by:</p>
<ul>
<li><strong>UsagePercentage</strong> times <strong>DataLimit</strong></li>
<li><strong>UsagePercentage</strong> times <strong>DataLimit</strong></li>
<li><strong>UsageOverage</strong> plus <strong>DataLimit</strong></li>
<li>(<strong>UsageOveragePercentage</strong> times <strong>DataLimit</strong>) plus <strong>DataLimit</strong></li>
<li><strong>UsageOverage</strong> plus (<strong>UsageOverage</strong> divided by (<strong>UsageOveragePercentage</strong> - 100) )</li>
<li><strong>UsageOverage</strong> plus <strong>DataLimit</strong></li>
</ul></td>
</tr>
<tr class="even">
<td><a href="element-usageoverage.md">UsageOverage</a> </td>
<td><p>Defines the number of bytes the subscriber has consumed over their data limit.</p></td>
</tr>
<tr class="odd">
<td><a href="element-usageoveragepercentage.md">UsageOveragePercentage</a> </td>
<td><p>Defines the percentage over the data limit a subscriber has consumed.</p></td>
</tr>
<tr class="even">
<td><a href="element-usagepercentage.md">UsagePercentage</a> </td>
<td><p>Defines the percentage of the data limit a subscriber has consumed.</p></td>
</tr>
<tr class="odd">
<td><a href="element-usagetimestamp.md">UsageTimestamp</a> </td>
<td><p>Defines a validity date and time of the usage information.</p></td>
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
<td><a href="element-message.md">Message</a> </td>
<td><p>Defines a MNO formatted message that contains the parsing rules necessary for Windows 8 to parse the message.</p></td>
</tr>
</tbody>
</table>

 

## Remarks

Values include rules for inferring the value if absent. If any value referenced in a rule is not specified, skip the rule. If all rules are skipped, no value is set.

## Requirements

|          | Value |
|----------|--------------|
| **Namespace** | `http://www.microsoft.com/networking/CarrierControl/WWAN/v1` |

 

 



