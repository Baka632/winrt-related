---
description: A helper function that retrieves a pointer to a C++/WinRT object's underlying IUnknown interface.
title: winrt::get_abi function (C++/WinRT)
dev_langs: ["C++"]
ms.date: 04/10/2018
ms.topic: "language-reference"
keywords: windows 10, uwp, standard, c++, cpp, winrt, projection, api, reference, IUnknown
ms.workload: ["cplusplus"]
---

# winrt::get_abi function (C++/WinRT)

A helper function that retrieves a pointer to a C++/WinRT object's underlying [IUnknown interface](/windows/win32/api/unknwn/nn-unknwn-iunknown). For more info, and code examples, see [Interop between C++/WinRT and the ABI](/windows/uwp/cpp-and-winrt-apis/interop-winrt-abi).

## Syntax
```cppwinrt
template <typename T, typename = std::enable_if_t<!std::is_base_of_v<winrt::Windows::Foundation::IUnknown, T>>>
auto get_abi(T const& object) noexcept;

inline void* get_abi(winrt::Windows::Foundation::IUnknown const& object) noexcept;

inline void* get_abi(winrt::hstring const& object) noexcept;

template <typename T>
static auto get_abi(winrt::array_view<T> object) noexcept;

template <typename T>
auto get_abi(winrt::param::async_iterable<T> const& object) noexcept;

template <typename K, typename V>
auto get_abi(winrt::param::async_map_view<K, V> const& object) noexcept;

template <typename T>
auto get_abi(winrt::param::async_vector_view<T> const& object) noexcept;

template <typename T>
auto get_abi(winrt::com_ptr<T> const& object) noexcept;

template <typename T>
auto get_abi(winrt::param::iterable<T> const& object) noexcept;

template <typename K, typename V>
auto get_abi(winrt::param::map<K, V> const& object) noexcept;

template <typename K, typename V>
auto get_abi(winrt::param::map_view<K, V> const& object) noexcept;

template <typename T>
auto get_abi(winrt::param::vector<T> const& object) noexcept;

template <typename T>
auto get_abi(winrt::param::vector_view<T> const& object) noexcept;
```

### Parameters
`object`
The C++/WinRT object whose **IUnknown** interface pointer to retrieve.

### Return value 
A pointer to the **IUnknown** interface of the C++/WinRT object.

## Requirements
**Minimum supported SDK:** Windows SDK version 10.0.17134.0 (Windows 10, version 1803)

**Namespace:** winrt

**Header:** %WindowsSdkDir%Include\<WindowsTargetPlatformVersion>\cppwinrt\winrt\base.h (included by default)

## See also 
* [winrt namespace](winrt.md)
* [winrt::put_abi function](put-abi.md)
* [Interop between C++/WinRT and the ABI](/windows/uwp/cpp-and-winrt-apis/interop-winrt-abi)
