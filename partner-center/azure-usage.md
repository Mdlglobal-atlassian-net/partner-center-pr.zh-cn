---
title: 针对最大预定利用率确定 Microsoft Azure 虚拟机大小 | 合作伙伴仪表板
Description: Information on purchasing and managing Azure reservations
author: v-petand
keywords: azure, 预订, 虚拟机, 管理, 利用率, 确定大小
ms.openlocfilehash: 4050780f9d3dc3ad7d3c4ece0d363845ec1efe9c
ms.sourcegitcommit: 034336ae3a697a97a62ad549b8645c836624efaa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2018
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>针对最大预定利用率确定 Microsoft Azure 虚拟机大小 

**适用范围**

-  合作伙伴仪表板
-  Azure 门户
-  云解决方案提供商计划中的合作伙伴

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>确定客户 Azure 预订的虚拟机大小 

代表客户购买 Microsoft Azure 预订时，你将需要选择一个大小能够满足客户计算需求的虚拟机 (VM)。 你可以使用以下方法之一查找此信息：

-   Azure 使用率 API
-   Azure 门户
-   Azure PowerShell
-   Azure 资源管理器 (ARM) API

每种方法的使用说明如下。 购买预订后，预订折扣会自动应用于与预订的属性和数量相匹配的虚拟机。 你不需要将预订分配给虚拟机。

>[!NOTE]
>预订折扣不适用于经典或促销的虚拟机。

>[!IMPORTANT]
>若要正确识别要代表客户购买的虚拟机的类型和大小，你必须使用下述方法之一，因为合作伙伴中心对帐文件中未正确显示虚拟机系列类型。


**使用 Azure 利用率 API 获取虚拟机大小信息**

1.  使用 API 响应中 additionalInfo 的 ServiceType 属性值来标识要购买的虚拟机大小。 

2.  有关详细信息，请参阅[合作伙伴仪表板 API](https://docs.microsoft.com/partner-center/develop/) 中的[获取客户的 Azure 利用率记录](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)。 

**使用 Microsoft Azure 门户获取虚拟机大小信息**

1.  在你的合作伙伴仪表板中，转到**客户**页面。

2.  查找想要购买 Azure 虚拟机预订的客户，然后选择向下箭头以展开客户的信息。 选择 **Microsoft Azure 管理门户**以在 Azure 门户中打开客户的记录。 

3.  从门户菜单中选择**虚拟机**，然后选择你想要为其购买预订的虚拟机。 

4.  在虚拟机的详细信息页面上，查找大小和区域信息，如下所示，并使用此信息在合作伙伴中心购买预订。  

    ![](images/usage1.png)

**使用 Microsoft Azure PowerShell 获取虚拟机大小信息**

使用下图中的信息，以获取你想要为其购买预订的虚拟机的位置和大小。 

![](images/usage2.png)

**使用 Azure 资源管理器 (ARM) API 获取虚拟机大小信息**

1.  使用 ARMClient 或 ARM API，为你想要为其购买预订的虚拟机调用 ARM 客户端。

2.  /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3.  此调用将返回 **vmSize** 和 **location** 的值，如下所示。

    ![](images/usage3.png)
    ![](images/usage4.png)
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>验证 Azure 虚拟机使用情况和预订折扣

代表客户购买 Azure 虚拟机预留实例后，预先为虚拟机空间付款的折扣会自动应用于与客户预订的属性和数量相匹配的虚拟机。 

你可以使用以下方法之一来验证客户的预订利用率，并查看应用了预订折扣的虚拟机：   

-   Azure 门户
-   Azure 利用率 API

每种方法的使用说明如下。

>[!NOTE]
>只有 Azure 利用率 API 会显示折扣所应用于的虚拟机。  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>在 Microsoft Azure 门户中验证客户的预订利用率

1.  在你的合作伙伴仪表板中，转到**客户**页面。

2.  查找想要验证其预订折扣和使用情况的客户，然后选择向下箭头以展开客户的信息。 选择 **Microsoft Azure 管理门户**以在 Azure 门户中打开客户的记录。 

3.  从门户菜单中选择**预订**，然后选择想要检查其使用情况的预订。 

4.  在**概述**页面上，查看预订的利用率图表，其中显示了应用于虚拟机的预订量。 

    >[!NOTE]
    >利用率数据最多可能会延迟 8 小时。
    
    a.  如果预订的利用率为 100%，则客户将实现预订购买可达到的所有可能的节省额。 
    
    b.  如果预订的利用率为 0%，那么折扣未应用于任何虚拟机。 
    
    c.  如果预订的利用率介于 1% 和 99% 之间，则有未使用的权益。 

5.  为了避免这种情况，请在购买之前确定正确的虚拟机大小以满足客户的计算需求。

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>利用 Azure 利用率 API 验证客户的预订利用率

>[!NOTE]
>只有 Azure 利用率 API 会显示折扣所应用于的虚拟机。  

你可以使用 Azure 利用率 API 获取预定利用率数据，以验证客户是否获得了预订折扣并查看折扣应用于的 VM（虚拟机）。 比较示例 A 与示例 B，了解如何验证客户的预定利用率。 

![](images\usage5.png)

-   reservationId 标识用于将折扣应用于虚拟机的 Azure 预定。
-   consumptionMeter 是应用了预订折扣的虚拟机的 MeterId。
-   由于应用了预订折扣，ReservationMeter 会显示 0 美元的成本。 

有关详细信息，请参阅[合作伙伴仪表板 API](https://docs.microsoft.com/partner-center/develop/) 中的[获取客户的 Azure 利用率记录](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)。

>[!IMPORTANT]
>软件（如 Microsoft Windows Server）成本目前未包含在虚拟机预定的价格中，并且在订单记录和发票上显示为单独的行项目。 但是，如果客户拥有 Azure 混合使用权益，则不会应用软件成本。 有关详细信息，请参阅[预留实例中不包含 Windows 软件成本](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)。  

## <a name="azure-reservations-resources"></a>Azure 预订资源
|**如需以下相关信息**   |**请阅读以下内容**    |
|:-----------------------------|:-----------------|
|云解决方案提供商计划中的 Azure 预订概述  | [销售 Microsoft Azure 虚拟机预留实例](azure-reservations.md)
|在合作伙伴仪表板中为客户购买 Azure 预订   |[购买 Azure 预订](azure-reservations-buying.md)
|Azure 预订计费   |[Azure 预订计费](azure-reservations-billing.md)   |
| 在合作伙伴仪表板中管理 Azure 预订 | [在合作伙伴仪表板中管理 Azure 预订](azure-reservations-manage.md)
|在 Azure 门户中购买 Azure 预订 | Azure 帮助中的[为包含 Azure 虚拟机预留实例的虚拟机预先付款](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) |
|在 Azure 门户中管理 Azure 预订   |Azure 帮助中的[管理虚拟机预留实例](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)  |
|使用合作伙伴中心 API 购买 Azure 预订 | 合作伙伴中心开发人员文档中的[购买 Azure 虚拟机预留实例](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)


