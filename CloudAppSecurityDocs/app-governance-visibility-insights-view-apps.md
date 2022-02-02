---
title: View your apps
ms.date: 11/09/2021
ms.topic: how-to
description: View your apps.
---

# View your apps

App governance allows you to quickly gain deep insights into the Microsoft 365 OAuth apps in your tenant. For example, you can see:

- A list of OAuth-enabled apps in the tenant that use the Microsoft Graph API, together with relevant app metadata and usage data.
- App details with deeper insights and information by selecting an app in the list.

## Getting a list of all the apps in your tenant

For a summary of apps in your tenant, go to **Microsoft 365 Defender > App governance > Apps**.

:::image type="content" source="media\app-governance\mapg-cc-apps.png" alt-text="The app governance app summary page in Microsoft 365 Defender." lightbox="media\app-governance\mapg-cc-apps.png":::

>[!Note]
> Your sign-in account must have one of [these roles](app-governance-get-started.md#administrator-roles) to view any app governance data.
>

You will see a list of apps and this information:

- App Name
- Added on

  When the app was registered in Azure AD
  
- Last modified

  Shows the date app governance was installed in client if that date is more recent than the date the app was last modified.
  
- Consent type

  Shows whether app consent has been given at the user or the admin level, and the number of users whose data is accessible to the app.
  
- Data usage (preview)

  The sum of the app’s data upload and download in the tenant over the last day, along with the change over the prior day.
  
- Publisher
- App status

  Shows whether the app is enabled or disabled, and if disabled who disabled the app
- Privilege level
- Certification

  Indicates whether the app is compatible with Microsoft technologies, compliant with Defender for Cloud Apps best practices, and supported by Microsoft.

- App ID

App governance sorts the app list alphabetically by **App name** by default. To sort the list by another app attribute, select the attribute name.

You can also select **Search** to search for an app by name.

## Getting detailed information on an app

For detailed information on a specific app in your tenant, go to **Microsoft 365 Defender > App governance > Apps > *app name***.

:::image type="content" source="media\app-governance\mapg-cc-apps-app.png" alt-text="The app governance app details pane in  Microsoft 365 Defender." lightbox="media\app-governance\mapg-cc-apps-app.png":::

The app details pane provides additional information on these tabs:

| Tab name | Description |
|:-------|:-----|
| Details | See additional data on the app such as the date first consented and the App ID. To see the properties of the app as registered in Azure AD, select **View app in Azure AD**. |
| Data usage |See the data usage by the app in the tenant and plot the data usage for SharePoint and Exchange resources. You can fliter usage insights by priority accounts only |
| Users | See a list of users who are using the app, whether they're a priority account, and the amount of data downloaded and uploaded. If an app is admin consented, the Total consented users will be all users in the tenant. |
| Permissions | See a summary and list of the Graph API and legacy permissions granted to the app, consent type, and whether they are in use. For more information, see the [Microsoft Graph permissions reference](/graph/permissions-reference). |
|||

For an enabled app, there's also a **Disable app** control to disable the use of the selected app and an **Enable app** control to enable the use of the disabled app. These actions require these administrator roles:

- Compliance Administrator
- Global or Company Administrator
- Security Administrator
- Security Operator

## Next step

[Determine your overall app compliance posture](app-governance-visibility-insights-compliance-posture.md).
