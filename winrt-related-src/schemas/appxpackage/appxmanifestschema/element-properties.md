---
description: Defines additional metadata about the package including attributes that describe how the package appears to users.
Search.Product: eADQiWindows 10XVcnh
title: Properties
ms.assetid: accc712c-c7b9-45e1-ba02-836abacbd9b5

keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# Properties


Defines additional metadata about the package including attributes that describe how the package appears to users.

**Note**  You may get an error if the manifest elements DisplayName or Description contain characters disallowed by the Windows firewall; namely “|” and “all”, due to which Windows fails to create the AppContainer profile for the package . Use this reference for [troubleshooting](/windows/win32/appxpkg/troubleshooting) if you get an error.

 

## Element hierarchy

<dl>
<dt><a href="element-package.md">&lt;Package&gt;</a></dt>
<dd><b>&lt;Properties&gt;</b></dd>
</dl>

## Syntax

``` syntax
<Properties>

  <!-- Child elements -->
  ( Framework?
  & DisplayName
  & PublisherDisplayName
  & Description?
  & Logo
  )

</Properties>
```

### Key

`?`   optional (zero or one)

`&`   interleave connector (may occur in any order)

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
<td><a href="element-description.md">Description</a> </td>
<td><p>A friendly description that can be displayed to users.</p></td>
</tr>
<tr class="even">
<td><a href="element-displayname.md">DisplayName</a> </td>
<td><p>A friendly name that can be displayed to users.</p></td>
</tr>
<tr class="odd">
<td><a href="element-framework.md">Framework</a> </td>
<td><p>Indicates whether the package is a framework package; that is, a package that can be used by other packages. Its value is <strong>false</strong> by default. You should not specify a value for it unless you are creating a framework.</p></td>
</tr>
<tr class="even">
<td><a href="element-logo.md">Logo</a> </td>
<td><p>A path to a file that contains an image.</p></td>
</tr>
<tr class="odd">
<td><a href="element-publisherdisplayname.md">PublisherDisplayName</a> </td>
<td><p>A friendly name for the publisher that can be displayed to users.</p></td>
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
<td><a href="element-package.md">Package</a> </td>
<td><p>Defines the root element of an app package manifest. The manifest describes the structure and capabilities of the software to the system.</p></td>
</tr>
</tbody>
</table>

 

## Examples

The following example is taken from the package manifest of one of the SDK samples.

```XML
<Properties>
    <DisplayName>ApplicationData SDK Sample</DisplayName>
    <PublisherDisplayName>Microsoft Corporation</PublisherDisplayName>
    <Description>The application data sample.</Description>
    <Logo>images\storeLogo-sdk.png</Logo>
</Properties>
```

## See also

[Upload app packages](/windows/uwp/publish/upload-app-packages)

[Create your app by reserving a name](/windows/uwp/publish/create-your-app-by-reserving-a-name)

## Requirements

|               |                                                             |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2010/manifest` |

 

 
