---
description: Declares an extensibility point for the app.
Search.Product: eADQiWindows 10XVcnh
title: uap:Extension (Windows 10)
ms.assetid: b0c2ee51-897b-40be-aa38-372e2f94897f
keywords: windows 10, uwp, schema, package manifest
ms.topic: reference
ms.date: 01/16/2020
---

# uap:Extension (Windows 10)


Declares an extensibility point for the app.

## Element hierarchy

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
<dd><b>&lt;uap:Extension&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<Extension Category           = "windows.fileTypeAssociation" | "windows.protocol" | "windows.autoPlayContent" | "windows.autoPlayDevice" | "windows.shareTarget" | ...
           Executable?    = A string between 1 and 256 characters in length that must end with ".exe" and cannot contain these characters: <, >, :, ", |, ?, or *. It specifies the default executable for the extension. If not specified, the executable defined for the app is used.  If specified, the EntryPoint property is also used. If that EntryPoint property isn't specified, the EntryPoint defined for the app is used.
           EntryPoint?    = A string between 1 and 256 characters in length, representing the  task handling the extension. This is normally the fully namespace-qualified name of a Windows Runtime type. If EntryPoint is not specified, the EntryPoint defined for the app is used instead.
           RuntimeType?   = A string between 1 and 255 characters in length that cannot start or end with a period or contain these characters: <, >, :, ", /, \, |, ?, or *.
           StartPage?     = A string between 1 and 256 characters in length that cannot contain these characters: <, >, :, ", |, ?, or *.
           ResourceGroup? = An alphanumeric string between 1 and 255 characters in length. Must begin with an alphabetic character.
           uap10:TrustLevel?       = String value. Can be one of the following: "appContainer", "mediumIL".
           uap10:RuntimeBehavior?  = String value. Can be one of the following: "windowsApp", "packagedClassicApp", "win32App".
           uap10:HostId?           = An alphanumeric string between 1 and 255 characters in length. Must begin with an alphabetic character.
           uap10:Parameters?       = A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end. >

  <!-- Child elements -->
  ( uap:FileTypeAssociation
  | uap:Protocol
  | uap:AutoPlayContent
  | uap:AutoPlayDevice
  | uap:ShareTarget
  | uap:FileOpenPicker
  | uap:FileSavePicker
  | uap:AppointmentsProvider
  | uap:WebAccountProvider
  | uap:DialProtocol
  | uap:AppService
  | uap:MediaPlayback
  | uap:VoipCall
  )?

</uap:Extension>
```

### Key

`?`   optional (zero or one)

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
<td><strong>Category</strong></td>
<td><p>The type of app extensibility point.</p></td>
<td><p>This attribute can have one of the following values:</p>
<ul>
<li>windows.fileTypeAssociation</li>
<li>windows.protocol</li>
<li>windows.autoPlayContent</li>
<li>windows.autoPlayDevice</li>
<li>windows.shareTarget</li>
<li>windows.search</li>
<li>windows.fileOpenPicker</li>
<li>windows.fileSavePicker</li>
<li>windows.cachedFileUpdater</li>
<li>windows.cameraSettings</li>
<li>windows.accountPictureProvider</li>
<li>windows.printTaskSettings</li>
<li>windows.lockScreenCall</li>
<li>windows.appointmentsProvider</li>
<li>windows.alarm</li>
<li>windows.webAccountProvider</li>
<li>windows.dialProtocol</li>
<li>windows.appService</li>
<li>windows.mediaPlayback</li>
<li>windows.print3DWorkflow</li>
<li>windows.lockScreen</li>
<li>windows.aboveLockScreen</li>
<li>windows.personalAssistantLaunch</li>
<li>windows.voipCall</li>
</ul></td>
<td>Yes</td>
<td></td>
</tr>
<tr class="even">
<td><strong>EntryPoint</strong></td>
<td><p>The activatable class ID.</p></td>
<td>A string between 1 and 256 characters in length, representing the task handling the extension. This is normally the fully namespace-qualified name of a Windows Runtime type. If EntryPoint is not specified, the EntryPoint defined for the app is used instead.</td>
<td>No</td>
<td></td>
</tr>
<tr class="odd">
<td><strong>Executable</strong></td>
<td><p>The default launch executable.</p></td>
<td>A string between 1 and 256 characters in length that must end with &quot;.exe&quot; and cannot contain these characters: &lt;, &gt;, :, &quot;, |, ?, or *. It specifies the default executable for the extension. If not specified, the executable defined for the app is used. If specified, the EntryPoint property is also used. If that EntryPoint property isn't specified, the EntryPoint defined for the app is used.</td>
<td>No</td>
<td></td>
</tr>
<tr class="even">
<td><strong>ResourceGroup</strong></td>
<td><p>A tag that you can use to group extension activations together for resource management purposes (for example, CPU and memory). The value you can set ResourceGroup is free-form and flexible. See <a href="element-application.md"><strong>Application@ResourceGroup</strong></a>  and Remarks.</p></td>
<td>An alphanumeric string between 1 and 255 characters in length. Must begin with an alphabetic character.</td>
<td>No</td>
<td></td>
</tr>
<tr class="odd">
<td><strong>RuntimeType</strong></td>
<td><p>The runtime provider. This attribute is used typically when there are mixed frameworks in an app.</p></td>
<td>A string between 1 and 255 characters in length that cannot start or end with a period or contain these characters: &lt;, &gt;, :, &quot;, /, \, |, ?, or *.</td>
<td>No</td>
<td></td>
</tr>
<tr class="even">
<td><strong>StartPage</strong></td>
<td><p>The web page that handles the extensibility point.</p></td>
<td>A string between 1 and 256 characters in length that cannot contain these characters: &lt;, &gt;, :, &quot;, |, ?, or *.</td>
<td>No</td>
<td></td>
</tr>
<tr class="even">
<td><strong>uap10:TrustLevel</strong></td>
<td><p>Specifies the trust level of the extension.</p></td>
<td>String value. Can be one of the following: "appContainer", "mediumIL". </td>
<td>No</td>
<td></td>
</tr>
<tr class="odd">
<td><strong>uap10:RuntimeBehavior</strong></td>
<td><p>Specifies the run time behavior of the extension.</p></td>
<td>String value. Can be one of the following: "windowsApp", "packagedClassicApp", "win32App". </td>
<td>No</td>
<td></td>
</tr>
<tr class="even">
<td><strong>uap10:HostId</strong></td>
<td><p>This value specifies the app ID of the host app for the extension.</p></td>
<td>An alphanumeric string between 1 and 255 characters in length. Must begin with an alphabetic character.</td>
<td>No</td>
<td></td>
</tr>
<tr class="odd">
<td><strong>uap10:Parameters</strong></td>
<td><p>Contains command line parameters to pass to the extension. Only supported for desktop apps that have package identity.</p></td>
<td>A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end. </td>
<td>No</td>
<td></td>
</tr>
</tbody>
</table>

 

### Child Elements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Child Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><a href="element-uap-appservice.md">uap:AppService</a> </td>
<td><p>Declares an app extensibility point of type <strong>windows.appService</strong>. Application Contracts are a way for an app to invoke a background task belonging to another app; or for a background task invoked to service an app contract a way to communicate with its caller.</p></td>
</tr>
<tr class="even">
<td><a href="element-uap-appointmentsprovider.md">uap:AppointmentsProvider</a> </td>
<td><p>Declares an app extensibility point of type <strong>windows.appointmentsProvider</strong>.</p></td>
</tr>
<tr class="odd">
<td><a href="element-uap-autoplaycontent.md">uap:AutoPlayContent</a> </td>
<td><p>Declares an app extensibility point of type <strong>windows.autoPlayContent</strong>. The app provides the specified AutoPlay content actions.</p></td>
</tr>
<tr class="even">
<td><a href="element-uap-autoplaydevice.md">uap:AutoPlayDevice</a> </td>
<td><p>Declares an app extensibility point of type <strong>windows.autoPlayDevice</strong>. The app provides the specified AutoPlay device actions.</p></td>
</tr>
<tr class="odd">
<td><a href="element-uap-dialprotocol.md">uap:DialProtocol</a> </td>
<td><p>Declares an app extensibility point of type <strong>windows.dialProtocol</strong>.</p></td>
</tr>
<tr class="even">
<td><a href="element-uap-fileopenpicker.md">uap:FileOpenPicker</a> </td>
<td><p>Declares an app extensibility point of type <strong>windows.fileOpenPicker</strong>. The app lets the user choose and open the specified types of files.</p></td>
</tr>
<tr class="odd">
<td><a href="element-uap-filesavepicker.md">uap:FileSavePicker</a> </td>
<td><p>Declares an app extensibility point of type <strong>windows.fileSavePicker</strong>. The app lets the user choose the file name, extension, and storage location for the specified types of files.</p></td>
</tr>
<tr class="even">
<td><a href="element-uap-filetypeassociation.md">uap:FileTypeAssociation</a> </td>
<td><p>Declares an app extensibility point of type <strong>windows.fileTypeAssociation</strong>. A file type association indicates that the app is registered to handle files of the specified types.</p></td>
</tr>
<tr class="odd">
<td><a href="element-uap-mediaplayback.md">uap:MediaPlayback</a> </td>
<td><p>Declares an app extensibility point of type <strong>mediaPlayback</strong> so that your app can declare that it performs video transcoding.</p></td>
</tr>
<tr class="even">
<td><a href="element-uap-protocol.md">uap:Protocol</a> </td>
<td><p>Declares an app extensibility point of type <strong>windows.protocol</strong>. A URI association indicates that the app is registered to handle URIs with the specified scheme.</p></td>
</tr>
<tr class="odd">
<td><a href="element-uap-sharetarget.md">uap:ShareTarget</a> </td>
<td><p>Declares an app extension point of type <strong>windows.shareTarget</strong>. The app can share the specified types of files.</p></td>
</tr>
<tr class="even">
<td><a href="element-uap-voipcall.md">uap:VoipCall</a> </td>
<td><p>Declares an app extensibility point of type <strong>voipCall</strong> so that your app can declare that it can perform an upgrade from a cellular call to a VoIP video call, and/or whether it is a VoIP app that supports dialing phone numbers directly.</p></td>
</tr>
<tr class="odd">
<td><a href="element-uap-webaccountprovider.md">uap:WebAccountProvider</a> </td>
<td><p>Declares an app extensibility point of type <strong>windows.webAccountProvider</strong>.</p></td>
</tr>
</tbody>
</table>

 

### Parent Elements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parent Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><a href="element-1-extensions.md">Extensions (type: CT_ApplicationExtensions)</a> </td>
<td><p>Defines one or more extensibility points for the app.</p></td>
</tr>
</tbody>
</table>

 

## Remarks

For most types of extensions, Extension@ResourceGroup must match Application@ResourceGroup (if Application@ResourceGroup is omitted then Extension@ResourceGroup should be omitted also).

For a UI-based contract: if Extension@ResourceGroup is not specified then it will be implicitly grouped with the Application; if Extension@ResourceGroup does not match Application@ResourceGroup then the manifest will fail schema validation.

If Extension@ResourceGroup is not specified for a background task, or for a contract that is based on a background task, it will be associated with a default group for all background tasks. Background task contracts are allowed to specify the same values as Application@ResourceGroup.

For the following Extensions, Extension@ResourceGroup allows the background task that is run to be grouped into different processes which will be resource- and lifecycle-managed independently of other groups: windows.backgroundTasks, windows.appServices, windows.preinstalledConfigTask, and windows.updateTask.

For example, if the manifest had these three entries.

```XML
        <Extension Category="windows.backgroundTasks" EntryPoint="Fabrikam.BackgroundTask" ResourceGroup="Group1">
          <BackgroundTasks>
            <Task Type="timer"/>
          </BackgroundTasks>
        </Extension>
        <Extension Category="windows.backgroundTasks" EntryPoint="Fabrikam.BackgroundTask2" ResourceGroup="Group2">
          <BackgroundTasks>
            <Task Type="controlChannel"/>
          </BackgroundTasks>
        </Extension>
        <Extension Category="windows.backgroundTasks" EntryPoint="Fabrikam.BackgroundTask3" ResourceGroup="Group2">
          <BackgroundTasks>
            <Task Type="pushNotification"/>
          </BackgroundTasks>
        </Extension>
```

Then the last two background tasks would be activated into the same instance of backgroundtaskhost.exe if they were activated concurrently. However, a separate instance of backgroundtaskhost.exe would be spun up for the first entry because it has a different ResourceGroup.

If no ResourceGroup is specified for an extension then all background tasks are activated into the same instance of backgroundtaskhost.exe.

Additionally if one of these extensions(windows.backgroundTasks, windows.appServices, windows.preinstalledConfigTask, windows.updateTask) specifies the same value of the ResourceGroup attribute of the parent Application element they will be activated in the same process as the UI.

## Requirements

|   | Value |
|--|--|
| **Namespace** | `http://schemas.microsoft.com/appx/manifest/uap/windows10`<br/><br/>`http://schemas.microsoft.com/appx/manifest/uap/windows10/10` (for the **uap10** attributes) |
