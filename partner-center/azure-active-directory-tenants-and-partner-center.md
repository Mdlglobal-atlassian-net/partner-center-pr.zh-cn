---
title: Azure Active Directory tenants and Partner Center | Partner Center
description: "To create a Partner Center account, your company must have an Azure Active Directory (Azure AD) tenant. Azure AD is Microsoft’s cloud-based directory and identity management service."
author: labrenne
robots: 
ms.openlocfilehash: ab16d167fc978d76c96fc6ef7c1b8eabe26a1ad5
ms.sourcegitcommit: c47f8e765def420017abe290f2f7327eab2cbba7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a>Azure Active Directory tenants and Partner Center  

**Applies to**

-  Partner Center

#<a name="why-you-need-an-azure-ad-tenant"></a>Why you need an Azure AD tenant

We need to link your organization’s Azure AD tenant to your new Partner Center account, so your tenant users can sign in to Partner Center with their Azure AD (Microsoft account) user names and passwords.

If your company already has an Azure AD tenant, you can link it to your Partner Center account. 

**注意**在你决定使用现有的 Azure AD 租户之前，请考虑租户中将需要使用合作伙伴中心的用户数。 If you have users in the tenant who won’t need to work in Partner Center, consider creating a new tenant for only those users who will need to work in Partner Center.

If your company doesn’t already have an Azure AD tenant, you can create one for free during the enrollment process. Select **Create new tenant** on the **Sign in to Azure Active Directory** page. 


## <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a>Not sure if your company already has an Azure AD tenant?

If you’re not sure whether your company has an Azure AD tenant, follow these steps to check. Note that If you have an active subscription to Microsoft Azure or Office 365, you already have an Azure AD tenant.
1.  Sign in to the Azure admin portal at https://ms.portal.azure.com
2.  Select Azure Active Directory from the menu and then select Domain Names.
3.  如果你已经有租户，则将列出你的域名。

##<a name="using-an-existing-tenant"></a>使用现有租户

If you want to use an existing Azure AD tenant but you’re having trouble signing in, find the scenario on the diagram below that best matches your situation and follow the recommended steps. 

![Do you have an Azure AD tenant or do you need to create one?](images/onboardingAADFlow.png)

For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)

# <a name="about-microsoft-azure"></a>About Microsoft Azure

Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters. Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines. 

When you purchase an Azure subscription, you’re essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company’s physical business. To the office building’s owner, your company is a tenant. 

An Azure AD tenant is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365. 

你的租户托管 Azure AD 用户及其相关信息 - 其密码、配置文件数据、权限等。 租户还包含组、应用程序以及关于公司及其安全性的其他信息。 
