---
title: Usage-based reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand usage-based reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 3cf0f20ed266fa5302264ef07092d47c050a9206
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389775"
---
# <a name="usage-based-file-fields"></a><span data-ttu-id="962d1-103">基于使用情况的文件字段</span><span class="sxs-lookup"><span data-stu-id="962d1-103">Usage-based file fields</span></span>

<span data-ttu-id="962d1-104">适用范围：</span><span class="sxs-lookup"><span data-stu-id="962d1-104">Applies to:</span></span>

- <span data-ttu-id="962d1-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="962d1-105">Partner Center</span></span>
- <span data-ttu-id="962d1-106">Microsoft Cloud for US Government 合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="962d1-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="962d1-107">To reconcile your charges against a customer's usage, compare the **ResellerID**, **ResellerName**, and **ResellerBillableAccount** from the reconciliation file with the **Customer name** and **Subscription ID** from Partner Center.</span><span class="sxs-lookup"><span data-stu-id="962d1-107">To reconcile your charges against a customer's usage, compare the **ResellerID**, **ResellerName**, and **ResellerBillableAccount** from the reconciliation file with the **Customer name** and **Subscription ID** from Partner Center.</span></span>

## <a name="fields-in-usage-based-reconciliation-files"></a><span data-ttu-id="962d1-108">Fields in usage-based reconciliation files</span><span class="sxs-lookup"><span data-stu-id="962d1-108">Fields in usage-based reconciliation files</span></span>

<span data-ttu-id="962d1-109">以下字段说明已使用的服务和费率。</span><span class="sxs-lookup"><span data-stu-id="962d1-109">The following fields explain which services were used and the rate.</span></span>

| <span data-ttu-id="962d1-110">列</span><span class="sxs-lookup"><span data-stu-id="962d1-110">Column</span></span> | <span data-ttu-id="962d1-111">描述</span><span class="sxs-lookup"><span data-stu-id="962d1-111">Description</span></span> | <span data-ttu-id="962d1-112">Sample value(s)</span><span class="sxs-lookup"><span data-stu-id="962d1-112">Sample value(s)</span></span> |
| ------ | ----------- | ------------ |
| <span data-ttu-id="962d1-113">PartnerID</span><span class="sxs-lookup"><span data-stu-id="962d1-113">PartnerID</span></span> | <span data-ttu-id="962d1-114">Partner identifier, in GUID format.</span><span class="sxs-lookup"><span data-stu-id="962d1-114">Partner identifier, in GUID format.</span></span> | <span data-ttu-id="962d1-115">*DA41BC5F-C52D-4464-8A8D-8C8DCC43503B*</span><span class="sxs-lookup"><span data-stu-id="962d1-115">*DA41BC5F-C52D-4464-8A8D-8C8DCC43503B*</span></span> |
| <span data-ttu-id="962d1-116">PartnerName</span><span class="sxs-lookup"><span data-stu-id="962d1-116">PartnerName</span></span> | <span data-ttu-id="962d1-117">Partner name.</span><span class="sxs-lookup"><span data-stu-id="962d1-117">Partner name.</span></span> | <span data-ttu-id="962d1-118">*Contoso, Ltd.*</span><span class="sxs-lookup"><span data-stu-id="962d1-118">*Contoso, Ltd.*</span></span> |
| <span data-ttu-id="962d1-119">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="962d1-119">PartnerBillableAccountID</span></span> | <span data-ttu-id="962d1-120">Partner account identifier.</span><span class="sxs-lookup"><span data-stu-id="962d1-120">Partner account identifier.</span></span> | <span data-ttu-id="962d1-121">*1010578050*</span><span class="sxs-lookup"><span data-stu-id="962d1-121">*1010578050*</span></span> |
| <span data-ttu-id="962d1-122">CustomerName</span><span class="sxs-lookup"><span data-stu-id="962d1-122">CustomerName</span></span> | <span data-ttu-id="962d1-123">Customer's organization name, as reported in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="962d1-123">Customer's organization name, as reported in Partner Center.</span></span> <span data-ttu-id="962d1-124">*Very important for reconciling the invoice with your system information.*</span><span class="sxs-lookup"><span data-stu-id="962d1-124">*Very important for reconciling the invoice with your system information.*</span></span> | <span data-ttu-id="962d1-125">*Test customer*</span><span class="sxs-lookup"><span data-stu-id="962d1-125">*Test customer*</span></span> |
| <span data-ttu-id="962d1-126">MPNID</span><span class="sxs-lookup"><span data-stu-id="962d1-126">MPNID</span></span> | <span data-ttu-id="962d1-127">MPN identifier of the CSP partner.</span><span class="sxs-lookup"><span data-stu-id="962d1-127">MPN identifier of the CSP partner.</span></span> | <span data-ttu-id="962d1-128">*4390934*</span><span class="sxs-lookup"><span data-stu-id="962d1-128">*4390934*</span></span> |
| <span data-ttu-id="962d1-129">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="962d1-129">ResellerMPNID</span></span> | <span data-ttu-id="962d1-130">MPN identifier of the reseller of record for the subscription.</span><span class="sxs-lookup"><span data-stu-id="962d1-130">MPN identifier of the reseller of record for the subscription.</span></span> <span data-ttu-id="962d1-131">For more information, see [how to itemize by partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner).</span><span class="sxs-lookup"><span data-stu-id="962d1-131">For more information, see [how to itemize by partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner).</span></span> | <span data-ttu-id="962d1-132">*4390934*</span><span class="sxs-lookup"><span data-stu-id="962d1-132">*4390934*</span></span> |
| <span data-ttu-id="962d1-133">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="962d1-133">InvoiceNumber</span></span> | <span data-ttu-id="962d1-134">显示指定交易所在的发票号码。</span><span class="sxs-lookup"><span data-stu-id="962d1-134">Invoice number where the specified transaction appears.</span></span> | <span data-ttu-id="962d1-135">*D020001IVK*</span><span class="sxs-lookup"><span data-stu-id="962d1-135">*D020001IVK*</span></span> |
| <span data-ttu-id="962d1-136">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="962d1-136">ChargeStartDate</span></span> | <span data-ttu-id="962d1-137">Start date of billing cycle, except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span><span class="sxs-lookup"><span data-stu-id="962d1-137">Start date of billing cycle, except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="962d1-138">时间始终是一天的开始，即 0:00。</span><span class="sxs-lookup"><span data-stu-id="962d1-138">The time is always the beginning of the day, 0:00.</span></span> | <span data-ttu-id="962d1-139">*2/1/2019 0:00*</span><span class="sxs-lookup"><span data-stu-id="962d1-139">*2/1/2019 0:00*</span></span> |
| <span data-ttu-id="962d1-140">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="962d1-140">ChargeEndDate</span></span> | <span data-ttu-id="962d1-141">End date of billing cycle, except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span><span class="sxs-lookup"><span data-stu-id="962d1-141">End date of billing cycle, except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="962d1-142">时间始终是一天的结束，即 23:59。</span><span class="sxs-lookup"><span data-stu-id="962d1-142">The time is always the end of the day, 23:59.</span></span> | <span data-ttu-id="962d1-143">*2/28/2019 23:59*</span><span class="sxs-lookup"><span data-stu-id="962d1-143">*2/28/2019 23:59*</span></span> |
| <span data-ttu-id="962d1-144">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="962d1-144">SubscriptionID</span></span> | <span data-ttu-id="962d1-145">Microsoft 帐单平台中订阅的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="962d1-145">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="962d1-146">May be useful to identify the subscription when contacting support.</span><span class="sxs-lookup"><span data-stu-id="962d1-146">May be useful to identify the subscription when contacting support.</span></span> <span data-ttu-id="962d1-147">Not used for reconciliation.</span><span class="sxs-lookup"><span data-stu-id="962d1-147">Not used for reconciliation.</span></span> <span data-ttu-id="962d1-148">*This is not the same as the **Subscription ID** on the Partner Admin Console.*</span><span class="sxs-lookup"><span data-stu-id="962d1-148">*This is not the same as the **Subscription ID** on the Partner Admin Console.*</span></span> | <span data-ttu-id="962d1-149">*usCBMgAAAAAAAAIA*</span><span class="sxs-lookup"><span data-stu-id="962d1-149">*usCBMgAAAAAAAAIA*</span></span> |
| <span data-ttu-id="962d1-150">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="962d1-150">SubscriptionName</span></span> | <span data-ttu-id="962d1-151">Nickname for the service offering.</span><span class="sxs-lookup"><span data-stu-id="962d1-151">Nickname for the service offering.</span></span> | <span data-ttu-id="962d1-152">*Microsoft Azure*</span><span class="sxs-lookup"><span data-stu-id="962d1-152">*Microsoft Azure*</span></span> |
| <span data-ttu-id="962d1-153">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="962d1-153">SubscriptionDescription</span></span> | <span data-ttu-id="962d1-154">Line of business of the service offering.</span><span class="sxs-lookup"><span data-stu-id="962d1-154">Line of business of the service offering.</span></span> | <span data-ttu-id="962d1-155">*Microsoft Azure*</span><span class="sxs-lookup"><span data-stu-id="962d1-155">*Microsoft Azure*</span></span> |
| <span data-ttu-id="962d1-156">OrderID</span><span class="sxs-lookup"><span data-stu-id="962d1-156">OrderID</span></span> | <span data-ttu-id="962d1-157">Microsoft 帐单平台中订单的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="962d1-157">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="962d1-158">May be useful to identify the subscription when contacting support.</span><span class="sxs-lookup"><span data-stu-id="962d1-158">May be useful to identify the subscription when contacting support.</span></span> <span data-ttu-id="962d1-159">Not used for reconciliation.</span><span class="sxs-lookup"><span data-stu-id="962d1-159">Not used for reconciliation.</span></span> | <span data-ttu-id="962d1-160">*566890604832738111*</span><span class="sxs-lookup"><span data-stu-id="962d1-160">*566890604832738111*</span></span> |
| <span data-ttu-id="962d1-161">ServiceName</span><span class="sxs-lookup"><span data-stu-id="962d1-161">ServiceName</span></span> | <span data-ttu-id="962d1-162">存在问题的 Azure 服务的名称。</span><span class="sxs-lookup"><span data-stu-id="962d1-162">The name of the Azure service in question.</span></span> | <span data-ttu-id="962d1-163">*VIRTUAL MACHINES*</span><span class="sxs-lookup"><span data-stu-id="962d1-163">*VIRTUAL MACHINES*</span></span> |
| <span data-ttu-id="962d1-164">ServiceType</span><span class="sxs-lookup"><span data-stu-id="962d1-164">ServiceType</span></span> | <span data-ttu-id="962d1-165">The specific type of Azure service.</span><span class="sxs-lookup"><span data-stu-id="962d1-165">The specific type of Azure service.</span></span> | <span data-ttu-id="962d1-166">*Service Bus – Individual or Pack*, *SQL Azure database – Business or Web Edition*</span><span class="sxs-lookup"><span data-stu-id="962d1-166">*Service Bus – Individual or Pack*, *SQL Azure database – Business or Web Edition*</span></span> |
| <span data-ttu-id="962d1-167">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="962d1-167">ResourceGUID</span></span> | <span data-ttu-id="962d1-168">所有服务数据和定价结构的特定唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="962d1-168">Specific unique identifier for all the service data and pricing structure.</span></span> | <span data-ttu-id="962d1-169">*DA41BC5F-C52D-4464-8A8D-8C8DCC43503B*</span><span class="sxs-lookup"><span data-stu-id="962d1-169">*DA41BC5F-C52D-4464-8A8D-8C8DCC43503B*</span></span> |
| <span data-ttu-id="962d1-170">ResourceName</span><span class="sxs-lookup"><span data-stu-id="962d1-170">ResourceName</span></span> | <span data-ttu-id="962d1-171">Azure 资源的名称。</span><span class="sxs-lookup"><span data-stu-id="962d1-171">The name of the Azure resource.</span></span> | <span data-ttu-id="962d1-172">*Data Transfer In (GB)* , *Data Transfer Out (GB)*</span><span class="sxs-lookup"><span data-stu-id="962d1-172">*Data Transfer In (GB)*, *Data Transfer Out (GB)*</span></span> |
| <span data-ttu-id="962d1-173">Region</span><span class="sxs-lookup"><span data-stu-id="962d1-173">Region</span></span> | <span data-ttu-id="962d1-174">The region to which the usage applies.</span><span class="sxs-lookup"><span data-stu-id="962d1-174">The region to which the usage applies.</span></span> <span data-ttu-id="962d1-175">Primarily used to assign rates to data transfers, because rates vary by region.</span><span class="sxs-lookup"><span data-stu-id="962d1-175">Primarily used to assign rates to data transfers, because rates vary by region.</span></span> | <span data-ttu-id="962d1-176">*Asia Pacific*, *Europe*, *Latin America*, *North America*</span><span class="sxs-lookup"><span data-stu-id="962d1-176">*Asia Pacific*, *Europe*, *Latin America*, *North America*</span></span> |
| <span data-ttu-id="962d1-177">SKU</span><span class="sxs-lookup"><span data-stu-id="962d1-177">SKU</span></span> | <span data-ttu-id="962d1-178">Unique Microsoft identifier for an offer.</span><span class="sxs-lookup"><span data-stu-id="962d1-178">Unique Microsoft identifier for an offer.</span></span> | <span data-ttu-id="962d1-179">*7UD-00001*</span><span class="sxs-lookup"><span data-stu-id="962d1-179">*7UD-00001*</span></span> |
| <span data-ttu-id="962d1-180">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="962d1-180">DetailLineItemId</span></span> | <span data-ttu-id="962d1-181">An identifier and quantity to itemize different rates for a service or resource in a given billing period.</span><span class="sxs-lookup"><span data-stu-id="962d1-181">An identifier and quantity to itemize different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="962d1-182">For Azure tiered pricing, there may be one rate for up to a certain quantity of billable units, then a different rate after that quantity.</span><span class="sxs-lookup"><span data-stu-id="962d1-182">For Azure tiered pricing, there may be one rate for up to a certain quantity of billable units, then a different rate after that quantity.</span></span> | <span data-ttu-id="962d1-183">*1*</span><span class="sxs-lookup"><span data-stu-id="962d1-183">*1*</span></span> |
| <span data-ttu-id="962d1-184">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="962d1-184">ConsumedQuantity</span></span> | <span data-ttu-id="962d1-185">The amount of service consumed (such as hours or GB) during the reporting period.</span><span class="sxs-lookup"><span data-stu-id="962d1-185">The amount of service consumed (such as hours or GB) during the reporting period.</span></span> <span data-ttu-id="962d1-186">此外还包括来自以前报告期间任何未开票的使用量。</span><span class="sxs-lookup"><span data-stu-id="962d1-186">Also includes any unbilled usage from previous reporting periods.</span></span> | <span data-ttu-id="962d1-187">*11*</span><span class="sxs-lookup"><span data-stu-id="962d1-187">*11*</span></span> |
| <span data-ttu-id="962d1-188">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="962d1-188">IncludedQuantity</span></span> | <span data-ttu-id="962d1-189">作为产品/服务的一部分包含在内的单位。</span><span class="sxs-lookup"><span data-stu-id="962d1-189">Units included as part of the offer.</span></span> <span data-ttu-id="962d1-190">Typically not present in CSP.</span><span class="sxs-lookup"><span data-stu-id="962d1-190">Typically not present in CSP.</span></span> | <span data-ttu-id="962d1-191">*0*</span><span class="sxs-lookup"><span data-stu-id="962d1-191">*0*</span></span> |
| <span data-ttu-id="962d1-192">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="962d1-192">OverageQuantity</span></span> | <span data-ttu-id="962d1-193">Units not included as part of the offer.</span><span class="sxs-lookup"><span data-stu-id="962d1-193">Units not included as part of the offer.</span></span> <span data-ttu-id="962d1-194">These must be paid for by the partner.</span><span class="sxs-lookup"><span data-stu-id="962d1-194">These must be paid for by the partner.</span></span> <span data-ttu-id="962d1-195">Equal to **ConsumedQuantity** minus **IncludedQuantity**.</span><span class="sxs-lookup"><span data-stu-id="962d1-195">Equal to **ConsumedQuantity** minus **IncludedQuantity**.</span></span> | <span data-ttu-id="962d1-196">*11*</span><span class="sxs-lookup"><span data-stu-id="962d1-196">*11*</span></span> |
| <span data-ttu-id="962d1-197">ListPrice</span><span class="sxs-lookup"><span data-stu-id="962d1-197">ListPrice</span></span> | <span data-ttu-id="962d1-198">Offer price in effect at subscription's start date.</span><span class="sxs-lookup"><span data-stu-id="962d1-198">Offer price in effect at subscription's start date.</span></span> | <span data-ttu-id="962d1-199">*$0.0808*</span><span class="sxs-lookup"><span data-stu-id="962d1-199">*$0.0808*</span></span> |
| <span data-ttu-id="962d1-200">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="962d1-200">PretaxCharges</span></span> | <span data-ttu-id="962d1-201">Equal to **ListPrist** multiplied by **OverageQuantity**, rounded to the nearest cent.</span><span class="sxs-lookup"><span data-stu-id="962d1-201">Equal to **ListPrist** multiplied by **OverageQuantity**, rounded to the nearest cent.</span></span> | <span data-ttu-id="962d1-202">*$0.085*</span><span class="sxs-lookup"><span data-stu-id="962d1-202">*$0.085*</span></span> |
| <span data-ttu-id="962d1-203">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="962d1-203">TaxAmount</span></span> | <span data-ttu-id="962d1-204">Tax amount charged.</span><span class="sxs-lookup"><span data-stu-id="962d1-204">Tax amount charged.</span></span> <span data-ttu-id="962d1-205">Based on your market's tax rules and specific circumstances.</span><span class="sxs-lookup"><span data-stu-id="962d1-205">Based on your market's tax rules and specific circumstances.</span></span> | <span data-ttu-id="962d1-206">*$0.08*</span><span class="sxs-lookup"><span data-stu-id="962d1-206">*$0.08*</span></span> |
| <span data-ttu-id="962d1-207">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="962d1-207">PostTaxTotal</span></span> | <span data-ttu-id="962d1-208">税后总额（如果税务适用）。</span><span class="sxs-lookup"><span data-stu-id="962d1-208">Total after tax, when tax is applicable.</span></span> | <span data-ttu-id="962d1-209">*$0.93*</span><span class="sxs-lookup"><span data-stu-id="962d1-209">*$0.93*</span></span> |
| <span data-ttu-id="962d1-210">货币</span><span class="sxs-lookup"><span data-stu-id="962d1-210">Currency</span></span> | <span data-ttu-id="962d1-211">货币类型。</span><span class="sxs-lookup"><span data-stu-id="962d1-211">Currency type.</span></span> <span data-ttu-id="962d1-212">每个计费单位仅使用一种货币。</span><span class="sxs-lookup"><span data-stu-id="962d1-212">Each billing entity has only one currency.</span></span> <span data-ttu-id="962d1-213">Check that it matches your first invoice and then after any major billing platform updates.</span><span class="sxs-lookup"><span data-stu-id="962d1-213">Check that it matches your first invoice and then after any major billing platform updates.</span></span> | <span data-ttu-id="962d1-214">*EUR*</span><span class="sxs-lookup"><span data-stu-id="962d1-214">*EUR*</span></span> |
| <span data-ttu-id="962d1-215">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="962d1-215">PretaxEffectiveRate</span></span> | <span data-ttu-id="962d1-216">每一单位的税前价格。</span><span class="sxs-lookup"><span data-stu-id="962d1-216">Pretax price per unit.</span></span> <span data-ttu-id="962d1-217">Equal to **PretaxCharges** divided by **OverageQuantity**, rounded to the nearest cent.</span><span class="sxs-lookup"><span data-stu-id="962d1-217">Equal to **PretaxCharges** divided by **OverageQuantity**, rounded to the nearest cent.</span></span> | <span data-ttu-id="962d1-218">*$0.08*</span><span class="sxs-lookup"><span data-stu-id="962d1-218">*$0.08*</span></span> |
| <span data-ttu-id="962d1-219">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="962d1-219">PostTaxEffectiveRate</span></span> | <span data-ttu-id="962d1-220">每一单位的税后价格。</span><span class="sxs-lookup"><span data-stu-id="962d1-220">Post tax price per unit.</span></span> <span data-ttu-id="962d1-221">Equal to **PostTaxTotal** divided by **OverageQuantity**, rounded to the nearest cent.</span><span class="sxs-lookup"><span data-stu-id="962d1-221">Equal to **PostTaxTotal** divided by **OverageQuantity**, rounded to the nearest cent.</span></span> <span data-ttu-id="962d1-222">Or, equal to **PretaxEffectiveRate** plus thet tax rate per unit amoun, rounded to the nearest cent.</span><span class="sxs-lookup"><span data-stu-id="962d1-222">Or, equal to **PretaxEffectiveRate** plus thet tax rate per unit amoun, rounded to the nearest cent.</span></span> | <span data-ttu-id="962d1-223">*$0.08*</span><span class="sxs-lookup"><span data-stu-id="962d1-223">*$0.08*</span></span> |
| <span data-ttu-id="962d1-224">ChargeType</span><span class="sxs-lookup"><span data-stu-id="962d1-224">ChargeType</span></span> | <span data-ttu-id="962d1-225">The [type of charge](recon-file-charge-types.md) or adjustment.</span><span class="sxs-lookup"><span data-stu-id="962d1-225">The [type of charge](recon-file-charge-types.md) or adjustment.</span></span> | <span data-ttu-id="962d1-226">See [charge types](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="962d1-226">See [charge types](recon-file-charge-types.md).</span></span> |
| <span data-ttu-id="962d1-227">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="962d1-227">CustomerBillableAccount</span></span> | <span data-ttu-id="962d1-228">Unique account identifier in the Microsoft billing platform.</span><span class="sxs-lookup"><span data-stu-id="962d1-228">Unique account identifier in the Microsoft billing platform.</span></span> | <span data-ttu-id="962d1-229">*1280018095*</span><span class="sxs-lookup"><span data-stu-id="962d1-229">*1280018095*</span></span> |
| <span data-ttu-id="962d1-230">UsageDate</span><span class="sxs-lookup"><span data-stu-id="962d1-230">UsageDate</span></span> | <span data-ttu-id="962d1-231">服务部署日期。</span><span class="sxs-lookup"><span data-stu-id="962d1-231">Date of service deployment.</span></span> | <span data-ttu-id="962d1-232">*2/1/2019 0:00*</span><span class="sxs-lookup"><span data-stu-id="962d1-232">*2/1/2019 0:00*</span></span> |
| <span data-ttu-id="962d1-233">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="962d1-233">MeteredRegion</span></span> | <span data-ttu-id="962d1-234">Identifies the location of a data center within the region (for services where this value is applicable and populated).</span><span class="sxs-lookup"><span data-stu-id="962d1-234">Identifies the location of a data center within the region (for services where this value is applicable and populated).</span></span> | <span data-ttu-id="962d1-235">*East Asia*, *South East Asia*, *North Europe*, *West Europe*, *North Central US*, *South Central US*</span><span class="sxs-lookup"><span data-stu-id="962d1-235">*East Asia*, *South East Asia*, *North Europe*, *West Europe*, *North Central US*, *South Central US*</span></span> |
| <span data-ttu-id="962d1-236">MeteredService</span><span class="sxs-lookup"><span data-stu-id="962d1-236">MeteredService</span></span> | <span data-ttu-id="962d1-237">Identifies the individual Azure service usage when it's not specifically identified in the **ServiceName** column.</span><span class="sxs-lookup"><span data-stu-id="962d1-237">Identifies the individual Azure service usage when it's not specifically identified in the **ServiceName** column.</span></span> <span data-ttu-id="962d1-238">For example, data transfers are reported as *Microsoft Azure - All Services* in the **ServiceName** column.</span><span class="sxs-lookup"><span data-stu-id="962d1-238">For example, data transfers are reported as *Microsoft Azure - All Services* in the **ServiceName** column.</span></span> | <span data-ttu-id="962d1-239">*AccessControl*, *CDN*, *Compute*, *Database*, *ServiceBus*, *Storage*</span><span class="sxs-lookup"><span data-stu-id="962d1-239">*AccessControl*, *CDN*, *Compute*, *Database*, *ServiceBus*, *Storage*</span></span> |
| <span data-ttu-id="962d1-240">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="962d1-240">MeteredServiceType</span></span> | <span data-ttu-id="962d1-241">Subheading for **MeteredService** field that provides additional clarification of Azure service usage.</span><span class="sxs-lookup"><span data-stu-id="962d1-241">Subheading for **MeteredService** field that provides additional clarification of Azure service usage.</span></span> | <span data-ttu-id="962d1-242">*EXTERNAL*</span><span class="sxs-lookup"><span data-stu-id="962d1-242">*EXTERNAL*</span></span> |
| <span data-ttu-id="962d1-243">项目</span><span class="sxs-lookup"><span data-stu-id="962d1-243">Project</span></span> | <span data-ttu-id="962d1-244">Customer-defined name for their service instance.</span><span class="sxs-lookup"><span data-stu-id="962d1-244">Customer-defined name for their service instance.</span></span> | <span data-ttu-id="962d1-245">*ORDDC52E52FDEF405786F0642DD0108BE4*</span><span class="sxs-lookup"><span data-stu-id="962d1-245">*ORDDC52E52FDEF405786F0642DD0108BE4*</span></span> |
| <span data-ttu-id="962d1-246">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="962d1-246">ServiceInfo</span></span> | <span data-ttu-id="962d1-247">The number of Azure Service Bus connections that were provisioned and utilized on a given day.</span><span class="sxs-lookup"><span data-stu-id="962d1-247">The number of Azure Service Bus connections that were provisioned and utilized on a given day.</span></span> | <span data-ttu-id="962d1-248">*1.000000 Connections / 30 days* (if you had an individually provisioned connection during a 30-day month), *25 Connections / 30 Days – Used: 1.000000* (if you had a 25 pack of Service Bus connections provisioned and you utilized 1 during that day)</span><span class="sxs-lookup"><span data-stu-id="962d1-248">*1.000000 Connections / 30 days* (if you had an individually provisioned connection during a 30-day month), *25 Connections / 30 Days – Used: 1.000000* (if you had a 25 pack of Service Bus connections provisioned and you utilized 1 during that day)</span></span> |
| <span data-ttu-id="962d1-249">CustomerID</span><span class="sxs-lookup"><span data-stu-id="962d1-249">CustomerID</span></span> | <span data-ttu-id="962d1-250">Unique Microsoft identifier for the customer, in GUID format.</span><span class="sxs-lookup"><span data-stu-id="962d1-250">Unique Microsoft identifier for the customer, in GUID format.</span></span> | <span data-ttu-id="962d1-251">*ORDDC52E52FDEF405786F0642DD0108BE4*</span><span class="sxs-lookup"><span data-stu-id="962d1-251">*ORDDC52E52FDEF405786F0642DD0108BE4*</span></span> |
| <span data-ttu-id="962d1-252">DomainName</span><span class="sxs-lookup"><span data-stu-id="962d1-252">DomainName</span></span> | <span data-ttu-id="962d1-253">Customer's domain name.</span><span class="sxs-lookup"><span data-stu-id="962d1-253">Customer's domain name.</span></span> <span data-ttu-id="962d1-254">该字段在第二个计费周期之前可能会显示为空白。</span><span class="sxs-lookup"><span data-stu-id="962d1-254">This field may appear blank until the second billing cycle.</span></span> | <span data-ttu-id="962d1-255">*example.onmicrosoft.com*</span><span class="sxs-lookup"><span data-stu-id="962d1-255">*example.onmicrosoft.com*</span></span> |
| <span data-ttu-id="962d1-256">单位</span><span class="sxs-lookup"><span data-stu-id="962d1-256">Unit</span></span> | <span data-ttu-id="962d1-257">The unit of the resource **Name**.</span><span class="sxs-lookup"><span data-stu-id="962d1-257">The unit of the resource **Name**.</span></span> | <span data-ttu-id="962d1-258">*GB* or *HOURS*</span><span class="sxs-lookup"><span data-stu-id="962d1-258">*GB* or *HOURS*</span></span> |