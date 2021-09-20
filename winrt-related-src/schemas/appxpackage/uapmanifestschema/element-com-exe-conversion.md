---

ms.assetid: 2f6b2357-2e05-40ac-861d-7cd67202f0e2
title: com:Conversion (in ExeServer/Class)
description: Specifies the formats an application can read and write (in ExeServer/Class).

ms.date: 03/29/2017
ms.topic: reference


keywords: windows 10, uwp, schema, manifest, com
---

# com:Conversion (in ExeServer/Class)

## Description
Specifies the formats an application can read and write.

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
<dd>
<dl>
<dt><a href="element-com-comserver.md">&lt;com:ComServer&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-com-exeserver.md">&lt;com:ExeServer&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-com-exeserver-class.md">&lt;com:Class&gt;</a></dt>
<dd><b>&lt;com:Conversion&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
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
<com:Conversion>
  <!-- Child elements -->
  ( Readable?,
  ReadWritable?
  )
</com:Conversion>
```

## Key
`?`    optional (zero or one) 

## Child Elements

| Child Element | Description |
|---------------|-------------|
| [Readable](element-com-exe-readable.md) | Specifies that the application can only read files. |
| [ReadWritable](element-com-exe-readwritable.md) | Specifies that the application can read and write files. |

## Remarks

## Examples

## Requirements
|               |    Value                                                         |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/manifest/com/windows10` |