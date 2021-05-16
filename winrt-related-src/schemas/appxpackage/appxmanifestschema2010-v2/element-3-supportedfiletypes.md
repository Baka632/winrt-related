---
description: Defines the file types that the app can share.
Search.Product: eADQiWindows 10XVcnh
title: 'SupportedFileTypes (Windows 8.1 extensions schema, child of FileSavePicker)'
ms.assetid: fd3072eb-572d-4855-8a9c-3de1599b5a00


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# SupportedFileTypes (extensions schema for Windows 8.1, child of FileSavePicker)




Defines the file types that the app can share.

## Element hierarchy

<dl>
<dt><a href="element-extension.md">&lt;Extension&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-sharetarget.md">&lt;ShareTarget&gt;</a></dt>
<dd><b>&lt;SupportedFileTypes&gt;</b></dd>
</dl>
<dl>
<dt><a href="element-fileopenpicker.md">&lt;FileOpenPicker&gt;</a></dt>
<dd><b>&lt;SupportedFileTypes&gt;</b></dd>
</dl>
<dl>
<dt><a href="element-filesavepicker.md">&lt;FileSavePicker&gt;</a></dt>
<dd><b>&lt;SupportedFileTypes&gt;</b></dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<SupportedFileTypes>

  <!-- Child elements -->
  ( FileType{1,10000}
  | SupportsAnyFileType
  )

</SupportedFileTypes>
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
<td><a href="element-3-filetype.md">FileType (type: ST_FileType)</a> </td>
<td><p>A file type specified as its file type extension. It is unique per application in the package and is case sensitive.</p></td>
</tr>
<tr class="even">
<td><a href="element-2-supportsanyfiletype.md">SupportsAnyFileType</a> </td>
<td><p>Indicates whether all file types are supported for sharing.</p></td>
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
<td><a href="element-fileopenpicker.md">FileOpenPicker</a> </td>
<td><p>Declares an app extensibility point of type <strong>windows.fileOpenPicker</strong>. The app lets the user choose and open the specified types of files.</p></td>
</tr>
<tr class="even">
<td><a href="element-filesavepicker.md">FileSavePicker</a> </td>
<td><p>Declares an app extensibility point of type <strong>windows.fileSavePicker</strong>. The app lets the user choose the file name, extension, and storage location for the specified types of files.</p></td>
</tr>
<tr class="odd">
<td><a href="element-sharetarget.md">ShareTarget</a> </td>
<td><p>Declares an app extension point of type <strong>windows.shareTarget</strong>. The app can share the specified types of files.</p></td>
</tr>
</tbody>
</table>

 

## Related elements


The following elements have the same name as this one, but different content or attributes:

-   **[SupportedFileTypes (type: CT_FTASupportedFileTypes)](element-supportedfiletypes.md)**

## Requirements

|               |     Value                                                        |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2010/manifest` |

 

 



