---
description: A friendly name for the publisher that can be displayed to users (Windows 10).
Search.Product: eADQiWindows 10XVcnh
title: PublisherDisplayName (Windows 10)
ms.assetid: 8df2d218-e62d-4b2e-8db5-3436c67aa04c
keywords: windows 10, uwp, schema, package manifest
ms.topic: reference
ms.date: 04/05/2017
---

# PublisherDisplayName (Windows 10)

A friendly name for the publisher that can be displayed to users.

## Element hierarchy

[\<Package\>](element-package.md)

&nbsp;&nbsp;&nbsp;&nbsp;[\<Properties\>](element-properties.md)

&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;**\<PublisherDisplayName\>**

## Syntax

```xml
<PublisherDisplayName>
  A string with a value between 1 and 256 characters in length. This string is localizable. 
</PublisherDisplayName>
```

## Attributes and elements

### Attributes

None.

### Child elements

None.

### Parent elements

| Parent element | Description |
|-|-|
| [Properties](element-properties.md) | Defines additional metadata about the package including attributes that describe how the package appears to users. |

> [!NOTE]
> You may get an error if the manifest elements DisplayName or Description contain characters disallowed by the Windows firewall; namely `|` and `all`, due to which Windows fails to create the AppContainer profile for the package. Use this reference for [troubleshooting](/windows/win32/appxpkg/troubleshooting) if you get an error.

## Remarks

This string is localizable.

## Requirements

| Item | Value |
|--|--|
| **Namespace** | `http://schemas.microsoft.com/appx/manifest/foundation/windows10` |
