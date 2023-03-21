---
description: Identifies the device family that your package targets (in Package/Dependencies). 
Search.Product: eADQiWindows 10XVcnh
title: TargetDeviceFamily (Windows 10)
ms.assetid: 457745aa-bc12-427b-b1f1-74c1618753c0
keywords: windows 10, uwp, schema, package manifest
ms.topic: reference
ms.date: 04/05/2017
---

# TargetDeviceFamily (Windows 10)

Identifies the device family that your package targets. For more info about device families, see [Programming with extension SDKs](/uwp/extension-sdks/device-families-overview).

## Element hierarchy

[\<Package\>](element-package.md)

&nbsp;&nbsp;&nbsp;&nbsp;[\<Dependencies\>](element-dependencies.md)

&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;**\<TargetDeviceFamily\>**

## Syntax

```xml
<TargetDeviceFamily
    Name = 'An alphanumeric string that can contain period and dash characters.'
    MinVersion = 'A version string in quad notation ("Major.Minor.Build.Revision"), where Major cannot be 0.'
    MaxVersionTested = 'A version string in quad notation ("Major.Minor.Build.Revision"), where Major cannot be 0.' />
```

## Attributes and elements

### Attributes

| Attribute | Description | Data type | Required | Default value |
|-|-|-|-|-|
| **Name** | The name of the device family that your app is targeting. See the [Examples](#examples) section for more information about the supported device family names. | An alphanumeric string that can contain period and dash characters. | Yes |  |
| **MinVersion** | The minimum version of the device family that your app is targeting. Used for applicability at deployment time. If the device family version of the system is lower than *MinVersion*, then the app is not considered applicable. | A version string in quad notation (`Major.Minor.Build.Revision`), where `Major` cannot be `0`. | Yes |  |
| **MaxVersionTested** | The maximum version of the device family that your app is targeting that you have tested it against. This is used at runtime to determine the effective process space for quirks. | A version string in quad notation (`Major.Minor.Build.Revision`), where `Major` cannot be `0`. | Yes |  |

### Child elements

None.

### Parent elements

| Parent element | Description |
|-|-|
| [Dependencies](element-dependencies.md) | Declares other packages that a package depends on to complete its software. |

## Examples

To target the set of APIs known as the "universal device family" (which means your app runs on all devices), just specify that one device family, as in the example below. You can still write adaptive code to light up APIs outside of the universal device family when your app is running on devices in specific device families. Versions 10.0.x.0 and 10.0.y.0 can, of course, be the same value.

```xml
<Dependencies>
    <TargetDeviceFamily Name="Windows.Universal" MinVersion="10.0.x.0" MaxVersionTested="10.0.y.0"/>
</Dependencies>
```

> [!NOTE]
> If you target "Windows.Universal" with both "MinVersion" and "MaxVersionTested" set to version 10.0.0.0, your app will use the versions specified in the Target Min Version and Target Version of the project file, respectively. If you are using "Windows.Universal" with "MinVersion" and "MaxVersionTested" set to a value other than 10.0.0.0, the app will target the specified "MinVersion" and "MaxVersionTested" instead of the values specified in the project file.

All child device families "derive" from (that is, they include) the "universal device family" set of APIs. So, a child device family implies "universal plus other child-device-family-specific APIs". When you target a child device family, you don't need to mention universal. In this next example, the app is targeting the set of APIs known as the "mobile device family", and consequently it will run only on devices that implement the mobile device family set of APIs (mobile devices). Replace "Mobile" with "Desktop", "Xbox", "Holographic", "IoT", or "IoTHeadless" for example, if you want to target another device family.

```xml
<Dependencies>
    <TargetDeviceFamily Name="Windows.Mobile" MinVersion="10.0.x.0" MaxVersionTested="10.0.y.0"/>
</Dependencies>
```

> [!NOTE]
> If the app is targeting a device family other than "Windows.Universal", the "MinVersion" and "MaxVersionTested" must be properly specified for the device family that is targeted.

To target the Xbox device family, set the Name attribute to "Windows.Xbox". Note that to target the Xbox device family, the MinVersion must be set to at least 10.0.14393.0.

```xml
<Dependencies>
    <TargetDeviceFamily Name="Windows.Xbox" MinVersion="10.0.x.0" MaxVersionTested="10.0.y.0"/>
</Dependencies>
```

If your app is created specifically for HoloLens and is not supported on other platforms, specify the target device family "Windows.Holographic".

```xml
<Dependencies>
    <TargetDeviceFamily Name="Windows.Holographic" MinVersion="10.0.x.0" MaxVersionTested="10.0.y.0"/>
</Dependencies>
```

If your app targets the Windows 10 Team Edition exclusively, set the Name attribute to "Windows.Team". This is commonly used for Microsoft Surface Hub devices.

```xml
<Dependencies>
    <TargetDeviceFamily Name="Windows.Team" MinVersion="10.0.x.0" MaxVersionTested="10.0.y.0"/>
</Dependencies>
```

If you want to target the IoT Core platform, set the Name attribute to "Windows.IoT". For a headless IoT app, use "Windows.IoTHeadless".

```xml
<Dependencies>
    <TargetDeviceFamily Name="Windows.IoT" MinVersion="10.0.x.0" MaxVersionTested="10.0.y.0"/>
</Dependencies>
```

> [!NOTE]
> Currently, apps targeting IoT or IoTHeadless are not valid in the app store and should be used for development purposes only.

In this example, the app targets the mobile and desktop device families. Consequently the app can run on mobile devices or on desktop devices, but no others. Note that the app must use adaptive code to call any API that is not in the universal device family set of APIs (unless the API happens to be shared by both device families).

```xml
<Dependencies>
    <TargetDeviceFamily Name="Windows.Mobile" MinVersion="10.0.x.0" MaxVersionTested="10.0.y.0"/>
    <TargetDeviceFamily Name="Windows.Desktop" MinVersion="10.0.x.0" MaxVersionTested="10.0.y.0"/>
</Dependencies>
```

In this last example, the app targets the universal device family (so, by default, it runs on all devices with the specified minimum version). The exception being that, for devices that implement the mobile device family, the app requires at least version 10.0.m.0 to be present. This is how you indicate that you do not support versions of child device families earlier than a specified minimum version, even if that differs from the version you support for the general case (the universal device family case). Also note the MaxVersionTested value for the mobile device family dependency in the example. Where z \> n, the app will run on version 10.0.z.0 of a mobile device, but it will experience 10.0.n.0-version behavior from the platform on that version.

```xml
<Dependencies>
    <TargetDeviceFamily Name="Windows.Universal" MinVersion="10.0.x.0" MaxVersionTested="10.0.y.0"/>
    <TargetDeviceFamily Name="Windows.Mobile" MinVersion="10.0.m.0" MaxVersionTested="10.0.n.0"/>
</Dependencies>
```

## Requirements

| Requirement | Value |
|--|--|
| Namespace | `http://schemas.microsoft.com/appx/manifest/foundation/windows10` |
