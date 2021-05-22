---

description: A helper function that copies to a C++/WinRT object from a handle, or from a raw pointer.
title: winrt::copy_from_abi function (C++/WinRT)
dev_langs: ["C++"]

ms.date: 04/11/2018
ms.topic: "language-reference"
keywords: windows 10, uwp, standard, c++, cpp, winrt, projection, api, reference, copy_from_abi
ms.localizationpriority: medium
ms.workload: ["cplusplus"]
---

# winrt::copy_from_abi function (C++/WinRT)
A helper function that copies to a [C++/WinRT](/windows/uwp/cpp-and-winrt-apis/intro-to-using-cpp-with-winrt) object from a handle, or from a raw pointer. Clears the C++/WinRT object, or decrements the reference count on any currently referenced interface, copies the parameter, and begins managing the handle or interface pointed to by it (which includes incrementing any reference count on the parameter). For more info, and code examples, see [Interop between C++/WinRT and the ABI](/windows/uwp/cpp-and-winrt-apis/interop-winrt-abi).

## Syntax

```cppwinrt
template <typename T, typename V, typename =
std::enable_if_t<!std::is_base_of_v<winrt::Windows::Foundation::IUnknown, T>>>
void copy_from_abi(T& object, V&& value);

void copy_from_abi(winrt::hstring& object, void* value);

void copy_from_abi(winrt::Windows::Foundation::IUnknown& object, void* value) noexcept;
```

### Parameters
`object`
A C++/WinRT object to operate on.

`value`
A handle, or a raw pointer to a target whose lifetime should be managed by the C++/WinRT object. In the case of the `IUnknown&, void*` overload, the function calls **AddRef** on *value*.

## Requirements
**Minimum supported SDK:** Windows SDK version 10.0.17134.0 (Windows 10, version 1803)

**Namespace:** winrt

**Header:** %WindowsSdkDir%Include\<WindowsTargetPlatformVersion>\cppwinrt\winrt\base.h (included by default)

## See also 
* [winrt namespace](winrt.md)
* [winrt::com_ptr struct template](com-ptr.md)
* [winrt::hstring struct](hstring.md)
* [Windows::Foundation::IUnknown struct](windows-foundation-iunknown.md)
* [Interop between C++/WinRT and the ABI](/windows/uwp/cpp-and-winrt-apis/interop-winrt-abi)
