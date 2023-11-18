---
description: Passaggio 4 di 4 - Collegare la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa - Documentazione Marketo - Documentazione del prodotto
title: Passaggio 4 di 4 - Connessione della soluzione Marketo con la connessione del controllo della password del proprietario della risorsa
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 1%

---

# Passaggio 4 di 4: connettere la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa {#step-4-of-4-connect-the-marketo-solution-ropc}

Ultimo passaggio della sincronizzazione. Ci sei quasi!

>[!PREREQUISITES]
>
>* [Passaggio 1 di 4: installare la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [Passaggio 2 di 4: configurare la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}
>* [Passaggio 3 di 4: configurare l’app client su MS Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>Se aggiorni l’autenticazione di base a OAuth, puoi utilizzare [questo articolo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"} per riconfigurare l’autenticazione.

## Immetti le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedi a Marketo e fai clic su **Aadmin**.

   ![](assets/login-admin.png)

1. Clic **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Seleziona **[!UICONTROL Microsoft]**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Clic **[!UICONTROL Modifica]** in **[!UICONTROL Immetti le credenziali]**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Assicurati che l’URL dell’organizzazione sia corretto, poiché non è possibile ripristinare le modifiche allo schema successive dopo l’invio. Se viene utilizzato un URL organizzazione errato, dovrai ottenere una nuova sottoscrizione Marketo. Se non conosci l’URL, [scopri come trovarlo qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

   >[!NOTE]
   >
   >Prima di immettere le nuove credenziali, è possibile [convalidale qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}.

1. Inserisci il **[!UICONTROL Nome utente]**, **[!UICONTROL Password]**, Microsoft Dynamics **URL**, **[!UICONTROL ID client]**, e **[!UICONTROL Segreto client]**. Clic **[!UICONTROL Salva]** al termine.

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato è `user@domain.com` o DOMINIO\utente.

## Seleziona campi da sincronizzare {#select-fields-to-sync}

1. Clic **[!UICONTROL Modifica]** in **[!UICONTROL Seleziona campi da sincronizzare]**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Seleziona i campi da sincronizzare con Marketo in modo che siano preselezionati. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo memorizza un riferimento ai campi da sincronizzare. Se elimini un campo in Dynamics, è consigliabile eseguire questa operazione con [sincronizzazione disabilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Then refresh the schema in Marketo by editing and saving the [Select Fields to Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.

## Sincronizza campi per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se hai creato un filtro personalizzato, accertati di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Vai a Amministratore e seleziona **[!DNL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clic **[!UICONTROL Modifica]** in Dettagli sincronizzazione campi.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e selezionalo. Il nome effettivo deve essere new_synctomkto, ma il nome visualizzato può essere qualsiasi cosa. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Abilita sincronizzazione {#enable-sync}

1. Clic **[!UICONTROL Modifica]** in **[!UICONTROL Abilita sincronizzazione]**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione su una sincronizzazione Microsoft Dynamics o quando immetti manualmente persone o lead.

1. Leggi tutto il contenuto del pop-up, immetti il tuo indirizzo e-mail e fai clic su **[!UICONTROL Avvia sincronizzazione]**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine riceverai una notifica e-mail.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Ottimo lavoro!

>[!MORELIKETHIS]
>
>[Riconfigura metodo di autenticazione Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"}
