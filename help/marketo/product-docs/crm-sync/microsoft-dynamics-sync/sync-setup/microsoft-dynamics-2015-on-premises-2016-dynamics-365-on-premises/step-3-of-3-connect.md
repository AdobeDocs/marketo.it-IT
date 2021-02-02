---
unique-page-id: 7504744
description: Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 3 di 3 - Marketo Docs - Documentazione prodotto
title: Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 3 di 3
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# Passaggio 3 di 3: Connect Marketo Dynamics (On-Prem 2015 e On-Prem 2016 365) {#step-of-connect-marketo-dynamics-on-premises-and-365}

>[!PREREQUISITES]
>
>* [Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)
>* [Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 2 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immettere le informazioni sull&#39;utente di sincronizzazione delle dinamiche {#enter-dynamics-sync-user-information}

1. Accedete a Marketo e fate clic su **Admin**.

   ![](assets/login-admin.png)

1. Fare clic su **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Selezionare **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Fare clic su **Modifica** in **Passaggio 1: Immettere Credentials**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Verificate che le credenziali siano corrette in quanto non sarà possibile ripristinare le modifiche successive dello schema dopo l&#39;invio. Se vengono salvate credenziali errate, dovrete ottenere una nuova iscrizione a Marketo.

1. Immettete il **Nome utente**, **Password** in Microsoft Dynamics **URL** e un **ID client** facoltativo. Fare clic su **Salva** al termine.

   ![](assets/client-id.png)

   >[!NOTE]
   >
   >Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere user@domain.com o DOMINIO\utente.

   >[!TIP]
   >
   >Non conosci l&#39;URL? Verrà illustrato come trovare l&#39; [URL del servizio di organizzazione dinamica](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) qui.

## Selezionare i campi da sincronizzare {#select-fields-to-sync}

1. Fare clic su **Modifica** in **Passaggio 2: Selezionare Campi da sincronizzare**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Selezionate i campi che desiderate sincronizzare con Marketo, in modo che siano preselezionati. Fare clic su **Salva**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

## Campi di sincronizzazione per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se avete creato un filtro personalizzato, accertatevi di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Accedi ad Admin e seleziona **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fare clic su **Modifica** in Dettagli sincronizzazione campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e controllalo. Il nome effettivo deve essere new_synctomkto, ma il nome visualizzato può essere qualsiasi cosa. Fare clic su **Salva**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Abilita sincronizzazione {#enable-sync}

1. Fare clic su **Modifica** in **Passaggio 3: Abilita Sync**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione rispetto a una sincronizzazione di Microsoft Dynamics o quando immetti manualmente le persone.

1. Leggete tutto nella finestra a comparsa, inserite il messaggio e-mail e fate clic su **Avvia sincronizzazione**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine, riceverete una notifica e-mail.

   ![](assets/image2015-3-16-9-59-51.png)

Ottimo lavoro!
