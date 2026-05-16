---
unique-page-id: 10098433
description: Limita l’accesso API a specifici indirizzi IP o intervalli tramite le restrizioni IP dei servizi web di amministrazione.
title: Creazione di un Inserisco nell'elenco Consentiti di accesso API basato su IP
exl-id: 1a2f2216-07ee-4d37-b883-458ea39fc452
feature: Administration
TQID: https://experienceleague.adobe.com/MIuDfjHpqBC2Z-hMEgtk0BvK-W2DEL25M-j6GNQK9zI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 161
ht-degree: 0%

---

# Creazione di un Inserisco nell&#39;elenco Consentiti di accesso API basato su IP {#create-an-allowlist-for-ip-based-api-access}

A volte, è necessario concedere l’accesso API solo a un indirizzo IP specifico o a un intervallo di indirizzi. A questo scopo, devi innanzitutto abilitare le restrizioni, quindi specificare gli indirizzi IP che possono utilizzare le API.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!CAUTION]
>
>L&#39;attivazione di questa funzionalità impedisce l&#39;accesso a [Marketo MCP Server](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mcp-server){target="_blank"} in questo momento. Questa situazione dovrebbe essere risolta in una prossima versione.

1. Passare all&#39;area **[!UICONTROL Admin]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-1.png)

1. Fare clic su **[!UICONTROL Web Services]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-2.png)

1. Nell&#39;area **[!UICONTROL IP Restrictions]** fare clic su **[!UICONTROL Edit],** o su **[!UICONTROL Edit IP Restrictions]** in alto a sinistra.

   ![](assets/create-an-allowlist-for-ip-based-api-access-3.png)

1. Selezionare la casella **[!UICONTROL Enable IP Restrictions]** e immettere gli indirizzi IP che si desidera Inserire nell&#39;elenco Consentiti.

   ![](assets/create-an-allowlist-for-ip-based-api-access-4.png)

   >[!NOTE]
   >
   >È possibile immettere un singolo indirizzo IP o un intervallo oppure utilizzare un carattere jolly.

1. Fare clic su **[!UICONTROL Add]** per aprire ulteriori campi e immettere altri indirizzi IP.

   ![](assets/create-an-allowlist-for-ip-based-api-access-5.png)

1. Fare clic su **[!UICONTROL Save]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-6.png)
