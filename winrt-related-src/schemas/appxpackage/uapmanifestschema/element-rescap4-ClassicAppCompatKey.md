---

title: rescap4:ClassicAppCompatKey
description: Registry keys for discovering classic app installations and launching executables.

ms.date: 04/10/2018
ms.topic: reference


keywords: windows 10, uwp, schema, manifest, desktop, extension 
---

# rescap4:ClassicAppCompatKey


## Description
Registry keys for discovering classic app installations and launching executables.

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
<dt><a href="element-rescap4-extension.md">&lt;rescap4:Extension&gt;</a></dt>
<dd>
<dl>
<dt><a href="element-rescap4-ClassicAppCompatKeys.md">&lt;rescap4:ClassicAppCompatKeys&gt;</a></dt>
<dd><b>&lt;rescap4:ClassicAppCompatKey&gt;</b></dd>
</dd>
</dl>
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
<rescap4:ClassicAppCompatKey Name       = A valid registry path in: HKEY_LOCAL_MACHINE\Sofware, HKEY_CURRENT_USER\Software, HKEY_CURRENT_CONFIG\Software, HKLM\Software, HKCU\Software, HKCC\Software. The path is not case sensitive.
                             ValueName? = A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end.
                             ValueType? = One of the following string values: REG_SZ, REG_BINARY, REG_DWORD, REG_QWORD, REG_MULTI_SZ, REG_EXPAND_SZ
                             Value?     = A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end. />

</rescap4:ClassicAppCompatKey>
```

### Key
`?` optional (zero or one)  

## Attributes
| Attribute | Description | Data Type | Required |
|-----------|-------------|-----------|----------|
| Name | The name of the registry path. | A valid registry path in: HKEY_LOCAL_MACHINE\Sofware, HKEY_CURRENT_USER\Software, HKEY_CURRENT_CONFIG\Software, HKLM\Software, HKCU\Software, HKCC\Software. The path is not case sensitive. | Yes |
| ValueName | Value name of a key in the registry path. | A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end. | No |
| ValueType | A value type. | One of the following string values: REG_SZ, REG_BINARY, REG_DWORD, REG_QWORD, REG_MULTI_SZ, REG_EXPAND_SZ | No |
| Value | The value of the ValueName. | A string between 1 and 32767 characters in length with a non-whitespace character at its beginning and end. | No |

## Child Elements
None.

## Requirements

|               | Value                                                       |
|---------------|-------------------------------------------------------------|
| **Namespace** | `http://schemas.microsoft.com/appx/manifest/foundation/windows10/restrictedcapabilities/4` |