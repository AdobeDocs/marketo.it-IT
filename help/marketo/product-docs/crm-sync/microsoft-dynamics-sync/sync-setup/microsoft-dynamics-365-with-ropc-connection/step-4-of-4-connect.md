---
description: Passaggio 4 di 4 - Connettere la soluzione Marketo con la connessione Controllo password proprietario risorsa - Marketo Docs - Documentazione del prodotto
title: Passaggio 4 di 4 - Connettere la soluzione Marketo con la connessione per il controllo della password del proprietario della risorsa
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
source-git-commit: f72f195e53d63e37ef2ed53980b9bffc59391430
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# Passaggio 4 di 4: Connessione della soluzione Marketo con la connessione del controllo password del proprietario della risorsa {#step-4-of-4-connect-the-marketo-solution-ropc}

Questo è l&#39;ultimo passaggio della sincronizzazione. Ci sei quasi!

>[!PREREQUISITES]
>
>* [Passaggio 1 di 4: Installare la soluzione Marketo con la connessione Controllo password proprietario risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [Passaggio 2 di 4: Configurare la soluzione Marketo con la connessione Controllo password proprietario risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
>* [Passaggio 3 di 4: Configurazione dell’app client su MS Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)


>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!IMPORTANT]
>
>Se stai effettuando l’aggiornamento dall’autenticazione di base a OAuth, dovrai contattare [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support) per informazioni sull’aggiornamento dei parametri aggiuntivi. L’abilitazione di questa funzione interrompe temporaneamente la sincronizzazione finché non vengono inserite nuove credenziali e la sincronizzazione non viene riabilitata. La funzione può essere disabilitata (fino ad aprile 2022) se desideri tornare alla vecchia modalità di autenticazione.

## Immetti le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedi a Marketo e fai clic su **Amministratore**.

   ![](assets/login-admin.png)

1. Fai clic su **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Seleziona **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Fai clic su **Modifica** in **Passaggio 1: Immettere le credenziali**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Assicurati che l’URL dell’organizzazione sia corretto in quanto non è possibile ripristinare le successive modifiche dello schema dopo l’invio. Se viene utilizzato un URL organizzazione non corretto, dovrai ottenere una nuova sottoscrizione Marketo. Se non conosci l’URL, [scopri come trovarlo qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

   >[!NOTE]
   >
   >Prima di immettere le nuove credenziali, è possibile [convalidali qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

1. Inserisci il **Nome utente**, **Password**, **ID client**, **Segreto client** e Microsoft Dynamics **URL**. Fai clic su **Salva** al termine.

   ![](assets/step-4-of-4-connect-the-marketo-solution-ropc-5.png)

   >[!NOTE]
   >
   >Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere `user@domain.com` o DOMINIO\utente.

## Seleziona campi da sincronizzare {#select-fields-to-sync}

1. Fai clic su **Modifica** in **Passaggio 2: Seleziona campi da sincronizzare**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Seleziona i campi da sincronizzare in Marketo, in modo che vengano preselezionati. Fai clic su **Salva**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo memorizza un riferimento ai campi da sincronizzare. Se elimini un campo in Dynamics, è consigliabile eseguire questa operazione con la [sincronizzazione disabilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Quindi aggiorna lo schema in Marketo modificando e salvando il [Seleziona campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Campi di sincronizzazione per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se hai creato un filtro personalizzato, assicurati di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Vai ad Amministratore e seleziona **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fai clic su **Modifica** in Dettagli sincronizzazione campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e controllalo. Il nome effettivo deve essere new_synctomkto ma il nome visualizzato può essere qualsiasi cosa. Fai clic su **Salva**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Abilita sincronizzazione {#enable-sync}

1. Fai clic su **Modifica** in **Passaggio 3: Abilita sincronizzazione**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente il deduplicazione rispetto a una sincronizzazione di Microsoft Dynamics o quando immetti manualmente persone o lead.

1. Leggi tutto nella finestra a comparsa, inserisci il tuo indirizzo e-mail e fai clic su **Avvia sincronizzazione**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine riceverai una notifica e-mail.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Ottimo lavoro!