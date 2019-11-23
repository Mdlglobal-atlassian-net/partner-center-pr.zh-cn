---
title: Office 365 Partner Advisory - Microsoft 365 Voice in CSP | Partner Center
description: PSTN services in some countries may be subject to special tax and regulatory requirements that may affect partner order and invoicing.
ms.topic: article
ms.date: 11/04/2019
author: maggiepuccievans
ms.author: evansma
keywords: Office, O365, PSTN services, taxes, requirements, invoice, invoicing
ms.localizationpriority: medium
ms.openlocfilehash: b6359a49503237e72c8cffdb5758bdd418910306
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384812"
---
# <a name="office-365-partner-advisory-microsoft-365-voice-in-csp"></a>Office 365 Partner Advisory: Microsoft 365 Voice in CSP

**适用于**

- 合作伙伴中心  

Public Switched Telephone Network (PSTN) services in some countries may be subject to special tax and regulatory requirements that may affect partner order and invoicing.  In the United States, Puerto Rico, and Canada, Skype for Business PSTN and Microsoft 365 Voice services are subject to special tax and regulatory requirements. In the United States and Puerto Rico, Microsoft prices PSTN services as tax-inclusive.  Unique PSTN taxes and regulations will affect Office 365 partners transacting Microsoft 365 Voice products.  如果合作伙伴标记了 Microsoft PSTN 服务的价格，则可能有责任计算和汇寄 PSTN 税款和费用。

## <a name="partner-recommendations"></a>Partner Recommendations

咨询税务和法律顾问，了解组织对 PSTN 服务法规、税务和费用以及其他潜在义务的责任。

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Invoice Presentation and Partner Reconciliation File

CSP invoices and CSP reconciliation files in the United States, Puerto Rico and Canada which include Skype for Business PSTN and Microsoft 365 Voice services will provide separate line items for the PSTN and non-PSTN components.

Additionally, CSP invoices will display the following footnote:

* The price displayed is a charge for Audio Conferencing and Calling Plan Services.  Any applicable transactional taxes are charged exclusively of the amount shown except for sales made within the United States.  In the U.S., the price displayed is tax inclusive as it includes a charge for the Calling Plan and Audio Conferencing Services and a charge for the taxes and fees we are required to charge.  Audio Conferencing and Calling Plan Services are serviced by the Microsoft Affiliate authorized to provide them.  See [Microsoft Volume Licensing](https://go.microsoft.com/fwlink/?LinkId=690247) for details.

## <a name="reconciliation-file-example"></a>Reconciliation File Example

Office 365 Enterprise E5 presents on reconciliation file as two line items with identical names and identical IDs, but each line item has a unique unit price (example: $28.40 and $2.00). 这可区分 Office 365 产品/服务的 Skype for Business PSTN 会议组件，以便正确征税。

**Partner Reconciliation example #1 (select columns):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 企业版 E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |周期费用   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 企业版 E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |周期费用   |2.00   |

**Partner Reconciliation example #2**

Microsoft 365 Business Voice available in Canada has additional PSTN taxable components that are consolidated on CSP Invoice (similar to Office 365 E5, two line items are presented, one for PSTN components and the other for non-PSTN components).  The CSP Reconciliation file for Microsoft 365 Business Voice will display all PSTN taxable components individually (individual PSTN components will not be consolidated in .CSV or API tool).  The summation of order details and billed amounts for customers found in the reconciliation file will match the CSP Invoice.

## <a name="additional-resources"></a>其他资源
For more details, visit the [Microsoft 365 for Partners](https://drumbeat.office.com/Pages/home2016.aspx) site.

