---
description: Declares a package extension point of type windows.activatableClass.outOfProcessServer.
Search.Product: eADQiWindows 10XVcnh
title: OutOfProcessServer (Windows 8 package schema)
ms.assetid: 575ad44f-e0e3-4682-a082-8d8184bd8dd4


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# OutOfProcessServer (package schema for Windows 8)


Declares a package extension point of type **windows.activatableClass.outOfProcessServer**. The app uses an executable (EXE) that exposes one or more activatable classes.

## Element hierarchy

<dl>
<dt><a href="element-package.md">&lt;Package&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-extensions.md">&lt;Extensions&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-extension.md">&lt;Extension&gt;</a></dt>
<dd><b>&lt;OutOfProcessServer&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<OutOfProcessServer ServerName = A string between 1 and 255 characters in length. >

  <!-- Child elements -->
  Path,
  Arguments?,
  Instancing,
  ActivatableClass{1,65535}

</OutOfProcessServer>
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
<td><p>The name of the executable.</p></td>
<td>A string between 1 and 255 characters in length.</td>
<td>Yes</td>
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
<td><a href="element-1-activatableclass.md">ActivatableClass (type: CT_OutOfProcessActivatableClass)</a> </td>
<td><p>Declares a runtime class associated with the extensibility point.</p></td>
</tr>
<tr class="even">
<td><a href="element-arguments.md">Arguments</a> </td>
<td><p>Specifies the list of comma-separated arguments to pass to the executable.</p></td>
</tr>
<tr class="odd">
<td><a href="element-instancing.md">Instancing</a> </td>
<td><p>Specifies whether the executable runs as a single instance or can run as multiple instances.</p></td>
</tr>
<tr class="even">
<td><a href="element-1-path.md">Path (type: ST_Executable)</a> </td>
<td><p>The path to the executable.</p></td>
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
<td><a href="element-extension.md">Extension (in type: CT_PackageExtensions)</a> </td>
<td><p>Declares an extensibility point for the package.</p></td>
</tr>
</tbody>
</table>

 

## Examples

```XML
<Extension Category="windows.activatableClass.outOfProcessServer">
      <OutOfProcessServer ServerName="Microsoft.SDKSamples.ToastServer">
        <Path>Microsoft.Samples.ExeServerAuthoring.exe</Path>
        <Instancing>singleInstance</Instancing>
        <ActivatableClass ActivatableClassId="Microsoft.Samples.ExeServerAuthoring.Toaster" />
      </OutOfProcessServer>
</Extension>
```

## Requirements

|               |    Value                                                         |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2010/manifest` |

 

 



