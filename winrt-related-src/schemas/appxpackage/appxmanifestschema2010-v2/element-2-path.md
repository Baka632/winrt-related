---
description: The path to the DLL.
Search.Product: eADQiWindows 10XVcnh
title: 'Path (Windows 8.1 extensions schema, child of ProxyStub)'
ms.assetid: 4522dd59-287a-4c40-8054-168d06f61a08


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# Path (extensions schema for Windows 8.1, child of ProxyStub)




The path to the DLL.

## Element hierarchy

<dl>
<dt><a href="element-package.md">&lt;Package&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-extensions.md">&lt;Extensions&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-1-extension.md">&lt;Extension&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-inprocessserver.md">&lt;InProcessServer&gt;</a></dt>
<dd><b>&lt;Path&gt;</b></dd>
</dl>
<dl>
<dt><a href="element-proxystub.md">&lt;ProxyStub&gt;</a></dt>
<dd><b>&lt;Path&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<Path>

  A string between 1 and 256 characters in length that cannot contain these characters: <, >, :, ", |, ?, or *.

</Path>
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
<td><a href="element-inprocessserver.md">InProcessServer</a> </td>
<td><p>Declares a package extensibility point of type <strong>windows.activatableClass.inProcessServer</strong>. The app uses a dynamic link library (DLL) that exposes one or more activatable classes.</p></td>
</tr>
<tr class="even">
<td><a href="element-proxystub.md">ProxyStub</a> </td>
<td><p>Declares a package extensibility point of type <strong>windows.activatableClass.proxyStub</strong>. A proxy can be composed of one or more interfaces.</p></td>
</tr>
</tbody>
</table>

 

## Related elements


The following elements have the same name as this one, but different content or attributes:

-   **[Path (type: ST_Executable)](element-1-path.md)**

## Requirements

|               |   Value                                                          |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2010/manifest` |

 

 



