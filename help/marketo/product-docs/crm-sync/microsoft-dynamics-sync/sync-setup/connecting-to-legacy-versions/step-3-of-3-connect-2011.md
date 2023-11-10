---
unique-page-id: 3571809
description: 'Passaggio 3 di 3: collegare Microsoft Dynamics a Marketo (on-premise 2011) - Documentazione di Marketo - Documentazione del prodotto'
title: 'Passaggio 3 di 3: collegare Microsoft Dynamics a Marketo (on-premise 2011)'
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Passaggio 3 di 3: collegare Microsoft Dynamics a Marketo (on-premise 2011) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

Va bene! Abbiamo installato la soluzione e configurato l&#39;utente di sincronizzazione. Successivamente, è necessario collegare Marketo e Dynamics.

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: installare la soluzione Marketo (on-premise 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}
>* [Passaggio 2 di 3: configurare l’utente di Marketo Sync in Dynamics (on-premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md){target="_blank"}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immetti le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedi a Marketo e fai clic su **[!UICONTROL Amministratore]**.

   ![](assets/login-admin.png)

1. Clic **[!UICONTROL CRM]**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Clic **[!DNL Microsoft]**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Clic **[!UICONTROL Modifica]** in **[!UICONTROL Immetti le credenziali]**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Assicurati che le credenziali siano corrette in quanto non è possibile ripristinare le modifiche allo schema successive dopo l’invio. Se vengono salvate credenziali non corrette, dovrai ottenere una nuova sottoscrizione Marketo.

1. Inserisci il **[!UICONTROL Nome utente]**, **[!UICONTROL Password]** e CRM **[!UICONTROL URL]**, quindi fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato è `user@domain.com` o DOMINIO\utente.
   >* Se non conosci l’URL, [scopri come trovarlo qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

## Seleziona campi da sincronizzare {#select-fields-to-sync}

Ora è necessario selezionare i campi da sincronizzare.

1. Clic **[!UICONTROL Modifica]** in **[!UICONTROL Seleziona campi da sincronizzare]**.

   ![](assets/image2015-3-16-9-51-28a.png)

1. Alcuni campi preselezionati verranno sincronizzati. Se lo desideri, aggiungi altro e fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

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

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Abilita sincronizzazione {#enable-sync}

1. Clic **[!UICONTROL Modifica]** in **[!UICONTROL Abilita sincronizzazione]**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione su una sincronizzazione Microsoft Dynamics o quando immetti manualmente persone o lead.

1. Leggi tutto il contenuto del pop-up, immetti il tuo indirizzo e-mail e fai clic su **[!UICONTROL Avvia sincronizzazione]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine riceverai una notifica e-mail.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   Ottimo lavoro!
