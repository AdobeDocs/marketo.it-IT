---
unique-page-id: 10098433
description: Restrict API access to specific IP addresses or ranges via Admin Web Services IP Restrictions.
title: Creare un elenco Consentiti per l’accesso API basato su IP
exl-id: 1a2f2216-07ee-4d37-b883-458ea39fc452
feature: Administration
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 15%

---

# Creare un elenco Consentiti per l’accesso API basato su IP {#create-an-allowlist-for-ip-based-api-access}

Sometimes, you want to give API access only to a specific IP address or a range of addresses. To do this, you first enable restrictions, then specify the IP addresses that are allowed to use the APIs.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!CAUTION]
>
>Enabling this feature prevents you from being able to access the [Marketo MCP Server](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mcp-server){target="_blank"} at this time. This is expected to be resolved in an upcoming release.

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-1.png)

1. Fai clic su **[!UICONTROL Web Services]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-2.png)

1. In the **[!UICONTROL IP Restrictions]** area, click **[!UICONTROL Edit],** or click **[!UICONTROL Edit IP Restrictions]** in the upper left.

   ![](assets/create-an-allowlist-for-ip-based-api-access-3.png)

1. Check the **[!UICONTROL Enable IP Restrictions]** box and enter the IP addresses you want to Allowlist.

   ![](assets/create-an-allowlist-for-ip-based-api-access-4.png)

   >[!NOTE]
   >
   >You can enter a single IP address or a range of them, or use a wildcard.

1. Click **[!UICONTROL Add]** to open additional fields to enter more IP addresses.

   ![](assets/create-an-allowlist-for-ip-based-api-access-5.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-6.png)
