---
description: Defines an app extensibility point of type windows.backgroundTasks (Windows 8.1).
Search.Product: eADQiWindows 10XVcnh
title: BackgroundTasks (extensions schema for Windows 8.1)
ms.assetid: 0e9cbbc5-3852-4158-87e7-12ea87be62e7


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# BackgroundTasks (extensions schema for Windows 8.1)




Defines an app extensibility point of type **windows.backgroundTasks**. Background tasks run in a dedicated background host; that is, without a UI.

## Element hierarchy

<dl>
<dt><a href="element-extension.md">&lt;Extension&gt;</a></dt>
<dd><b>&lt;BackgroundTasks&gt;</b></dd>
</dl>

## Syntax

``` syntax
<BackgroundTasks ServerName? = A string between 1 and 255 characters in length. >

  <!-- Child elements -->
  TaskChoice{1,8}

</BackgroundTasks>
```

### Key

`?`   optional (zero or one)
`{}`   specific range of occurrences
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
<td><strong>ServerName</strong></td>
<td><p>The server name. Ensures that only one instance of the server exists at runtime.</p></td>
<td>A string between 1 and 255 characters in length.</td>
<td>No</td>
<td></td>
</tr>
</tbody>
</table>

 

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
<td><a href="element-taskchoice.md">TaskChoice</a> </td>
<td><p>The abstract task choice element for the XSD substitution group. This can't be declared in the XML.</p></td>
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
<td><a href="element-extension.md">Extension (type: CT_ApplicationExtension)</a> </td>
<td><p>Declares an extensibility point for the app.</p></td>
</tr>
</tbody>
</table>

 

## Remarks

Extensions of type "windows.backgroundTask" must specify either a StartPage or EntryPoint attribute in the Extension element. For more info (and an example) see [**How to declare background tasks in the application manifest (JavaScript and HTML)**](/previous-versions/windows/apps/hh977042(v=win.10)) or [**How to declare background tasks in the application manifest (C#/VB/C++ and XAML)**](/previous-versions/windows/apps/hh977049(v=win.10)).

## Requirements

|               |    Value                                                         |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2010/manifest` |

 

 
