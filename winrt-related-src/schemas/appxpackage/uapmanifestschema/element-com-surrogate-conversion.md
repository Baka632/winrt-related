---

ms.assetid: b51ea723-898b-4864-ac9f-8bc4c7672df9
title: com:Conversion (in SurrogateServer/Class)
description: Specifies the formats an application can read and write (in SurrogateServer/Class).

ms.date: 03/29/2017
ms.topic: reference


keywords: windows 10, uwp, schema, manifest, com
---


# com:Conversion (in SurrogateServer/Class)

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
<dt><a href="element-com-surrogateserver.md">&lt;com:SurrogateServer&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-com-surrogateserver-class.md">&lt;com:Class&gt;</a></dt>
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
  Readable?,
  ReadWritable?
</com:Conversion>
```

## Key
`?`    optional (zero or one) 

## Child Elements

| Child Element | Description |
|---------------|-------------|
| [Readable](element-com-surrogate-readable.md) | Specifies that the application can only read files. |
| [ReadWritable](element-com-surrogate-readwritable.md) | Specifies that the application can read and write files. |

## Remarks

## Examples

## Requirements
|               |    Value                                                         |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/manifest/com/windows10` |