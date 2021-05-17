---

ms.assetid: ffb76b68-b2c2-424f-8785-10da06294fb7
title: com:ComInterface
description: Declares a package extension point of type windows.comInterface.

ms.date: 03/29/2017
ms.topic: reference


keywords: windows 10, uwp, schema, manifest, com
---

# com:ComInterface

## Description
Declares a package extension point of type **windows.comInterface**. The comInterface extension may include three types of registrations: **Interface**, **ProxyStub**, or **TypeLib**.

## Element Hierarchy
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
<dt><a href="element-com-extension.md">&lt;com:Extension&gt;</a></dt>
<dd><b>&lt;com:ComInterface&gt;</b></dd>
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
```syntax
<ComInterface>
  <!-- Child elements -->
  ( com:ProxyStub{0,1000},
  com:Interface{0,10000},
  com:TypeLib{0,1000}
  )
</ComInterface>
```

## Key
`{}`   specific range of occurrences

## Child Elements

| Child Element | Description |
|---------------|-------------|
| [ProxyStub](element-com-proxystub.md) | Registers a proxy stub. |
| [Interface](element-com-interface.md) | Registers new COM Interfaces. |
| [TypeLib](element-com-typelib.md) | Registers a type library. |

## Remarks
The **comInterface** extension can be under the Application/Extensions/Extension manifest element, or under the Package/Extensions/Extension manifest element. There is no functional difference between these two options, but both placements have different advantages.

If the extension is under Application/Extensions/Extension, you can improve the readability of the manifest by keeping interface registrations near the class registrations that implement them. However, if you place the extension under Package/Extensions/Extension, you won't need to determine which Application to use for each interface. It's possible to use multiple **comInterface** extensions in either Application/Extensions/Extension or Package/Extensions/Extension, but this is neither recommended nor necessary.

> [!NOTE]
> Any registrations in **comInterface** that depend on another registration (e.g. an **Interface** references a **ProxyStub** and/or a **TypeLib**) must be in the same **comInterface** extension. 

## Examples

## Requirements

|               |     Value                                                        |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/manifest/com/windows10` |