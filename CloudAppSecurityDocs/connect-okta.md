---
title: Connect Okta to Defender for Cloud Apps
description: This article provides information about how to connect your Okta to Defender for Cloud Apps using the API connector for visibility and control over use.
ms.date: 11/09/2021
ms.topic: how-to
---
# Connect Okta to Microsoft Defender for Cloud Apps

[!INCLUDE [Banner for top of topics](includes/banner.md)]

This article provides instructions for connecting Microsoft Defender for Cloud Apps to your existing Okta account using the connector APIs. This connection gives you visibility into and control over Okta use. For information about how Defender for Cloud Apps protects Okta, see [Protect Okta](protect-okta.md).

## How to connect Okta to Defender for Cloud Apps

1. It's recommended that you create an admin Service Account in Okta for Defender for Cloud Apps.

    Make sure you use an account with Super Admin permissions.

    Make sure your Okta account is verified.

1. In the Okta console, click **Admin**.

    - Click on **Security** and then **API**.

         ![Okta api.](media/okta-api.png "Okta api")

    - Click **Create Token**.

         ![Okta create token.](media/okta-createtoken.jpg "Okta create token")

    - In the **Create Token** pop-up, name your Defender for Cloud Apps token, and click **Create Token**.

         ![Okta token pop-up.](media/okta-token-pop-up.png)

    - In the **Token created successfully** pop-up, copy the **Token value**.

         ![Okta token value.](media/okta-token-value.png "Okta token value")

1. In the Defender for Cloud Apps console, click **Investigate** and then **Connected apps**.

1. In the **App connectors page**, click the plus button and then **Okta**.

    ![connect Okta.](media/connect-okta.png "connect Okta")

1. In the pop-up, in the **Domain** field, enter your Okta domain and paste your Token into the **Token** field.

1. Click **Connect** to create the token for Okta in Defender for Cloud Apps.

1. Make sure the connection succeeded by clicking **Test API**.

    Testing may take a couple of minutes. After receiving a success notice, click **Close**.

After connecting Okta, you'll receive events for 60 days prior to connection.

If you have any problems connecting the app, see [Troubleshooting App Connectors](troubleshooting-api-connectors-using-error-messages.md).

## Next steps

> [!div class="nextstepaction"]
> [Control cloud apps with policies](control-cloud-apps-with-policies.md)

[!INCLUDE [Open support ticket](includes/support.md)]
