---
unique-page-id: 3571830
description: Passaggio 3 di 3 - Connetti Microsoft Dynamics con Marketo (Online) - Marketo Docs - Documentazione prodotto
title: Passaggio 3 di 3 - Connetti Microsoft Dynamics con Marketo (online)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# Passaggio 3 di 3: Connetti Microsoft Dynamics con Marketo (online) {#step-of-connect-microsoft-dynamics-with-marketo-online}

Questo è l&#39;ultimo passaggio della sincronizzazione. Siamo quasi lì!

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: Installazione della soluzione Marketo (online)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)
   >
   >
* [Passaggio 2 di 3: Impostazione di Marketo Sync User in Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immettere le informazioni sull&#39;utente di sincronizzazione delle dinamiche {#enter-dynamics-sync-user-information}

1. Accedete a Marketo e fate clic su **Admin**.

   ![](assets/login-admin.png)

1. Fare clic su **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Selezionare **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Fare clic su **Modifica** in **Passaggio 1: Immettere Credentials**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Verificate che le credenziali siano corrette in quanto non sarà possibile ripristinare le modifiche successive dello schema dopo l&#39;invio. Se vengono salvate credenziali errate, dovrete ottenere una nuova iscrizione a Marketo.

1. Immettere **Nome utente**, **Password** e Microsoft Dynamics **URL** (ID client e Segreto cliente sono facoltativi). Fare clic su **Salva** al termine.

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere user@domain.com o DOMINIO\utente.

## Selezionare i campi da sincronizzare {#select-fields-to-sync}

1. Fare clic su **Modifica** in **Passaggio 2: Selezionare Campi da sincronizzare**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Selezionate i campi che desiderate sincronizzare con Marketo, in modo che siano preselezionati. Fare clic su **Salva**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

## Campi di sincronizzazione per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se avete creato un filtro personalizzato, accertatevi di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Accedi ad Admin e seleziona **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fare clic su **Modifica** in Dettagli sincronizzazione campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e controllalo. Il nome effettivo deve essere new_synctomkto, ma il nome visualizzato può essere qualsiasi cosa. Fare clic su **Salva**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Abilita sincronizzazione {#enable-sync}

1. Fare clic su **Modifica** in **Passaggio 3: Abilita Sync**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione rispetto a una sincronizzazione di Microsoft Dynamics, o quando immetti manualmente persone o lead.

1. Leggete tutto nella finestra a comparsa, inserite il vostro indirizzo e-mail e fate clic su **Avvia sincronizzazione**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine, riceverete una notifica e-mail.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Ottimo lavoro!
