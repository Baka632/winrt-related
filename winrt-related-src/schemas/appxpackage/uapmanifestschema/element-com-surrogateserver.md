---

ms.assetid: 66534b5a-4f04-4fc6-9a3f-91a7b82930e9
title: com:SurrogateServer
description: Registers a SurrogateServer with one or many class registrations.

ms.date: 03/29/2017
ms.topic: reference


keywords: windows 10, uwp, schema, manifest, com
---


# com:SurrogateServer

## Description
Registers a SurrogateServer with one or many class registrations.

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
<dd><b>&lt;com:SurrogateServer&gt;</b></dd>
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
<com:SurrogateServer  
    CustomSurrogateExecutable? = A string between 1 and 256 characters in length that must end with ".exe" and cannot contain these characters: <, >, :, ", |, ?, or *.
    DisplayName? = A string between 1 and 256 characters in length. This string is localizable.
    LaunchAndActivationPermission? = [SDDL string](/windows/win32/secauthz/security-descriptor-string-format).
    AppId? = A GUID in the form xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx. 
    SystemSurrogate? = A string type. >

  <!-- Child elements -->
  Class{1,10000}
</com:SurrogateServer>
```

## Key
`{}`   specific range of occurrences

## Attributes

| Attribute | Description | Data type | Required |
|-----------|-------------|-----------|----------|
| CustomSurrogateExecutable | A path to the DllSurrogate in the AppId key. This path is relative to the package root and must reference a file in the package. This is mututally exclusive with SystemSurrogate. | A string between 1 and 256 characters in length that must end with ".exe" and cannot contain these characters: <, >, :, ", &#124;, ?, or * | No |
| DisplayName | DisplayName is a localizable string corresponding to the default AppID key value. | A string between 1 and 256 characters in length. | No |
| LaunchAndActivationPermission | An [SDDL string](/windows/win32/secauthz/security-descriptor-string-format) that corresponds to the LaunchPermission value of the AppID key. | [SDDL string](/windows/win32/secauthz/security-descriptor-string-format). | No |
| AppId | The AppId that references the associated AppId key. | A GUID in the form xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx. | No |
| SystemSurrogate | A value that corresponds to well-known values from the DllSurrogate value of the AppId key. This is mututally exclusive with CustomSurrogateExecutable. | A string type | No |

## Child Elements

| Child Element | Description |
|---------------|-------------|
| [Class](element-com-surrogateserver-class.md) | Defines a SurrogateServer class registration. |

## Remarks
If there is no value for the DllSurrogate in the [AppId key](/windows/win32/com/appid-key), do not use the CustomSurrogateExecutable attribute.

**LaunchAndActivationPermission** is an [SDDL string](/windows/win32/secauthz/security-descriptor-string-format) that corresponds to the LaunchPermission value of the [AppID key](/windows/win32/com/appid-key).

The **SystemSurrogate** corresponds to the values of the DllSurrogate value of the AppId key. For example, if the DllSurrogate value is `%System32%\prevhost.exe` or `%SysWow64%\prevhost.exe`, then **SystemSurrogate** should be set to `PreviewHost` and the **CustomSurrogateExecutable** should not be set. 

## Examples

## Requirements
|               |     Value                                                        |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/manifest/com/windows10` |