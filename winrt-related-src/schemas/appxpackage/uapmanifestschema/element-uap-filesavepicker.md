---
description: Declares an app extensibility point of type windows.fileSavePicker.
Search.Product: eADQiWindows 10XVcnh
title: uap:FileSavePicker (Windows 10)
ms.assetid: 9b6f7fef-57c0-46ba-9b17-417e907d4084


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# uap:FileSavePicker (Windows 10)


Declares an app extensibility point of type **windows.fileSavePicker**. The app lets the user choose the file name, extension, and storage location for the specified types of files.

## Element hierarchy

<dl>
<dt><a href="element-package.md">&lt;Package&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-applications.md">&lt;Applications&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-application.md">&lt;Application&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-1-extensions.md">&lt;Extensions&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-uap-extension.md">&lt;uap:Extension&gt;</a></dt>
<dd><b>&lt;uap:FileSavePicker&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<FileSavePicker>

  <!-- Child elements -->
  uap:SupportedFileTypes

</uap:FileSavePicker>
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
<td><a href="element-3-uap-supportedfiletypes.md">uap:SupportedFileTypes (type: CT_CharmsSupportedFileTypes)</a> </td>
<td><p>Defines the file types that the app can share.</p></td>
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
<td><a href="element-uap-extension.md">uap:Extension</a> </td>
<td><p>Declares an extensibility point for the app.</p></td>
</tr>
</tbody>
</table>

 

## See also


**Tasks**
[Accessing files with file pickers](/previous-versions/windows/apps/hh465174(v=win.10))

**Concepts**
[App contracts and extensions](/previous-versions/windows/apps/hh464906(v=win.10))

## Requirements

|   | Value |
|--|--|
| **Namespace** | `http://schemas.microsoft.com/appx/manifest/uap/windows10` |


 

 
