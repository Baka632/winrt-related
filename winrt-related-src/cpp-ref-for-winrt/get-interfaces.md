---

description: A helper function that retrieves an array containing the identifiers of the interfaces that are implemented by a C++/WinRT object.
title: winrt::get_interfaces function (C++/WinRT)
dev_langs: ["C++"]

ms.date: 05/01/2018
ms.topic: "language-reference"
keywords: windows 10, uwp, standard, c++, cpp, winrt, projection, api, reference, interface, identifiers, IInspectable, GetIids
ms.localizationpriority: medium
ms.workload: ["cplusplus"]
---

# winrt::get_interfaces function (C++/WinRT)
A helper function that retrieves an array containing the identifiers of the interfaces that are implemented by a [C++/WinRT](/windows/uwp/cpp-and-winrt-apis/intro-to-using-cpp-with-winrt) object. These are the same identifiers that are returned from a call to [**IInspectable::GetIids**](/windows/win32/api/inspectable/nf-inspectable-iinspectable-getiids).

Also see the [implements::find_interface](./implements.md#implementsfind_interface-function) and [implements::get_local_iids](./implements.md#implementsget_local_iids-function) functions.

## Syntax
```cppwinrt
inline winrt::com_array<GUID> get_interfaces(winrt::Windows::Foundation::IInspectable const& object);
```

### Parameters
`object`
A C++/WinRT object to operate on.

### Return value 
A [**winrt::com_array**](com-array.md) containing the interface identifiers.

## Requirements
**Minimum supported SDK:** Windows SDK version 10.0.17134.0 (Windows 10, version 1803)

**Namespace:** winrt

**Header** %WindowsSdkDir%Include\<WindowsTargetPlatformVersion>\cppwinrt\winrt\base.h (included by default)

## See also 
* [winrt namespace (C++/WinRT)](winrt.md)
* [winrt::com_array struct template](com-ptr.md)
* [winrt::implements::find_interface member function](./implements.md#implementsfind_interface-function)
* [winrt::implements::get_local_iids member function](./implements.md#implementsget_local_iids-function) 
* [IInspectable::GetIids](/windows/win32/api/inspectable/nf-inspectable-iinspectable-getiids)