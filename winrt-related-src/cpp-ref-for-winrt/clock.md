---

description: A type containing static helper functions for converting a Windows::Foundation::DateTime (that is, a std::chrono::time_point) to and from winrt::file_time, and to and from time_t.
title: winrt::clock struct (C++/WinRT)
dev_langs: ["C++"]

ms.date: 04/10/2018

ms.topic: "language-reference"


keywords: windows 10, uwp, standard, c++, cpp, winrt, projection, api, reference, weak
ms.workload: ["cplusplus"]
---

# winrt::clock struct (C++/WinRT)
A type containing static helper functions for converting a [Windows::Foundation::DateTime](/uwp/api/windows.foundation.datetime) (that is, a [std::chrono::time_point](/cpp/standard-library/time-point-class)) to and from **winrt::file_time**, and to and from [time_t](/cpp/c-runtime-library/reference/time-time32-time64).

**winrt::clock** is *defined* as using the same units as **Windows::Foundation::DateTime** (a signed 64-bit integer of 100-nanosecond intervals since Jan 1 1601). Other C++ standard clocks don't typically define their resolution, and don't use the epoch Jan 1 1601, which is a Windows Runtime/[FILETIME](/windows/win32/api/minwinbase/ns-minwinbase-filetime) epoch.

## Syntax
```cppwinrt
struct clock
```

## Requirements
**Minimum supported SDK:** Windows SDK version 10.0.17134.0 (Windows 10, version 1803)

**Namespace:** winrt

**Header:** %WindowsSdkDir%Include\<WindowsTargetPlatformVersion>\cppwinrt\winrt\base.h (included by default)

## Member type aliases
|Alias name|Type|
|------------|-----------------|
|clock::rep|A synonym for **int64_t**.|
|clock::period|A synonym for **Windows::Foundation::TimeSpan::period**.|
|clock::duration|A synonym for **Windows::Foundation::TimeSpan**.|
|clock::time_point|A synonym for **Windows::Foundation::DateTime**.|

## Member functions
|Function|Description|
|------------|-----------------|
|[clock::now function](#clocknow-function)|Retrieves the current time as a **Windows::Foundation::DateTime**.|
|[clock::from_file_time function](#clockfrom_file_time-function)|Converts a **winrt::file_time** value to a **Windows::Foundation::DateTime**.|
|[clock::from_time_t function](#clockfrom_time_t-function)|Converts a **time_t** value to a **Windows::Foundation::DateTime**.|
|[clock::to_file_time function](#clockto_file_time-function)|Converts a **Windows::Foundation::DateTime** value to a **winrt::file_time**.|
|[clock::to_time_t function](#clockto_time_t-function)|Converts a **Windows::Foundation::DateTime** value to a **time_t**.|

## clock::now function
Retrieves the current time as a **Windows::Foundation::DateTime**.

### Syntax
```cppwinrt
static Windows::Foundation::DateTime now() noexcept;
```

### Return value 
The current time as a **Windows::Foundation::DateTime**.

## clock::from_file_time function
Converts a **winrt::file_time** value to a **Windows::Foundation::DateTime**.

### Syntax
```cppwinrt
static Windows::Foundation::DateTime from_file_time(winrt::file_time const& time) noexcept;
```

### Parameters
`time`
A **winrt::file_time** value to convert to a **Windows::Foundation::DateTime**.

### Return value 
The **winrt::file_time** value converted into a **Windows::Foundation::DateTime**.

## clock::from_time_t function
Converts a **time_t** value to a **Windows::Foundation::DateTime**.

### Syntax
```cppwinrt
static Windows::Foundation::DateTime from_time_t(time_t time) noexcept;
```

### Parameters
`time`
A **time_t** value to convert to a **Windows::Foundation::DateTime**.

### Return value 
The **time_t** value converted into a **Windows::Foundation::DateTime**.

## clock::to_file_time function
Converts a **Windows::Foundation::DateTime** value to a **winrt::file_time**.

### Syntax
```cppwinrt
static file_time to_file_time(Windows::Foundation::DateTime const& time) noexcept;
```

### Parameters
`time`
A **Windows::Foundation::DateTime** value to convert to a **winrt::file_time**.

### Return value 
The **Windows::Foundation::DateTime** value converted into a **winrt::file_time**.

## clock::to_time_t function
Converts a **Windows::Foundation::DateTime** value to a **time_t**.

### Syntax
```cppwinrt
static time_t to_time_t(Windows::Foundation::DateTime const& time) noexcept;
```

### Parameters
`time`
A **Windows::Foundation::DateTime** value to convert to a **time_t***.

### Return value 
The **Windows::Foundation::DateTime** value converted into a **time_t**.

## See also 
* [winrt namespace](winrt.md)
* [FILETIME](/windows/win32/api/minwinbase/ns-minwinbase-filetime)
* [std::chrono::time_point](/cpp/standard-library/time-point-class)
* [time_t](/cpp/c-runtime-library/reference/time-time32-time64)
* [Windows::Foundation::DateTime](/uwp/api/windows.foundation.datetime)
