---
ms.assetid: ae4a725d-10f9-4e03-a579-c3db2d859a9f
title: com:Extension (Windows 10)
description: Provides functionality to expose COM registrations to clients outside of the app package.
ms.date: 03/29/2017
ms.topic: reference
keywords: windows 10, uwp, schema, manifest, com
---


# com:Extension (Windows 10)

## Description
Provides functionality to expose COM registrations to clients outside of the app package.

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
<dd><b>&lt;com:Extension&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
</dl>


## Syntax
```syntax
<com:Extension Category = "windows.comServer" | "windows.comInterface" 
               uap10:TrustLevel?   = String value. Can be one of the following: "appContainer", "mediumIL".
               ap10:RuntimeBehavior?  = String value. Can be one of the following: "windowsApp", "packagedClassicApp", "win32App".
               uap10:HostId?       = An alphanumeric string between 1 and 255 characters in length. Must begin with an alphabetic character.
               ap10:Parameters?   = A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end. >

  <!-- Child elements -->
  ( com:ComServer
  | com:ComInterface )
</com:Extension>
```

## Key

## Attributes

| Attribute | Description | Data type | Required |
|-----------|-------------|-----------|----------|
| Category | The type of app extensibility point. | This attribute can have one of the following values: <ul><li>windows.comServer</li><li>windows.comExtension</li></ul>| Yes |
| uap10:TrustLevel | Specifies the trust level of the extension. | String value. Can be one of the following: "appContainer", "mediumIL".  | No |
| uap10:RuntimeBehavior | Specifies the run time behavior of the extension. | String value. Can be one of the following: "windowsApp", "packagedClassicApp", "win32App".  | No |
| uap10:HostId | Specifies the app ID of the host app for the extension. | An alphanumeric string between 1 and 255 characters in length. Must begin with an alphabetic character.  | No |
| uap10:Parameters | Contains command line parameters to pass to the extension. Only supported for desktop apps that have package identity. | A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end.  | No |


## Child Elements

| Child Element         | Description |
|-----------------------|-------------|
| [com:ComServer](element-com-comserver.md) | Declares a package extension point of type **windows.comServer**. |
| [com:ComInterface](element-com-cominterface.md) | Declares a package extension point of type **windows.comInterface**. |

## Parent Elements

| Parent Element | Description |
|----------------|-------------|
| [Extensions (type: CT_ApplicationExtensions)](element-1-extensions.md) | Defines one or more extensibility points for the app. |

## Remarks

## Examples

## Requirements

|               |       Value                                                      |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/manifest/com/windows10`<br/><br/>`http://schemas.microsoft.com/appx/manifest/uap/windows10/10` (for the **uap10** attributes) |
