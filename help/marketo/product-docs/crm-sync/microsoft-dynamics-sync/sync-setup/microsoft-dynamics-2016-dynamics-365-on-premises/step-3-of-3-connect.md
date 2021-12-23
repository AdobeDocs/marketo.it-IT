---
unique-page-id: 7504744
description: Installare Marketo per Microsoft Dynamics 2016/Dynamics 365 On-Premises Passaggio 3 di 3 - Documentazione Marketo - Documentazione del prodotto
title: Installare Marketo per Microsoft Dynamics 2016/Dynamics 365 On-Premises, passaggio 3 di 3
exl-id: 054bf725-7a80-4114-8360-2d86e2e33dd7
source-git-commit: 1e20fdd1d3c6bba265ceabe499e0d7a4babf4ef1
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Passaggio 3 di 3: Connetti Marketo Dynamics (2016 On Prem/Dynamics 365 On-Premises) {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [Installare Marketo per Microsoft Dynamics 2016/Dynamics 365 On-Premises, passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)
>* [Installare Marketo per Microsoft Dynamics 2016/Dynamics 365 On-Premises, passaggio 2 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immetti le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedi a Marketo e fai clic su **Amministratore**.

   ![](assets/login-admin.png)

1. Fai clic su **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Seleziona **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Fai clic su **Modifica** in **Passaggio 1: Immettere le credenziali**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Assicurati che le tue credenziali siano corrette in quanto non è possibile ripristinare le successive modifiche dello schema dopo l’invio. Se vengono salvate le credenziali errate, sarà necessario ottenere una nuova sottoscrizione Marketo.

1. Inserisci il **Nome utente**, **Password** a Microsoft Dynamics **URL** e **ID client/segreto**. Fai clic su **Salva** al termine.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* Se il provisioning del tuo Marketo è stato eseguito prima di ottobre 2020, gli ID client e il segreto sono campi facoltativi. Altrimenti, sono obbligatori. L&#39;ottenimento di queste informazioni dipenderà dalla versione di MSD in uso.
   >* Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere `user@domain.com` o DOMINIO\utente.
   >* Se non conosci l’URL, [scopri come trovarlo qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


   >[!TIP]
   >
   >Non conosce l&#39;URL? Ti mostreremo come trovare il tuo [URL del servizio dell’organizzazione Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) qui.

## Seleziona campi da sincronizzare {#select-fields-to-sync}

1. Fai clic su **Modifica** in **Passaggio 2: Seleziona campi da sincronizzare**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Seleziona i campi da sincronizzare in Marketo, in modo che vengano preselezionati. Fai clic su **Salva**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

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

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Abilita sincronizzazione {#enable-sync}

1. Fai clic su **Modifica** in **Passaggio 3: Abilita sincronizzazione**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente il deduplicazione rispetto a una sincronizzazione Microsoft Dynamics o quando immetti manualmente le persone.

1. Leggi tutto nella finestra a comparsa, inserisci il tuo messaggio e-mail e fai clic su **Avvia sincronizzazione**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine riceverai una notifica e-mail.

   ![](assets/image2015-3-16-9-59-51.png)

Ottimo lavoro!
