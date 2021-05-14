---


title: Element Hierarchy (app installer file schema)
description: The following list summarizes the allowed hierarchies for the App Installer file schema, starting with the outermost element at the top.
ms.topic: reference
ms.date: 10/10/2017


keywords: windows 10, uwp, app installer, AppInstaller, sideload, related set, optional packages
---

# Element Hierarchy (app installer file schema)

The following list summarizes the allowed hierarchies for the App Installer file schema, starting with the outermost element at the top.

-   [AppInstaller](element-appinstaller.md)
    -   [MainBundle](element-main-bundle.md)     
    -   [MainPackage](element-main-package.md)   
    -   [OptionalPackages](element-optional-packages.md)  
        -   [Bundle](element-bundle.md)  
        -   [Package](element-package.md)
    -   [RelatedPackages](element-related-packages.md)  
        -   [Bundle](element-bundle.md) 
        -   [Package](element-package.md)
    -   [Dependencies](element-dependencies.md)  
        -   [Bundle](element-bundle.md)  
        -   [Package](element-package.md)
    -   [UpdateSettings](element-update-settings.md) 
        -   [OnLaunch](element-onlaunch.md)
        -   [AutomaticBackgroundTask](element-automatic-background-task.md)
        -   [ForceUpdateFromAnyVersion](element-force-update-from-any-version.md)
