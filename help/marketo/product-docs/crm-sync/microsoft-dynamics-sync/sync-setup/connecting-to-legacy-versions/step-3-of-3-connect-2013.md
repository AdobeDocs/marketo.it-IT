---
unique-page-id: 3571819
description: Passaggio 3 di 3 - Connessione di Marketo e Dynamics (on-premise 2013) - Documentazione di Marketo - Documentazione del prodotto
title: 'Passaggio 3 di 3: connessione di Marketo e Dynamics (on-premise 2013)'
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---

# Passaggio 3 di 3: Connessione di Marketo e Dynamics (on-premise 2013) {#step-of-connect-marketo-and-dynamics-on-premises}

Va bene! Abbiamo installato la soluzione e configurato l&#39;utente di sincronizzazione. Successivamente, è necessario collegare Marketi Engage e Dynamics.

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: installare la soluzione Marketo in Dynamics (on-premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md){target="_blank"}
>* [Passaggio 2 di 3: configurare l&#39;utente Sync per Marketo (on-premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md){target="_blank"}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immetti le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedi a Marketo e fai clic su **[!UICONTROL Amministratore]**.

   ![](assets/login-admin.png)

1. Fai clic su **[!UICONTROL CRM]**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Seleziona **[!DNL Microsoft]**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Clic **[!UICONTROL Modifica]** in **[!UICONTROL Immetti le credenziali]**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Assicurati che le credenziali siano corrette in quanto non è possibile ripristinare le modifiche allo schema successive dopo l’invio. Se vengono salvate credenziali non corrette, dovrai ottenere una nuova sottoscrizione Marketo.

1. Inserisci il **[!UICONTROL Nome utente]**, **[!UICONTROL Password]** e Microsoft Dynamics **[!UICONTROL URL]** quindi fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato è `user@domain.com` o DOMINIO\utente.
   >* Se non conosci l’URL, [scopri come trovarlo qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

## Seleziona campi da sincronizzare {#select-fields-to-sync}

Ora è necessario selezionare i campi da sincronizzare.

1. Clic **[!UICONTROL Modifica]** in **[!UICONTROL Seleziona campi da sincronizzare]**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Seleziona i campi da sincronizzare con Marketo in modo che siano preselezionati. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

   >[!NOTE]
   >
   >Marketo memorizza un riferimento ai campi da sincronizzare. Se elimini un campo in Dynamics, è consigliabile eseguire questa operazione con [sincronizzazione disabilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Then refresh the schema in Marketo by editing and saving the [Select Fields to Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.

## Sincronizza campi per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se hai creato un filtro personalizzato, accertati di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Vai a Amministratore e seleziona **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clic **[!UICONTROL Modifica]** in Dettagli sincronizzazione campi.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e selezionalo. Il nome effettivo deve essere new_synctomkto, ma il nome visualizzato può essere qualsiasi cosa. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Abilita sincronizzazione {#enable-sync}

1. Clic **[!UICONTROL Modifica]** in **[!UICONTROL Abilita sincronizzazione]**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione su una sincronizzazione Microsoft Dynamics o quando immetti manualmente persone o lead.

1. Leggi tutto il contenuto del pop-up, immetti il tuo indirizzo e-mail e fai clic su **[!UICONTROL Avvia sincronizzazione]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine riceverai una notifica e-mail.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

Ottimo lavoro! Hai appena liberato la potenza della sincronizzazione bidirezionale tra Marketo e Microsoft Dynamics. Se hai acquistato Marketo Sales Insight, è più divertente:

>[!MORELIKETHIS]
>
>[Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2013](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md){target="_blank"}
