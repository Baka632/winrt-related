---
description: Specifies which pages in the web context have access to the system's geolocation devices and access to the clipboard.
Search.Product: eADQiWindows 10XVcnh
title: ApplicationContentUriRules (extensions schema for Windows 8.1)
ms.assetid: 8bb7c378-6461-4c01-b02f-b7f17c32daaa


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# ApplicationContentUriRules (extensions schema for Windows 8.1)




Specifies which pages in the web context have access to the system's geolocation devices (if the app has permission to access this capability) and access to the clipboard.

## Element hierarchy

<dl>
<dt><a href="element-package.md">&lt;Package&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-applications.md">&lt;Applications&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-application.md">&lt;Application&gt;</a></dt>
<dd><b>&lt;ApplicationContentUriRules&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<ApplicationContentUriRules>

  <!-- Child elements -->
  Rule{1,100}

</ApplicationContentUriRules>
```

### Key

`{}`   specific range of occurrences
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
<td><a href="element-rule.md">Rule</a> </td>
<td><p>Specifies which pages in the web context have access to the system's geolocation devices (if the app has permission to access this capability) and access to the clipboard.</p></td>
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
<td><a href="element-application.md">Application</a> </td>
<td><p>Represents an app that comprises part of or all of the functionality delivered in the package.</p></td>
</tr>
</tbody>
</table>

 

## Requirements

|               |     Value                                                        |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2010/manifest` |

 

 



