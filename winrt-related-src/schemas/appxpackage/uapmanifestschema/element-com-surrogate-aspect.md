---

ms.assetid: 2023c216-5faa-432e-9d03-796705436eb6
title: com:Aspect (in SurrogateServer/Class)
description: Specifies the desired data or view aspect of the object when drawing or getting data (in SurrogateServer/Class).

ms.date: 03/29/2017
ms.topic: reference


keywords: windows 10, uwp, schema, manifest, com
---

# com:Aspect (in SurrogateServer/Class)

## Description
Specifies the desired data or view aspect of the object when drawing or getting data.

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
<dd>
<dl>
<dt><a href="element-com-surrogate-miscstatus.md">&lt;com:MiscStatus&gt;</a></dt>
<dd><b>&lt;com:Aspect&gt;</b></dd>
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
</dd>
</dl>


## Syntax
```syntax
<com:Aspect  
    Type = A string as one of the enumeration values: Content, Thumbnail, Icon, or DocPrint.
    OleMiscFlag = An integer value in the range of 0-4194303. >
</com:Aspect>
```

## Key

## Attributes

| Attribute | Description | Data type | Required |
|-----------|-------------|-----------|----------|
| Type      | The string value for the view aspect of the object. | A string as one of the enumeration values: Content, Thumbnail, Icon, or DocPrint. | Yes |
| OleMiscFlag | The integer value for the view aspect of the object. | An integer value in the range of 0-4194303. | Yes |

## Remarks

## Examples

## Requirements
|               |       Value                                                      |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/manifest/com/windows10` |