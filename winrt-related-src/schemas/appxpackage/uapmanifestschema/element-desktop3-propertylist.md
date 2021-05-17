---

title: desktop3:PropertyList
description: Contains the properties that are under the Properties tab of a file.

ms.date: 10/10/2017
ms.topic: reference


keywords: windows 10, uwp, schema, manifest, desktop, extension 
---

# desktop3:PropertyList


## Description
Contains the properties that are under the Properties tab of a file.

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
<dt><a href="element-uap-extension.md">&lt;uap:Extension&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-uap-filetypeassociation.md">&lt;uap:FileTypeAssociation&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-desktop3-PropertyLists.md">&lt;desktop3:PropertyLists&gt;</a></dt>
<dd><b>&lt;desktop3:PropertyList&gt;</b></dd>
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
<desktop3:PropertyList Property = A string value as one of the following: "fullDetails", or "previewDetails"
                       Value    = A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end. />
```

## Attributes
| Attribute | Description | Data type | Required |
|-----------|-------------|-----------|----------|
| Property | Specifies whether the properties are displayed in the Preview Pane, or the Details tab of the Properties dialog box. | A string value as one of the following: "fullDetails", or "previewDetails" | Yes |
| Value | A list of property values, separated by semicolons, such as: System.Description; System.Content | A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end. | Yes |

## See Also
[Using Property Lists](/windows/win32/properties/building-property-handlers-property-lists)

## Requirements

|               |      Value                                                       |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/manifest/desktop/windows10/3` |