---
unique-page-id: 3571819
description: Passaggio 3 di 3 - Connect Marketo e Dynamics (On-Premises 2013) - Marketo Docs - Documentazione prodotto
title: Passaggio 3 di 3 - Connect Marketo e Dynamics (On-Premises 2013)
translation-type: tm+mt
source-git-commit: ce8b67b8549d23ff4ddd1d341632c6c5ff33990d
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---


# Passaggio 3 di 3: Connect Marketo e Dynamics (On-Premises 2013) {#step-of-connect-marketo-and-dynamics-on-premises}

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

Bene! Abbiamo installato la soluzione e configurato l&#39;utente di sincronizzazione. Quindi, dobbiamo collegare Marketo e Dynamics.

>[!NOTE]
>
>**Prerequisiti**
>
>* [Passaggio 1 di 3: Installare la soluzione Marketo in Dynamics (On-Premises 2013)](step-1-of-3-install.md)
>* [Passaggio 2 di 3: Configurare l&#39;utente di sincronizzazione per Marketo (On-Premises 2013)](step-2-of-3-configure.md)

>



>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immettere le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedi a Marketo e fai clic su **Admin**.

   ![](assets/login-admin.png)

1. Fate clic su **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Selezionare **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Fate clic su **MODIFICA** nel **passaggio 1: Immettere le credenziali**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Verificate che le credenziali siano corrette in quanto non sarà possibile ripristinare le modifiche successive dello schema dopo l&#39;invio. Se vengono salvate credenziali errate, dovrete ottenere una nuova iscrizione a Marketo.

1. Immettete il **nome** utente, la **password** e l’ **URL** di Microsoft Dynamics, quindi fate clic su **SALVA**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#631610061123070c0e020a0d4d000c0e) o DOMINIO\utente.

   >[!TIP]
   >
   >Non conosci l&#39;URL? Verrà mostrato come trovare l&#39;URL [del servizio](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) Dynamics Organization.

## Seleziona campi da sincronizzare {#select-fields-to-sync}

Ora è necessario selezionare i campi sui quali eseguire la sincronizzazione.

1. Fare clic su **EDIT **al **passaggio 2: Selezionare Campi da sincronizzare**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Selezionate i campi che desiderate sincronizzare con Marketo, in modo che siano preselezionati. Fate clic su **Salva**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

## Campi di sincronizzazione per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se avete creato un filtro personalizzato, accertatevi di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Vai ad Admin e seleziona **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fate clic su **Modifica** in Dettagli sincronizzazione campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e controllalo. Il nome effettivo deve essere new_synctomkto, ma il nome visualizzato può essere qualsiasi cosa. Fate clic su **Salva**.

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Abilita sincronizzazione {#enable-sync}

1. Fare clic su **EDIT **al **punto 3: Abilita sincronizzazione**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione rispetto a una sincronizzazione di Microsoft Dynamics, o quando immetti manualmente persone o lead.

1. Leggete tutto nella finestra a comparsa, inserite il messaggio e-mail e fate clic su **START SYNC**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine, riceverete una notifica e-mail.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

Ottimo lavoro! Hai appena liberato la potenza della sincronizzazione bidirezionale tra Marketo e Microsoft Dynamics. Se hai acquistato Marketo Sales Insight, c&#39;è più divertimento da avere:

>[!NOTE]
>
>**Articoli correlati**
>
>* [Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 2013](../../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)

>



