---
unique-page-id: 3571830
description: Passaggio 3 di 3 - Connetti Microsoft Dynamics con Marketo (Online) - Marketo Docs - Documentazione prodotto
title: Passaggio 3 di 3 - Connetti Microsoft Dynamics con Marketo (online)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---


# Passaggio 3 di 3: Connetti Microsoft Dynamics con Marketo (online) {#step-of-connect-microsoft-dynamics-with-marketo-online}

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

Questo è l&#39;ultimo passaggio della sincronizzazione. Siamo quasi lì!

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: Installazione della soluzione Marketo (online)](step-1-of-3-install.md)
   >
   >
* [Passaggio 2 di 3: Impostazione di Marketo Sync User in Dynamics](step-2-of-3-set-up.md)

>



>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immettere le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedi a Marketo e fai clic su **Admin**.

   ![](assets/login-admin.png)

1. Fate clic su **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Selezionare **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Fate clic su **Modifica** nel **passaggio 1: Immettere le credenziali**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Verificate che le credenziali siano corrette in quanto non sarà possibile ripristinare le modifiche successive dello schema dopo l&#39;invio. Se vengono salvate credenziali errate, dovrete ottenere una nuova iscrizione a Marketo.

1. Immettete il **nome** utente, la **password** e l&#39; **URL** di Microsoft Dynamics (ID client e Segreto cliente sono facoltativi). Al termine, fate clic su **Salva** .

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#bcc9cfd9cefcd8d3d1ddd5d292dfd3d1) o DOMINIO\utente.

## Seleziona campi da sincronizzare {#select-fields-to-sync}

1. Fate clic su **Modifica** nel **passaggio 2: Selezionare Campi da sincronizzare**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Selezionate i campi che desiderate sincronizzare con Marketo, in modo che siano preselezionati. Fate clic su **Salva**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

## Campi di sincronizzazione per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se avete creato un filtro personalizzato, accertatevi di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Vai ad Admin e seleziona **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fate clic su **Modifica** in Dettagli sincronizzazione campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e controllalo. Il nome effettivo deve essere new_synctomkto, ma il nome visualizzato può essere qualsiasi cosa. Fate clic su **Salva**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Abilita sincronizzazione {#enable-sync}

1. Fate clic su **Modifica** nel **passaggio 3: Abilita sincronizzazione**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione rispetto a una sincronizzazione di Microsoft Dynamics, o quando immetti manualmente persone o lead.

1. Leggete tutto nella finestra a comparsa, inserite il vostro indirizzo e-mail e fate clic su **Avvia sincronizzazione**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine, riceverete una notifica e-mail.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Ottimo lavoro!
