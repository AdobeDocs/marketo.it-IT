---
unique-page-id: 2359798
description: Aggiungere CNAME aggiuntivi per pagina di destinazione - Documenti Marketo - Documentazione prodotto
title: Aggiunta di CNAME aggiuntivi per pagine di destinazione
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---


# Aggiungi CNAME di pagina di destinazione aggiuntivi {#add-additional-landing-page-cnames}

È possibile aggiungere CNAME di pagina di destinazione per consentire a diversi URL di puntare alle pagine di destinazione Marketo. Seguendo i passaggi indicati di seguito potrai gestire più domini.

>[!CAUTION]
>
>I cookie non sono condivisibili tra domini diversi.

>[!TIP]
>
>**Stesso dominio di primo livello - Buono! I cookie sono condivisi**.<br/> **go**.mycompany.com >  **info**.mycompany.com
>
>**Diversi domini di primo livello - Scorretto! I cookie sono _non_ condivisi**.<br/> vai.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Trova la stringa account {#find-your-account-string}

1. Andate nell&#39;area **Admin** e fate clic su **Pagine di destinazione**.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. Copiare la **Stringa account** dalla sezione **Settings**.

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. Prendetene nota per il passaggio successivo.

## Invia richiesta all&#39;IT {#send-request-to-it}

1. Chiedi al reparto IT di configurare il CNAME seguente: (Sostituite la parola [CNAME] con il CNAME di vostra scelta e [ACCOUNT STRING] con il testo del passaggio precedente).

   [CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

## Aggiungere un nuovo CNAME {#add-a-new-cname}

1. Una volta che il reparto IT ha creato il CNAME, andate a **Admin** e fate clic su **Pagine di destinazione**.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. Fare clic su **New**, quindi selezionare **New Domain Alias**.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. Immettere l&#39; **Alias di dominio.** La  **pagina** predefinita viene visualizzata se il visitatore non inserisce un URL. Inserire dove devono andare in quel caso.

   >[!NOTE]
   >
   >Per Pagina predefinita, potete selezionare una pagina di destinazione o un URL esterno, ad esempio il sito Web pubblico.

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. Immettere la **pagina predefinita** e fare clic su **Crea**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

Bello! Ora sai cosa fare se vuoi aggiungere un CNAME.
