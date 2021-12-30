---

description: A base class, for you to derive from, that represents a view of a contiguous sequence of elements in an associative collection.
title: winrt::map_view_base struct template (C++/WinRT)
dev_langs: ["C++"]

ms.date: 08/25/2018
ms.topic: "language-reference"
keywords: windows 10, uwp, standard, c++, cpp, winrt, projection, api, reference, map, view, associative, collection
ms.workload: ["cplusplus"]
---

# winrt::map_view_base struct template (C++/WinRT)

A base class from which you can derive to implement your own custom view, or span, of a contiguous sequence of elements in an associative collection. For more info, and code examples, see [Collections with C++/WinRT](/windows/uwp/cpp-and-winrt-apis/collections).

## Syntax
```cppwinrt
template <typename D, typename K, typename V, typename Version = winrt::impl::no_collection_version>
struct map_view_base : iterable_base<D, winrt::Windows::Foundation::Collections::IKeyValuePair<K, V>, Version>
```

### Template parameters
`typename D`
Your derived type name.

`typename K`
The type of the keys in the collection that the **map_view_base** views, or spans.

`typename V`
The type of the values in the collection that the **map_view_base** views, or spans.

`typename Version`
A type that provides versioning policy and services to the collection.

## Requirements
**Minimum supported SDK:** Windows SDK version 10.0.17763.0 (Windows 10, version 1809)

**Namespace:** winrt

**Header:** %WindowsSdkDir%Include\<WindowsTargetPlatformVersion>\cppwinrt\winrt\base.h (included by default)

## Member functions
|Function|Description|
|------------|-----------------|
|[map_view_base::First function](#map_view_basefirst-function)|Retrieves an [**IIterator**](/uwp/api/windows.foundation.collections.iiterator_t_) representing the first element viewed by the **map_view_base** object.|
|[map_view_base::HasKey function](#map_view_basehaskey-function)|Determines whether the specified key belongs to an element viewed by the **map_view_base** object.|
|[map_view_base::Lookup function](#map_view_baselookup-function)|Looks up the element identified by the specified key, and retrieves the corresponding value.|
|[map_view_base::Size function](#map_view_basesize-function)|Retrieves the number of elements viewed by the **map_view_base** object.|
|[map_view_base::Split function](#map_view_basesplit-function)|Splits the map view into two views.|

## Iterators
A **map_view_base** is a range, and that range is defined by internal free functions (each of which retrieves an iterator) that are compatible with standard language features. Because of this, you can enumerate the elements viewed by a **map_view_base** object with a range-based `for` statement.

You can also retrieve an [**IIterator**](/uwp/api/windows.foundation.collections.iiterator_t_) from the [map_view_base::First](#map_view_basefirst-function) function, and use that to iterate through the elements viewed by a **map_view_base** object.

```cppwinrt
...
#include <iostream>
using namespace winrt;
using namespace Windows::Foundation::Collections;
...
struct MyMapView :
    implements<MyMapView, IMapView<winrt::hstring, int>, IIterable<IKeyValuePair<winrt::hstring, int>>>,
    winrt::map_view_base<MyMapView, winrt::hstring, int>
{
    auto& get_container() const noexcept
    {
        return m_values;
    }

private:
    std::map<winrt::hstring, int> m_values{
        { L"AliceBlue", 0xfff0f8ff }, { L"AntiqueWhite", 0xfffaebd7 }
    };
};
...
IMapView<winrt::hstring, int> view{ winrt::make<MyMapView>() };

for (auto const& el : view)
{
    std::wcout << el.Key().c_str() << L", " << std::hex << el.Value() << std::endl;
}

IIterator<IKeyValuePair<winrt::hstring, int>> it{ view.First() };
while (it.HasCurrent())
{
    std::wcout << it.Current().Key().c_str() << L", " << std::hex << it.Current().Value() << std::endl;
    it.MoveNext();
}
```

## map_view_base::First function
Retrieves an [**IIterator**](/uwp/api/windows.foundation.collections.iiterator_t_) representing the first element viewed by the **map_view_base** object.

### Syntax
```cppwinrt
auto First();
```

### Return value
An [**IIterator**](/uwp/api/windows.foundation.collections.iiterator_t_) representing the first element viewed by the **map_view_base** object.

## map_view_base::HasKey function
Determines whether the specified key belongs to an element viewed by the **map_view_base** object.

### Syntax
```cppwinrt
bool HasKey(K const& key) const noexcept;
```

### Parameters
`key`
The key to look for.

### Return value
`true` if an element containing the key is found, otherwise `false`.

## map_view_base::Lookup function
Looks up the element identified by the specified key, and retrieves the corresponding value.

### Syntax
```cppwinrt
V Lookup(K const& key) const;
```

### Parameters
`key`
The key to look up.

### Return value
The value corresponding to the key being looked up if found, otherwise a [winrt::hresult_out_of_bounds](error-handling/hresult-out-of-bounds.md) exception is thrown.

## map_view_base::Size function
Retrieves the number of elements viewed by the **map_view_base** object.

### Syntax
```cppwinrt
uint32_t Size() const noexcept;
```

### Return value
A value representing the number of elements viewed by the **map_view_base** object.

## map_view_base::Split function
Splits the map view into two views.

### Syntax
```cppwinrt
void Split(Windows::Foundation::Collections::IMapView<K, V>& first, Windows::Foundation::Collections::IMapView<K, V>& second) const noexcept;
```

### Parameters
`first`
One half of the original map.

`second`
The second half of the original map.

## See also 
* [winrt namespace](winrt.md)
* [winrt::single_threaded_map function template](single-threaded-map.md)
* [Collections with C++/WinRT](/windows/uwp/cpp-and-winrt-apis/collections)
