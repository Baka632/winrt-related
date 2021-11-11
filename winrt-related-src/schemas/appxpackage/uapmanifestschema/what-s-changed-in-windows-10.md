---
title: What's different in Windows 10
description: This topic lists changes to the package manifest schema reference for each version of Windows 10, including namespaces and features that have been added or changed.
ms.assetid: 2afadf58-6dcc-4959-b97b-47d2075af692
keywords: windows 10, uwp, schema, package manifest
ms.topic: reference
ms.date: 01/16/2020
ms.custom: 19H1
---

# What's different in Windows 10

This topic lists changes to the package manifest schema reference for each version of Windows 10, including namespaces and features that have been added or changed. See the [Element Hierarchy](root-elements.md) for reference info on all elements, attributes, and types in the schema.

The following sections list the namespaces and XML prefixes added to the package manifest schema in each update of Windows 10. To get the latest version of Windows 10, see [Download Windows 10](https://www.microsoft.com/software-download/windows10).

## Windows 11 - Build 22000
### Added namespaces and XML prefixes 
| Prefix        | Namespace | 
|---------------|-----------|
| desktop9           | `http://schemas.microsoft.com/appx/manifest/desktop/windows10/9` |

## Windows 10 - Build 20348
### Added namespaces and XML prefixes 
| Prefix        | Namespace | 
|---------------|-----------|
| desktop7           | `http://schemas.microsoft.com/appx/manifest/desktop/windows10/7` |

## Windows 10, Version 2004
### Added namespaces and XML prefixes
| Prefix   | Namespace |
|----------|-----------|
| uap10     | `http://schemas.microsoft.com/appx/manifest/uap/windows10/10` |
| com3     | `http://schemas.microsoft.com/appx/manifest/com/windows10/3` |

## Windows 10, Build 18362, Version 1903
### Added namespaces and XML prefixes
| Prefix   | Namespace | 
|----------|-----------|
| uap8     | `http://schemas.microsoft.com/appx/manifest/uap/windows10/8` | 
| desktop6 | `http://schemas.microsoft.com/appx/manifest/desktop/windows10/6` |
| rescap6  | `http://schemas.microsoft.com/appx/manifest/foundation/windows10/restrictedcapabilities/6` |

## Windows 10, Build 17763, Version 1809
### Added namespaces and XML prefixes
| Prefix   | Namespace | 
|----------|-----------|
| uap7     | `http://schemas.microsoft.com/appx/manifest/uap/windows10/7` | 
| desktop5 | `http://schemas.microsoft.com/appx/manifest/desktop/windows10/5` |
| rescap5  | `http://schemas.microsoft.com/appx/manifest/foundation/windows10/restrictedcapabilities/5` |

## Windows 10, Build 17134, Version 1803
### Added namespaces and XML prefixes
| Prefix   | Namespace | 
|----------|-----------|
| uap6     | `http://schemas.microsoft.com/appx/manifest/uap/windows10/6` | 
| desktop4 | `http://schemas.microsoft.com/appx/manifest/desktop/windows10/4` |
| rescap4  | `http://schemas.microsoft.com/appx/manifest/foundation/windows10/restrictedcapabilities/4` | 


## Windows 10, Fall Creators Update - Build 16299.15, Version 1709
### Added namespaces and XML prefixes 
| Prefix   | Namespace | 
|----------|-----------|
| com2     | `http://schemas.microsoft.com/appx/manifest/com/windows10/2` |
| desktop3 | `http://schemas.microsoft.com/appx/manifest/desktop/windows10/3` |
| uap5     | `http://schemas.microsoft.com/appx/manifest/uap/windows10/5` |

## Windows 10, Creators Update - Build 15063, Version 1703
### Added namespaces and XML prefixes 
| Prefix   | Namespace | 
|----------|-----------|
| com      | `http://schemas.microsoft.com/appx/manifest/com/windows10` |
| desktop2 | `http://schemas.microsoft.com/appx/manifest/desktop/windows10/2` |
| rescap3  | `http://schemas.microsoft.com/appx/manifest/foundation/windows10/restrictedcapabilities/3` |
| uap4     | `http://schemas.microsoft.com/appx/manifest/uap/windows10/4` |


## Windows 10, Anniversary Update - Build 14393, Version 1607
### Added namespaces and XML prefixes 
| Prefix  | Namespace | 
|---------|-----------|
| desktop | `http://schemas.microsoft.com/appx/manifest/desktop/windows10` |
| rescap2 | `http://schemas.microsoft.com/appx/manifest/foundation/windows10/restrictedcapabilities/2` |
| uap3    | `http://schemas.microsoft.com/appx/manifest/uap/windows10/3` |


## Windows 10, November Update - Build 10586, Version 1511
### Added namespaces and XML prefixes 
| Prefix   | Namespace | 
|----------|-----------|
| f2       | `http://schemas.microsoft.com/appx/manifest/foundation/windows10/2` |
| uap2     | `http://schemas.microsoft.com/appx/manifest/uap/windows10/2` |


## Windows 10 - Build 10240, Version 1507
### Added namespaces and XML prefixes 
| Prefix        | Namespace | 
|---------------|-----------|
| uap           | `http://schemas.microsoft.com/appx/manifest/uap/windows10` |
| f             | `http://schemas.microsoft.com/appx/manifest/foundation/windows10` |
| holo          | `http://schemas.microsoft.com/appx/manifest/holographic/windows10` |
| mobile        | `http://schemas.microsoft.com/appx/manifest/mobile/windows10` |
| rescap        | `http://schemas.microsoft.com/appx/manifest/foundation/windows10/restrictedcapabilities` |
| serverpreview | `http://schemas.microsoft.com/appx/manifest/serverpreview/windows10` |  



<!-- This section specifies changes from Windows 8.x to Windows 10. This information is probably no longer needed. 

## Elements and attributes that have been added

-   [**uap:Capability**](element-uap-capability.md) element (and its child elements). Valid values for the uap:Capability@Name attribute are "documentsLibrary", "picturesLibrary", "videosLibrary", "musicLibrary", "enterpriseAuthentication", "sharedUserCertificates", "userAccountInformation", "removableStorage", "appointments", "contacts", "phoneCall", and "blockedChatMessages". See [App capability declarations](/windows/uwp/packaging/app-capability-declarations).
-   [**uap:Extension**](element-uap-extension.md) element. Valid values for the uap:Extension@Category attribute are "windows.webAccountProvider", "windows.dialProtocol", "windows.appService", "windows.mediaPlayback", and "windows.print3DWorkflow".
-   [**PublisherCacheFolders**](element-publishercachefolders.md) element.
-   [**uap:SupportedUsers**](element-uap-supportedusers.md) element.
-   [**uap:Task**](element-uap-task.md) element. Valid values for the @Type attribute are "chatMessageNotification", "vpnClient", "phoneCall", and "mediaProcessing".
-   [**Application\@ResourceGroup**](element-application.md) attribute.
-   [**uap:FileTypeAssociation\@DesiredView**](element-uap-filetypeassociation.md) attribute.
-   [**uap:Protocol\@DesiredView**](element-uap-protocol.md) attribute.
-   [**uap:Protocol\@ReturnResults**](element-uap-protocol.md) attribute.
-   [**uap:Rule\@WindowsRuntimeAccess**](element-uap-rule.md) attribute.
-   [**uap:VisualElements\@AppListEntry**](element-uap-visualelements.md) attribute.

## Elements and attributes that have changed
-   The [**uap:ApplicationContentUriRules**](element-uap-applicationcontenturirules.md) element (and its child elements) is now in an xml namespace that uses the "uap:" xml namespace prefix.
-   For the [**Capability**](element-capability.md) element, some values for the @Name attribute have moved to the new [**uap:Capability**](element-uap-capability.md) element. Valid values for **Capability\@Name** are now "internetClient", "internetClientServer", "privateNetworkClientServer", and "allJoyn". See [App capability declarations](/previous-versions/windows/apps/hh464936(v=win.10)).
-   For the [**Extension**](element-1-extension.md) element, some values for the @Category attribute have moved to the new [**uap:Extension**](element-uap-extension.md) element. For **Extension\@Category**, new valid values are "windows.preInstalledConfigTask", "windows.updateTask", and "windows.restrictedLaunch". The values "windows.contactPicker" and "windows.contact" have been removed.
-   The Application/Extensions/Extension/[**uap:FileTypeAssociation**](element-uap-filetypeassociation.md) element is now in an xml namespace that uses the "uap:" xml namespace prefix.
-   The Application/Extensions/Extension/[**uap:Protocol**](element-uap-protocol.md) element is now in an xml namespace that uses the "uap:" xml namespace prefix.
-   The Application/Extensions/Extension/[**uap:AutoPlayContent**](element-uap-autoplaycontent.md) element is now in an xml namespace that uses the "uap:" xml namespace prefix.
-   The Application/Extensions/Extension/[**uap:AutoPlayDevice**](element-uap-autoplaydevice.md) element is now in an xml namespace that uses the "uap:" xml namespace prefix.
-   The Application/Extensions/Extension/[**uap:ShareTarget**](element-uap-sharetarget.md) element is now in an xml namespace that uses the "uap:" xml namespace prefix.
-   The Application/Extensions/Extension/[**uap:FileOpenPicker**](element-uap-fileopenpicker.md) element is now in an xml namespace that uses the "uap:" xml namespace prefix.
-   The Application/Extensions/Extension/[**uap:FileSavePicker**](element-uap-filesavepicker.md) element is now in an xml namespace that uses the "uap:" xml namespace prefix.
-   The Application/Extensions/Extension/[**uap:AppointmentsProvider**](element-uap-appointmentsprovider.md) element is now in an xml namespace that uses the "uap:" xml namespace prefix.
-   The [**Application\@StartPage**](element-application.md) attribute was previously required to be a relative Windows file path referencing a document in the app's package. Now it additionally may be an absolute URL (so that a web site can publish as an app in the Store).
-   For the [**DeviceCapability\@Name**](element-devicecapability.md) attribute, new valid values are "bluetooth", "wiFiControl", "radios", and "optical". See [App capability declarations](/previous-versions/windows/apps/hh464936(v=win.10)).
-   The [**PackageDependency\@Publisher**](element-packagedependency.md) attribute is now required.
-   For the [**Task\@Type**](element-task.md) attribute, new valid values are "general", "deviceConnectionChange", and "bluetooth".
-   The [**uap:VisualElements**](element-uap-visualelements.md) element (and its child elements) is now in an xml namespace that uses the "uap:" xml namespace prefix.
-   The [**VisualElements\@Logo**](../appxmanifestschema2010-v2/element-visualelements.md) attribute has been renamed [**uap:VisualElements\@Square150x150Logo**](element-uap-visualelements.md).
-   The [**VisualElements\@Square30x30Logo**](../appxmanifestschema2010-v2/element-visualelements.md) attribute has been renamed [**uap:VisualElements\@Square44x44Logo**](element-uap-visualelements.md).
-   The [**VisualElements\@Square70x70Logo**](../appxmanifestschema2010-v2/element-visualelements.md) attribute has been renamed [**uap:VisualElements\@Square71x71Logo**](element-uap-visualelements.md).

### Removed attributes and elements 
-   [**ApplicationView**](../appxmanifestschema2013/element-applicationview.md) element.
-   [**Prerequisites**](../appxmanifestschema2010-v2/element-prerequisites.md) element.
-   [**VisualElements\@DefaultSize**](../appxmanifestschema2010-v2/element-visualelements.md) attribute.
-   [**VisualElements\@ForegroundText**](../appxmanifestschema2010-v2/element-visualelements.md) attribute.
-   [**VisualElements\@SmallLogo**](../appxmanifestschema2010-v2/element-visualelements.md) attribute.
-   [**VisualElements\@ToastCapable**](../appxmanifestschema2010-v2/element-visualelements.md) attribute.

-->

## Example

To use an XML namespace in the the app package manifest, include the namespaces and `IgnorableNamespaces` within the [`Package`](./element-package.md) element.

```xml
<?xml version='1.0' encoding='utf-8'?>
<Package
  xmlns="http://schemas.microsoft.com/appx/manifest/foundation/windows10"
  xmlns:uap="http://schemas.microsoft.com/appx/manifest/uap/windows10"
  xmlns:uap4="http://schemas.microsoft.com/appx/manifest/uap/windows10/4"
  IgnorableNamespaces="uap uap4">
```