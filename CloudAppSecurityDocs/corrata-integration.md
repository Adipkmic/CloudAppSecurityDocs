---
title: Integrate Defender for Cloud Apps with Corrata
description: This article describes how to integrate Microsoft Defender for Cloud Apps with Corrata for seamless Cloud Discovery and automated block of unsanctioned apps.
ms.date: 11/09/2021
ms.topic: how-to
---
# Integrate Defender for Cloud Apps with Corrata

[!INCLUDE [Banner for top of topics](includes/banner.md)]

If you work with both Defender for Cloud Apps and Corrata, you can integrate the two products to enhance your security Cloud Discovery experience for mobile app use. Corrata, as a local Mobile gateway, monitors your organization's traffic from mobile devices enabling you to set policies for blocking transactions. Together, Defender for Cloud Apps and Corrata provide the following capabilities:

- Seamless deployment of Cloud Discovery - Use Corrata to collect your mobile device traffic and send it to Defender for Cloud Apps. This eliminates the need for installation of log collectors on your network endpoints to enable Cloud Discovery.
- Corrata's block capabilities are automatically applied on apps you set as unsanctioned in Defender for Cloud Apps.
- Enhance your Corrata portal with the Defender for Cloud Apps risk assessment for leading cloud apps, which can be viewed directly in the Corrata portal.

## Prerequisites

- A valid license for Microsoft Defender for Cloud Apps
- A valid license for Corrata Cloud

## Deployment

1. In the Corrata portal, do the steps to complete the [Corrata partner integration with Microsoft Defender for Cloud Apps](https://corrata.com/microsoft-mcas-onboarding/).
2. In the [Defender for Cloud Apps portal](https://portal.cloudappsecurity.com/), do the following integration steps:
    1. Click on the settings cog and select **Cloud Discovery Settings**.
    2. Click on the **Automatic log upload** tab and then click **Add data source**.
    3. In the **Add data source** page, enter the following settings:

        - Name = Corrata
        - Source = Corrata
        - Receiver type = FTP

        ![data source Corrata.](media/data-source-corrata.png)

    4. Click **View sample of expected log file**. Then click **Download sample log** to view a sample discovery log, and make sure it matches your logs.

3. Investigate cloud apps discovered on your network. For more information and investigation steps, see [Working with Cloud Discovery](working-with-cloud-discovery-data.md).

4. Any app that you set as unsanctioned in Defender for Cloud Apps will be pinged by Corrata, and then automatically blocked by Corrata. For more information about unsanctioning apps, see [Sanctioning/unsanctioning an app](governance-discovery.md#BKMK_SanctionApp).

## Next steps

> [!div class="nextstepaction"]
> [Control cloud apps with policies](control-cloud-apps-with-policies.md)

[!INCLUDE [Open support ticket](includes/support.md)]
