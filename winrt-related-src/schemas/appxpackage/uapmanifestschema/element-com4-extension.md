---
title: com4:Extension
description: Provides functionality to expose COM registrations to clients outside of the app package (com4:Extension).
ms.date: 03/13/2022
ms.topic: reference
keywords: windows 10, windows 11, uwp, schema, manifest, com
---

# com4:Extension



## Description

Provides functionality to expose COM registrations to clients outside of the app package. The com4 extension is a new version that is a superset of and replacement for the previous COM schema versions. See the Remarks section for more information.



## Element Hierarchy
<dl><dt><a href = "element-package.md">&lt;Package&gt;</a></dt>
<dd>
<dl><dt><a href = "element-applications.md">&lt;Applications&gt;</a></dt>
<dd>
<dl><dt><a href = "element-application.md">&lt;Application&gt;</a></dt>
<dd>
<dl><dt><a href = "element-1-extensions.md">&lt;Extensions&gt;</a></dt>
<dd>
<dd><b>&lt;com4:Extension&gt;</b></dd></dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax
```syntax
<com4:Extension     Category = "windows.comServer" | "windows.comInterface"
    Executable? = A string between 1 and 256 characters in length that must end with ".exe" and cannot contain these characters: <, >, :, ", |, ?, or *.
    EntryPoint? = A string between 1 and 256 characters in length that cannot start or end with a whitespace character.
    RuntimeType? = A string between 1 and 255 characters in length that cannot start or end with a period or contain these characters: <, >, :, ", /, \, |, ?, or *.
    StartPage? = A string between 1 and 256 characters in length that cannot contain these characters: <, >, :, ", |, ?, or *.
    ResourceGroup? = An alphanumeric string between 1 and 255 characters in length. Must begin with an alphabetic character.
    TrustLevel? = "appContainer" | "mediumIL"
    RuntimeBehavior? = "windowsApp" | "packagedClassicApp" | "win32App"
    HostId? = An alphanumeric string between 1 and 255 characters in length. Must begin with an alphabetic character.
    Parameters? = A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end.
    Id? = A string between 1 and 255 characters in length with a non-whitespace character at its beginning and end.
    Subsystem? = "console" | "windows"
    SupportsMultipleInstances? = Boolean.
    ResourceGroup? = An alphanumeric string between 1 and 255 characters in length. Must begin with an alphabetic character.
    CurrentDirectoryPath? = A string that cannot contain these characters: <, >, |, ?, or *. >
    Parameters? = A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end.
    CompatMode? = "classic" | "modern"
    Scope? = "machine" | "user"
>
<!-- Child elements -->
  (com4:ComServer |
  com4:ComInterface)
</com4:Extension>
```

## Key
`?`    optional (zero or one) 


## Attributes

| Attribute | Description | Data type | Required |
| -----------| -------------| -----------| ----------|
| Category | The type of app extensibility point. | One of the following values: "windows.comServer" , "windows.comInterface"| Yes |
| Executable | A path relative to the package root and must reference a file in the package. This specifies the default executable for the extension. If not specified, the executable defined for the app is used.  If specified, the EntryPoint property is also used. If that EntryPoint property isn't specified, the EntryPoint defined for the app is used. | One of the following values: A string between 1 and 256 characters in length that must end with ".exe" and cannot contain these characters: <, >, :, ", ,, ?, or *.| No |
| EntryPoint | The activatable class ID. | A string between 1 and 256 characters in length that cannot start or end with a whitespace character.| No |
| RuntimeType | The runtime provider. This attribute is used typically when there are mixed frameworks in an app. | One of the following values: A string between 1 and 255 characters in length that cannot start or end with a period or contain these characters: <, >, :, ", /, \, ,, ?, or *.| No |
| StartPage | The web page that handles the extensibility point. | One of the following values: A string between 1 and 256 characters in length that cannot contain these characters: <, >, :, ", ,, ?, or *.| No |
| ResourceGroup | A tag that you can use to group extension activations together for resource management purposes (for example, CPU and memory). The value you can set ResourceGroup is free-form and flexible. See [Application@ResourceGroup](element-application.md). | An alphanumeric string between 1 and 255 characters in length. Must begin with an alphabetic character.| No |
| uap10:TrustLevel | Specifies the trust level of the extension. | One of the following values: "appContainer" , "mediumIL"| No |
| uap10:RuntimeBehavior | Specifies the run time behavior of the extension. | One of the following values: "windowsApp" , "packagedClassicApp" , "win32App"| No |
| uap10:HostId | This value specifies the app ID of the host app for the extension. | An alphanumeric string between 1 and 255 characters in length. Must begin with an alphabetic character.| No |
| uap10:Parameters | Contains command line parameters to pass to the extension. Only supported for desktop apps that have package identity. | A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end.| No |
| uap11:Id | TBD - The definitions I've found for the ManganeseExtensionAttributesGroup attributes don't all seem applicable to this extension. | TBD - The definitions I've found for the ManganeseExtensionAttributesGroup attributes don't all seem applicable to this extension. | No |
| uap11:Subsystem | TBD - The definitions I've found for the ManganeseExtensionAttributesGroup attributes don't all seem applicable to this extension.  | One of the following values: "console" , "windows"| No |
| uap11:SupportsMultipleInstances | TBD - The definitions I've found for the ManganeseExtensionAttributesGroup attributes don't all seem applicable to this extension.  | Boolean.| No |
| uap11:ResourceGroup | TBD - The definitions I've found for the ManganeseExtensionAttributesGroup attributes don't all seem applicable to this extension.  | An alphanumeric string between 1 and 255 characters in length. Must begin with an alphabetic character.| No |
| uap11:CurrentDirectoryPath | TBD - The definitions I've found for the ManganeseExtensionAttributesGroup attributes don't all seem applicable to this extension.  | One of the following values: A string that cannot contain these characters: <, >, ,, ?, or *. >| No |
| uap11:Parameters | TBD | A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end.| No |
| desktop7:CompatMode | TBD | One of the following values: "classic" , "modern"| No |
| desktop7:Scope | TBD | One of the following values: "machine" , "user"| No |


## Child Elements

| Element | Description |
| -----------| -------------|
| [com4:ComServer](element-com4-comserver.md) | Declares a package extension point of type windows.comServer. The comServer extension may include four types of registrations: Class, ServiceServer, SurrogateServer, InProcessServer, InProcessHandler, ManagedInProcessServer. |
| [com4:ComInterface](element-com4-cominterface.md) | Declares a package extension point of type **windows.comInterface** (com4:ComInterface). |

## Remarks

The com4 extension is essentially a rewrite of the old windows.comServer/windows.comInterface extension syntax. This extension is a superset of the previous com extension functionality, with identical behavior for the inherited syntax. One fundamental change in the com4 extension is the strict enforcement of unique key and keyref attributes (e.g. Id attributes). In the previous version, each extension was treated as a separate document, allowing non-unique keys and dangling references to be validated.	Applications targeting Windows 11 that can use the new com4 namespace for all of their windows.comServer/windows.comInterface extensions should use it. Mixing the new namespace with the older namespaces is not recommended.

The following example shows how to register an out-of-process and an in-process server implementation for the same class.

```xml
<com4:Class Id="f4ed7720-9b3a-44a4-xxxx-xxxxxxxxxxxx" DisplayName="CLSID_Foo"/> 
<com:ExeServer Executable="MyServer.exe" DisplayName="My server">  
  <com4:ClassReference Id="f4ed7720-9b3a-44a4-xxxx-xxxxxxxxxxxx"/>  
</com:ExeServer> 
<com4:InProcessServer Path="MyServer.dll">  
  <com4:ClassReference Id="f4ed7720-9b3a-44a4-xxxx-xxxxxxxxxxxx"/>  
</com4:InProcessServer> 

```

### New features in the com4 extension

- Support for in-process servers (both unmanaged and managed) and custom in-process handlers (i.e. not the OLE default handler). This capability is currently functionally limited and restricted by policy:
    - This is currently only intended for use by sparse packages and doesn’t work for most normal packages due to ACLs on the install location that prevent the package’s dlls from being loaded outside the package. For more information on sparse packages, see [Grant identity to non-packaged desktop apps](/windows/apps/desktop/modernize/grant-identity-to-nonpackaged-apps).
    -	Use of any of the com4 syntax requires a custom capability Microsoft.classicAppCompat_8wekyb3d8bbwe
- It is now possible to associate a TypeLib with a class registration. 



## Requirements
| Prefix | Value |
| ---------------| -------------------------------------------------------------|
| com4 | http://schemas.microsoft.com/appx/manifest/com/windows10/4 |


