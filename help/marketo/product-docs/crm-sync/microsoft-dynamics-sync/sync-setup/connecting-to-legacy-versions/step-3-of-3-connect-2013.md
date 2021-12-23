---
unique-page-id: 3571819
description: 'Passaggio 3 di 3: collegare Marketo e Dynamics (On-Premises 2013) - Documentazione Marketo - Documentazione del prodotto'
title: 'Passaggio 3 di 3: collegare Marketo e Dynamics (On-Premises 2013)'
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Passaggio 3 di 3: Collegare Marketo e Dynamics (On-Premises 2013) {#step-of-connect-marketo-and-dynamics-on-premises}

Bene! Abbiamo installato la soluzione e configurato l&#39;utente di sincronizzazione. Successivamente, è necessario collegare Marketo e Dynamics.

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: Installare la soluzione Marketo in Dynamics (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)
>* [Passaggio 2 di 3: Configura l’utente di sincronizzazione per Marketo (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-2-of-3-configure.md)


>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immetti le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedi a Marketo e fai clic su **Amministratore**.

   ![](assets/login-admin.png)

1. Fai clic su **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Seleziona **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Fai clic su **Modifica** in **Passaggio 1: Immettere le credenziali**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Assicurati che le tue credenziali siano corrette in quanto non è possibile ripristinare le successive modifiche dello schema dopo l’invio. Se vengono salvate le credenziali errate, sarà necessario ottenere una nuova sottoscrizione Marketo.

1. Inserisci il **Nome utente**, **Password** e Microsoft Dynamics **URL** quindi fai clic su **Salva**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere user@domain.com o DOMAIN\user.
   >* Se non conosci l’URL, [scopri come trovarlo qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## Seleziona campi da sincronizzare {#select-fields-to-sync}

Ora è necessario selezionare i campi su cui si desidera eseguire la sincronizzazione.

1. Fai clic su **Modifica** in **Passaggio 2: Seleziona campi da sincronizzare**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Seleziona i campi da sincronizzare in Marketo, in modo che vengano preselezionati. Fai clic su **Salva**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

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

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Abilita sincronizzazione {#enable-sync}

1. Fai clic su **Modifica** in **Passaggio 3: Abilita sincronizzazione**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente il deduplicazione rispetto a una sincronizzazione di Microsoft Dynamics o quando immetti manualmente persone o lead.

1. Leggi tutto nella finestra a comparsa, inserisci il tuo messaggio e-mail e fai clic su **Avvia sincronizzazione**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine riceverai una notifica e-mail.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

Ottimo lavoro! Hai appena liberato la potenza della sincronizzazione bidirezionale tra Marketo e Microsoft Dynamics. Se hai acquistato Marketo Sales Insight, è più divertente avere:

>[!MORELIKETHIS]
>
>[Installazione e configurazione di Marketo Sales Insight in Microsoft Dynamics 2013](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
