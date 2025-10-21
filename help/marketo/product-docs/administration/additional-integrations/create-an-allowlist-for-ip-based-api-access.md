---
unique-page-id: 10098433
description: Creare un Inserisco nell'elenco Consentiti di accesso API basato su IP - Documentazione di Marketo - Documentazione del prodotto
title: Creare un elenco Consentiti per l’accesso API basato su IP
exl-id: 1a2f2216-07ee-4d37-b883-458ea39fc452
feature: Administration
source-git-commit: 3595cdc76a0f92da10dc5ddaac64c4cf83056e88
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 13%

---

# Creare un elenco Consentiti per l’accesso API basato su IP {#create-an-allowlist-for-ip-based-api-access}

A volte, è necessario concedere l’accesso API solo a un indirizzo IP specifico o a un intervallo di indirizzi. A questo scopo, devi innanzitutto abilitare le restrizioni, quindi specificare gli indirizzi IP che possono utilizzare le API.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>Questa funzione opera indipendentemente dalle [restrizioni di accesso basate su IP di Marketo Engage](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} che vengono sostituite dal [controllo di accesso basato su IP di Admin Console](https://helpx.adobe.com/it/enterprise/using/ip-based-access.html){target="_blank"}. Continuerà a funzionare così com’è dopo la migrazione di Adobe IMS.

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-1.png)

1. Fai clic su **[!UICONTROL Web Services]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-2.png)

1. Nell&#39;area **[!UICONTROL IP Restrictions]** fare clic su **[!UICONTROL Edit],** o su **[!UICONTROL Edit IP Restrictions]** in alto a sinistra.

   ![](assets/create-an-allowlist-for-ip-based-api-access-3.png)

1. Inserire nell&#39;elenco Consentiti Selezionare la casella **[!UICONTROL Enable IP Restrictions]** e immettere gli indirizzi IP che si desidera.

   ![](assets/create-an-allowlist-for-ip-based-api-access-4.png)

   >[!NOTE]
   >
   >È possibile immettere un singolo indirizzo IP o un intervallo oppure utilizzare un carattere jolly.

1. Fare clic su **[!UICONTROL Add]** per aprire ulteriori campi e immettere altri indirizzi IP.

   ![](assets/create-an-allowlist-for-ip-based-api-access-5.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-6.png)
