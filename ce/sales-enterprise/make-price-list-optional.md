---
title: "Make price list optional (Dynamics 365 Sales) | MicrosoftDocs"
description: "Allow your salespeople to add products without associating a price list first."
keywords: "price list, optional, Quote, order, invoice, opportunity"
ms.date: 08/01/2019
ms.service: dynamics-365-sales
ms.custom: dyn365-sales
ms.topic: article
ms.assetid: 94c80808-d68e-4df7-b5a6-40e6ee791f48
author: shubhadaj
ms.author: shujoshi
manager: annbe
---

# Allow adding products without associated price list

[!INCLUDE[cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

When adding products to opportunities, quotes, orders, or invoices, at times, salespeople need to specify the product prices ad hoc. You can allow salespeople to add products without associating a price list first.

> [!IMPORTANT]
> - [!INCLUDE[cc-preview-features-definition](../includes/cc-preview-features-definition.md)]
> - [!INCLUDE[cc-preview-features-no-ms-support](../includes/cc-preview-features-no-ms-support.md)]
> - To learn about enabling preview features in the 2019 release wave 2, see [How do I enable the 2019 release wave 2 updates](/power-platform/admin/preview-october-2019-updates#when-will-the-2019-release-wave-2-features-be-enabled)

## Make price list optional (Sales Hub)

1.	In your app, at the bottom of the site map, select **Change area** ![Icon to change the work area](media/change-area-icon.png "Icon to change the work area"), and select **App Settings**.

2.	Under **Product Catalog**, select **Product Catalog Settings**.

3.  Under **Make price lists optional**, set the **Allow line item creation without an associated price list** option to **Yes**.

    ![Option to make selection of price list optional](media/sales-hub-make-price-list-optional.png "Option to make selection of price list optional")

4.  Select **Apply**.

## Make price list optional (legacy web client)

1.  In your app, on the nav bar, select the **Settings** icon, and then select **Advanced Settings**.

    The Business Management settings page opens in a new browser tab.

2.  On the nav bar, select **Settings**, and then select **Administration**.

3.  Select **System Settings**.

4.  In the **System Settings dialog** box, on the **Sales** tab, set the **Make
    price lists optional** field to **Yes**.

    ![Option to make selection of price list optional](media/make-price-list-optional.png "Option to make selection of price list optional")

### See also
[Add products to an opportunity](add-products-opportunity.md)  
[Add products to a quote, order, or invoice](add-product-quote-order-invoice.md)
