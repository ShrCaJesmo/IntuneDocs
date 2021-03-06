---
# required metadata

title: Windows 10 education settings in Microsoft Intune - Azure | Microsoft Docs
description: See a list of all the education settings for Windows 10 devices. Use these settings in a device configuration profile with the Take a Test app, choose how users or students sign in, monitor the screen during the test, and more in Intune.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 07/03/2019
ms.topic: reference
ms.service: microsoft-intune
ms.localizationpriority: medium
ms.technology:
ms.assetid: 6f4de4bd-3dde-4a8d-8e22-46c5d06c3eea

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: kakyker  
ms.suite: ems
search.appverid: MET150
#ms.tgt_pltfrm:
ms.custom: intune-azure
ms.collection: M365-identity-device-management
---

# Configure the Take a Test app on Windows 10 devices using Intune

The Take a Test app lets you securely administer online tests on your classroom's Windows 10 devices. To set up the Take a Test app, you'll need to create a device configuration profile in Intune and configure the secure assessment settings. This article describes the settings you'll find for the Take a Test app. 

After you've configured the profile, assign and deploy it to your students. 

[Take a Test app in Intune](education-settings-configure.md) provides more information on this feature.

## Before you begin

[Create a device configuration profile](education-settings-configure.md#create-a-device-profile).

## Take a test settings
After you create a device configuration profile, go to **Profile type** and select **Secure assessment (Education)**. You'll find the following Take a Test app settings. 


- **Account type**: Choose how users sign in to the test. Your options:
  - Azure AD account
  - Domain account
  - Local account
  - Local guest account: Only available on devices running Windows 10, version 1903 and later.    
- **Account user name**: Enter the user name of the account used with the Take a Test app. You can enter accounts in the following format:
  - `user@contoso.com`
  - `domain\username`
  - `user@contoso.com`
  - `computerName\username`
- **Account name**: To set up a local guest account type, enter the name of the account used with the Take a Test app. The account name will appear as a tile on the sign-in screen. Students click the tile to launch the test.​  
- **Assessment URL**: Enter the URL of the test you want users to take. For more information on getting the URL, see the [Take a Test documentation](https://docs.microsoft.com/education/windows/take-tests-in-windows-10).
- **Printer connection**: Choose **Require** to only allow access to the Take a Test app from devices that are connected to a printer. This setting also makes the app’s print button available to test-takers. **Not configured** allows students to access the app from devices that aren't connected to a printer.​  
- **Screen monitoring**: Choose **Allow** to monitor the screen activity while users are taking a test. **Not configured** prevents you from monitoring the screen during the test.
- **Text suggestions**: Choose **Allow** so test takers can see text suggestions. **Not configured** blocks text suggestions while users are taking a test.

## Next steps

Be sure to [assign the profile](device-profile-assign.md), and [monitor its status](device-profile-monitor.md).
