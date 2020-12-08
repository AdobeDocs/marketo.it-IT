---
unique-page-id: 2359798
description: Aggiungere CNAME aggiuntivi per pagina di destinazione - Documenti Marketo - Documentazione prodotto
title: Aggiunta di CNAME aggiuntivi per pagine di destinazione
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# Aggiunta di CNAME aggiuntivi per pagine di destinazione {#add-additional-landing-page-cnames}

È possibile aggiungere CNAME di pagina di destinazione per consentire a diversi URL di puntare alle pagine di destinazione Marketo. Seguendo i passaggi indicati di seguito potrai gestire più domini.

>[!CAUTION]
>
>I cookie non sono condivisibili tra domini diversi.

>[!TIP]
>
>**Stesso dominio di primo livello - Buono! I cookie sono shared.go**.mycompany.com > **info**.mycompany.**comDiversi domini di primo livello - Bad! I cookie non sono condivisi.**
>vai.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Trova la stringa account {#find-your-account-string}

1. Andate nell&#39;area **Admin** e fate clic su Pagine **di** destinazione.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. Copiate la stringa **** account dalla sezione **Impostazioni** .

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. Prendetene nota per il passaggio successivo.

## Invia richiesta all&#39;IT {#send-request-to-it}

1. Chiedi al reparto IT di configurare il CNAME seguente: (Sostituite la parola [CNAME] con il CNAME di vostra scelta e la stringa [] ACCOUNT con il testo del passaggio precedente).

   [CNAME].YourCompany.com > [ACCOUNT STRING].mktoweb.com

## Aggiungere un nuovo CNAME {#add-a-new-cname}

1. Dopo che il reparto IT ha creato il CNAME, vai in **Admin** e fai clic su Pagine **di** destinazione.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. Fare clic su **Nuovo** , quindi selezionare **Nuovo alias** dominio.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. Immettere l&#39;alias **di dominio.** La pagina **** predefinita viene visualizzata se il visitatore non inserisce un URL. Inserire dove devono andare in quel caso.

   >[!NOTE]
   >
   >Per Pagina predefinita, potete selezionare una pagina di destinazione o un URL esterno, ad esempio il sito Web pubblico.

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. Inserite la pagina **** predefinita e fate clic su **Crea**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

Bello! Ora sai cosa fare se vuoi aggiungere un CNAME.
