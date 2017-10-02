---
title: Simplify device setup with Windows Autopilot | Partner Center
description: Add a Windows AutoPilot deployment profile in Partner Center to simplify device setup with Windows Autopilot
author: KPacquer
keywords: autopilot, windows autopilot, microsoft autopilot, zero-touch deployment, oobe, login screens
ms.openlocfilehash: 72cf8a8361a12c545501a452788d231f930c4928
ms.sourcegitcommit: d9f3e4e8115c0ad44f97041d352b703cda7ba9e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="simplify-device-setup-with-windows-autopilot"></a>Simplify device setup with Windows Autopilot 

Windows Autopilot streamlines and secures device setup for new Windows 10 Pro devices from first boot in only a few steps. To learn more, see [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).

## <a name="features"></a>Features

*  **Disable local administrator permissions** for the end users setting up devices
*  **Show an organization's login page**. The organization can predefine a logon page that adds the device as a work device, and joins the device with Azure Active Directory.
*  **Enroll the device into a Mobile Device Manager (MDM)**, for example: Microsoft Intune, after OOBE is complete.
*  **Streamline the out-of-box experience (OOBE)** to use just the steps and decisions required, using a Windows AutoPilot Deployment profile. 

## <a name="requirements"></a>Requirements

*  Devices pre-installed with Windows 10 Pro Creators Update (version 1703 or later) or Windows 10 Pro for Advanced PCs.
*  Device identifier known as a hardware hash (128 HWH or 4k HWH), which is typically provided by an OEM. You'll use identifiers to assign organization profiles in Partner Center. After September 2017 you will no longer need the hardware hash. 
*  The devices must have access to the internet. When the device can’t connect, it shows the default Windows out-of-box experience (OOBE) screens.
*  Enrolling the device into an MDM requires Azure Active Directory Premium.

## <a name="add-organization-login-pages-to-oobe"></a>Add organization login pages to OOBE

To add organization-specific pages, add the devices into your organization’s [Azure AD directory](https://go.microsoft.com/fwlink/?linkid=848958) and create login pages.


## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a>Remove Windows pages from OOBE with a Windows AutoPilot deployment profile

### <a name="examples-of-settings-in-a-windows-autopilot-deployment-profile"></a>Examples of settings in a Windows AutoPilot deployment profile
*  Skip Privacy Settings in setup
*  Disable local admin account in setup
*  Automatically skip pages in setup
   *  Automatically select setup for work or school
   *  Skip Cortana, OneDrive, and OEM registration setup pages

### <a name="add-devices-and-apply-a-profile"></a>Add devices and apply a profile

In Partner Center, you can create a Windows AutoPilot deployment profile and apply it to a list of the devices.

To configure devices, upload a list of the devices into Partner Center, create a profile that applies to the devices, and apply it.

1.  Add the list of devices into Partner Center.

    Sales agents and admin agents have access to add the list of devices into Partner Center.
    
    Indirect resellers can work with their indirect provider to add this.

    a.  Create a .csv file using the PowerShell script from the topic: [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot). This .csv file contains device info including the serial number, OEM name, model name, product ID and device identifier. 

    b.  From the Partner Center dashboard, go to **Customers** > select the customer that’s receiving the devices > **Devices > Add devices**.

    c.  Name the batch of devices, for example, “Contoso Sales Department PCs – April 2017 order.” 

    d.  Click **Browse** > select the device info file > **Validate**.

    **Note:** If you get an error message after trying to upload the .csv file, check the format of the file. After August, you can use the Hardware Hash only, or the OEM name, serial number, and model in that column order, or the Windows Product ID. You can also use the sample .csv file provided from the link next to **Add devices**.

2.  Create a profile that you can apply to the devices. (Only admin agents have access to create and apply profiles in Partner Center.)

    a.  From **Devices**, click **Add new profile**.

    b.  Name the profile, for example, “Contoso Desktop Profile – Skip All OOBE”.

    c.  Configure the OOBE settings. For example, check **Skip Express Settings in setup**.

    d.  Click **Submit**.

3.  Apply the profile.

    a.  From **Devices**, in the **Assign and delete devices** pane, select the devices that you want to configure. To select an entire batch, click the checkbox next to the batch name (for example, “Contoso Sales Department PCs – March 2017 order”).

    b.  Click **Apply profile**, and select the profile (for example, “Contoso Desktop Profile – Skip All OOBE”). The devices will show the profile in the Profile column.

4.  Optional: Test to see that your profile works.

    a.  Connect a device to the network, and turn it on.

    b.  Verify that the appropriate OOBE screens (if any) appear.

    c.  To prepare the device for a new user, complete the OOBE experience, then reset the device to its factory default settings.


## <a name="to-update-or-delete-a-profile"></a>To update or delete a profile 

Once you’ve assigned a profile to a device, you can update it, even if you’ve already given the device to your customer. When the device connects to the internet, it downloads the latest version of your profile during the OOBE process. If your customer restores their device to its factory default settings, the device will again download the latest updates to your profile. 

### <a name="you-can-remove-a-profile-from-a-device"></a>You can remove a profile from a device
1. Select the device (or batch of devices) you want to remove the profile from. 

2. In **Assign and delete devices** pane, select **Remove profile**.

3. Go to the profile you want to remove and delete it. The profile will be deleted from all devices.

From **Devices**, select the profile. From here, you can modify the existing settings.

## <a name="windows-autopilot-eula-dismissal--important-information"></a>Windows Autopilot EULA 解除 - 重要信息

使用此工具，你可以在为客户管理的设备上配置 Windows 的单个安装。 如果客户授权你进行此操作，你可以选择不显示或隐藏在设置 Windows 时向用户正常显示的某些设置屏幕，包括 EULA 接受屏幕。 

使用此功能，即表明你同意不显示或隐藏专为用户提供通知或条款接受的任何屏幕，意味着你已从客户方获得隐藏条款的充分许可和授权，并且你已代表你的客户（组织或单个用户，根据具体情况而定）同意所有通知并接受所有对该客户适用的条款。 这包括你同意在不使用此工具禁止显示或隐藏时将向用户呈现的许可证的条款和条件或通知。 如果你的客户尚未从 Microsoft 或其许可的分销商处获取有效的软件许可，则该客户不得在这些设备上使用该 Windows 软件。


