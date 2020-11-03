---
Description: Declares a device capability required by a package.
Search.Product: eADQiWindows 10XVcnh
title: DeviceCapability
ms.assetid: 4353c4fd-f038-4986-81ed-d2ec0c6235ef


keywords: windows 10, uwp, schema, package manifest


ms.topic: reference
ms.date: 04/05/2017
---

# DeviceCapability




Declares a device capability required by a package.

## Element hierarchy

**&lt;DeviceCapability&gt;**

## Syntax

``` syntax
<DeviceCapability Name = A string between 1 and 50 characters in length or a GUID in the form xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx. />
```

## Attributes and Elements


### Attributes

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Attribute</th>
<th>Description</th>
<th>Data type</th>
<th>Required</th>
<th>Default value</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong>Name</strong></td>
<td><p>The name of the device capability, either specified as a friendly name or a device interface class GUID.</p></td>
<td>A string between 1 and 50 characters in length or a GUID in the form xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx.</td>
<td>Yes</td>
<td></td>
</tr>
</tbody>
</table>

 

### Child Elements

None.

### Parent Elements

This outermost (document) element may not be contained by any other elements.

## Remarks

If the *Name* attribute is specified as a GUID, then it is validated as GUID.

Apps are granted access to some devices by default. For UWP apps, this includes access to print and scanner devices. To access other types of devices, you must specify them using a **DeviceCapability** element. Some device capabilities must be added to the package manifest manually. For more info, see [How to specify device capabilities in a package manifest](../how-to-specify-device-capabilities-in-a-package-manifest.md).

For more info about capability declarations, see [App capability declarations](/previous-versions/windows/apps/hh464936(v=win.10)).

Some device capabilities require child elements. This table lists device capabilities by name or GUID and specifies if any child elements are required.

| Device capability                     | Description                                                                                                                                                                                                                                                                                                                                               |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **location**                          | Provides access to the user's current location.                                                                                                                                                                                                                                                                                                           |
| **microphone**                        | Provides access to the microphone's audio feed.                                                                                                                                                                                                                                                                                                           |
| **proximity**                         | Required for near-field communication (NFC) between devices in close proximity. Near-field proximity may be used to send files or connect with an app on a proximate device.                                                                                                                                                                              |
| **webcam**                            | Provides access to the camera's video feed.                                                                                                                                                                                                                                                                                                               |
| **usb**                               | Provides access to APIs in the [**Windows.Devices.Usb**](/uwp/api/Windows.Devices.Usb) namespace. This capability requires child elements. For more info, see [Updating the app manifest package for a USB device](/windows-hardware/drivers/usbcon/).                                                                                     |
| **humaninterfacedevice**              | Provides access to APIs in the [**Windows.Devices.HumanInterfaceDevice**](/uwp/api/Windows.Devices.HumanInterfaceDevice) namespace. This capability requires child elements. For more info, see [How to specify device capabilities for HID](../how-to-specify-device-capabilities-for-hid.md).                                             |
| **bluetooth.genericAttributeProfile** | Provides access to APIs in the [**Windows.Devices.Bluetooth.GenericAttributeProfile**](/uwp/api/Windows.Devices.Bluetooth.GenericAttributeProfile) namespace. This capability requires child elements. For more info, see [How to specify device capabilities for Bluetooth](../how-to-specify-device-capabilities-for-bluetooth.md). |
| **bluetooth.rfcomm**                  | Provides access to APIs in the [**Windows.Devices.Bluetooth.Rfcomm**](/uwp/api/Windows.Devices.Bluetooth.Rfcomm) namespace. This capability requires child elements. For more info, see [How to specify device capabilities for Bluetooth](../how-to-specify-device-capabilities-for-bluetooth.md).                                 |
| **pointOfService**                    | Provides access to Point of Service (POS) barcode scanners and magnetic stripe readers, via the [**Windows.Devices.PointOfService**](/uwp/api/Windows.Devices.PointOfService) namespace. These APIs are not supported on Windows Phone.                                                                                                                  |
| Other devices (represented by GUIDs)  | Includes specialized devices and Windows Portable Devices.                                                                                                                                                                                                                                                                                                |

 

## Examples

Here's an example of a [**Capabilities**](element-capabilities.md) node. For more examples, see [How to specify device capabilities in a package manifest](../how-to-specify-device-capabilities-in-a-package-manifest.md).

```XML
<Capabilities>
  <Capability Name="internetClient"/>
  <Capability Name="musicLibrary"/>
  <Capability Name="videosLibrary"/>
  <DeviceCapability Name="microphone"/>
  <DeviceCapability Name="webcam"/>
</Capabilities>
```

## See also


[App capability declarations](/previous-versions/windows/apps/hh464936(v=win.10))

[How to specify device capabilities in a package manifest](../how-to-specify-device-capabilities-in-a-package-manifest.md)

## Requirements

|               |                                                             |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/2010/manifest` |

 

 