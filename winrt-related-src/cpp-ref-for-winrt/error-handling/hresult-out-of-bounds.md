---

description: A type derived from winrt::hresult_error, representing an E_BOUNDS HRESULT error code.
title: winrt::hresult_out_of_bounds struct (C++/WinRT)
dev_langs: ["C++"]

ms.date: 04/25/2018
ms.topic: "language-reference"
keywords: windows 10, uwp, standard, c++, cpp, winrt, projection, api, reference, hresult, error, code, E_BOUNDS
ms.localizationpriority: medium
ms.workload: ["cplusplus"]
---

# winrt::hresult_out_of_bounds struct (C++/WinRT)
A type derived from **winrt::hresult_error**, representing an E_BOUNDS HRESULT error code. Also see the [winrt::hresult_error](hresult-error.md) topic to learn about the members that are also available to **winrt::hresult_out_of_bounds**.

## Syntax
```cppwinrt
struct hresult_out_of_bounds : winrt::hresult_error
```

## Requirements
**Minimum supported SDK:** Windows SDK version 10.0.17134.0 (Windows 10, version 1803)

**Namespace:** winrt

**Header:** %WindowsSdkDir%Include\<WindowsTargetPlatformVersion>\cppwinrt\winrt\base.h (included by default)

## Constructors
|Constructor|Description|
|------------|-----------------|
|[hresult_out_of_bounds::hresult_out_of_bounds constructor](#hresult_out_of_boundshresult_out_of_bounds-constructor)|Initializes a new instance of the **hresult_out_of_bounds** struct with a copy of the input data.|

## hresult_out_of_bounds::hresult_out_of_bounds constructor
Initializes a new instance of the **hresult_out_of_bounds** struct with a copy of the input data.

### Syntax
```cppwinrt
hresult_out_of_bounds() noexcept;
hresult_out_of_bounds(winrt::hstring const& message) noexcept;
hresult_out_of_bounds(winrt::hresult_error::from_abi_t) noexcept
```

### Parameters
`message`
An informative string to help developers to correct the reported error condition.

## See also 
* [winrt namespace](../winrt.md)
* [winrt::hresult_error struct](hresult-error.md)
* [Error handling with C++/WinRT](/windows/uwp/cpp-and-winrt-apis/error-handling)
