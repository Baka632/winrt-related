---
description: Specifies an image used in the toast template.
Search.Product: eADQiWindows 10XVcnh
title: image (Toast schema)
ms.assetid: 29c4061d-bfe4-4f24-b484-2df25a48e98e

keywords: windows 10, uwp, schema, toast notifications


ms.topic: reference
ms.date: 04/05/2017
---

# image (Toast schema)

Specifies an image used in the toast template.

## Element hierarchy

<dl>
<dt><a href="element-toast.md">&lt;toast&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-visual.md">&lt;visual&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-binding.md">&lt;binding&gt;</a></dt>
<dd><b>&lt;image&gt;</b></dd>
</dl>
</dd>
</dl>
</dd>
</dl>

## Syntax

``` syntax
<image id             = integer
       src            = string
       alt?           = string
       addImageQuery? = boolean 
       placement? = "appLogoOverride" | "hero"/>
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
<td><strong>addImageQuery</strong></td>
<td><p>Set to &quot;true&quot; to allow Windows to append a query string to the image URI supplied in the toast notification. Use this attribute if your server hosts images and can handle query strings, either by retrieving an image variant based on the query strings or by ignoring the query string and returning the image as specified without the query string. This query string specifies scale, contrast setting, and language; for instance, a value of</p>
<p>&quot;www.website.com/images/hello.png&quot;</p>
<p>given in the notification becomes</p>
<p>&quot;www.website.com/images/hello.png?ms-scale=100&amp;ms-contrast=standard&amp;ms-lang=en-us&quot;</p></td>
<td>boolean</td>
<td>No</td>
<td>false</td>
</tr>
<tr class="even">
<td><strong>alt</strong></td>
<td><p>A description of the image, for users of assistive technologies.</p></td>
<td>string</td>
<td>No</td>
<td>None</td>
</tr>
<tr class="odd">
<td><strong>id</strong></td>
<td><p>The image element in the toast template that this image is intended for. If a template has only one image, then this value is 1. The number of available image positions is based on the template definition.</p></td>
<td>integer</td>
<td>Yes</td>
<td>None</td>
</tr>
<tr class="even">
<td><strong>src</strong></td>
<td><p>The URI of the image source, using one of these protocol handlers:</p>
<ul>
<li><p>http:// or https://</p>
<p>A web-based image.</p></li>
<li><p>ms-appx:///</p>
<p>An image included in the app package.</p></li>
<li><p>ms-appdata:///local/</p>
<p>An image saved to local storage.</p></li>
<li><p>file:///</p>
<p>A local image. (Supported only for desktop apps. This protocol cannot be used by UWP apps.)</p></li>
</ul></td>
<td>string</td>
<td>Yes</td>
<td>None</td>
</tr>
<tr class="even">
<td><strong>placement</strong></td>
<td><p>The placement of the image.</p> <ul><li>"appLogoOverride" - The image replaces your app's logo in the toast notification.</li><li>"hero" - The image is displayed as a hero image. </li></ul><p>For more information, see <a href="/windows/apps/design/shell/tiles-and-notifications/adaptive-interactive-toasts">Toast content</a>.</p></li>
</ul></td>
<td>string</td>
<td>No</td>
<td>None</td>
</tr>
</tbody>
</table>

 

### Child Elements

None.

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
<td><a href="element-binding.md">binding</a> </td>
<td><p>Specifies the toast template. Note that only one binding element can be included in a toast notification.</p></td>
</tr>
</tbody>
</table>

## See also

* [Toast content](/windows/apps/design/shell/tiles-and-notifications/adaptive-interactive-toasts)
* [Notifications Visualizer](/windows/apps/design/shell/tiles-and-notifications/notifications-visualizer)
 



 

 



