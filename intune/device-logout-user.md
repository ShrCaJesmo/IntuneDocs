---
# required metadata

title: Log out the user of an iOS device 
titleSuffix: Microsoft Intune
description: Learn how to log out the current user of an iOS device with Intune."
keywords:
author: ErikjeMS
ms.author: erikje
manager: dougeby
ms.date: 08/27/2018
ms.topic: conceptual
ms.service: microsoft-intune
ms.localizationpriority: high
ms.technology:
ms.assetid: 702bc46c-1a6f-4689-bd53-3b778a447baa

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
#ms.reviewer: coferro
ms.suite: ems
search.appverid: MET150
#ms.tgt_pltfrm:
ms.custom: intune-azure
ms.collection: M365-identity-device-management
---

# Logout the current user on Intune-managed iOS devices


[!INCLUDE [azure_portal](./includes/azure_portal.md)]

The **Logout current user** action logs out the current user on a shared iPad device. 

## Supported platforms

- Windows - Not supported
- Windows Phone - Not supported
- iOS - Supported on iOS 9.3 and later (shared iPad devices only)
- macOS - Not supported
- Android - Not supported

## How to log out the current user

1. Sign into the Azure portal.
2. Choose **More Services** > **Monitoring + Management** > **Intune**.
3. On the **Intune** blade, choose **Devices**.
4. On the **Devices and groups** blade, choose **All devices**.
5. From the list of devices you manage, choose an iOS device, and then choose the **Logout current user** device remote action.

## Next steps

To see the status of the action you just took, on the **Devices and groups** blade, choose **Device Actions**.
