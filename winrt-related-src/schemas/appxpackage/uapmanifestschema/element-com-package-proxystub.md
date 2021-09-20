---

ms.assetid: 04c01463-ed54-428c-b26a-0fc36310eb67
title: com:ProxyStub (in Package/Extensions)
description: Registers a proxy stub (in Package/Extensions).

ms.date: 03/29/2017
ms.topic: reference


keywords: windows 10, uwp, schema, manifest, com
---


# com:ProxyStub (in Package/Extensions)

## Description
Registers a proxy stub.

## Element Hierarchy
<dl>
<dt><a href="element-package.md">&lt;Package&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-extensions.md">&lt;Extensions&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-extension.md">&lt;Extension&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-com-package-cominterface.md">&lt;ComInterface&gt;</a></dt>
<dd><b>&lt;ProxyStub&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
</dl>



## Syntax
```syntax
<ProxyStub
    Id = A GUID in the form xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx.
    DisplayName? = A string between 1 and 256 characters in length. This string is localizable.
    Path = A string between 1 and 256 characters in length that cannot contain these characters: <, >, :, ", |, ?, or *. >

    <!-- Child elements -->
    com2:ProxyStubDll

</ProxyStub>
```

## Key
`?`    optional (zero or one)  

## Attributes

| Attribute | Description | Data type | Required |
|-----------|-------------|-----------|----------|
| Id | The proxy stub's CLSID. | A GUID in the form xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx. | Yes |
| DisplayName | A localizable string corresponding to the default value of the proxy stub's CLSID key. | A string between 1 and 256 characters in length. This string is localizable. | No |
| Path | The path relative to the package root. Path must reference a file in the package. | A string between 1 and 256 characters in length that cannot contain these characters: <, >, :, ", &#124;, ?, or *. | Yes |

## Child Elements

| Child Element | Description |
|---------------|-------------|
| [com2:ProxyStubDll](element-com2-package-proxystubdll.md) | Specifies the path and processor architecture of a ProxyStub DLL. |

## Remarks
Proxy stub registrations correspond to the CLSID registration for the Interface's [ProxyStubClsid32](/windows/win32/com/proxystubclsid32) keys.

A proxy stub element must have either a Path attribute or one or more ProxyStubDll child elements, but not both.

## Examples

## Requirements
|               |     Value                                                        |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/manifest/com/windows10` |