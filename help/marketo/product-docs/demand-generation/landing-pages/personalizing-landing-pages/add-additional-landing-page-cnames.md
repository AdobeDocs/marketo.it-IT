---
unique-page-id: 2359798
description: Aggiungere CNAME aggiuntivi per le pagine di destinazione - Documenti Marketo - Documentazione del prodotto
title: Aggiungi CNAME aggiuntivi per pagine di destinazione
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Aggiungi CNAME aggiuntivi per pagine di destinazione {#add-additional-landing-page-cnames}

Puoi aggiungere CNAME per pagine di destinazione per consentire a URL diversi di puntare alle pagine di destinazione di Marketo. Seguendo i passaggi seguenti potrai gestire più domini.

>[!CAUTION]
>
>I cookie non sono condivisibili tra i domini.

>[!TIP]
>
>**Stesso dominio di primo livello - Buono! I cookie sono condivisi**.<br/> **andare**.mycompany.com > **info**.miasocietà.com
>
>**Diversi domini di primo livello - Cattivo! I cookie sono _not_ condiviso**.<br/> vai.**mia azienda**.com > vai.**mynewcompany**.com

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Trova La Stringa Account {#find-your-account-string}

1. Vai a **Amministratore** area e fai clic su **Pagine di destinazione**.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. Copia il **Stringa account** dal **Impostazioni** sezione .

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. Prendi nota del passaggio successivo.

## Invia richiesta all&#39;IT {#send-request-to-it}

1. Chiedi al tuo reparto IT di configurare il seguente CNAME: (Sostituisci la parola [CNAME] con il CNAME di tua scelta e [STRINGA ACCOUNT] con il testo del passaggio precedente).

   [CNAME].YourCompany.com > [STRINGA ACCOUNT].mktoweb.com

## Aggiungi un nuovo CNAME {#add-a-new-cname}

1. Una volta creato il CNAME dal reparto IT, vai a **Amministratore** quindi fai clic su **Pagine di destinazione**.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. Fai clic su **Nuovo** quindi seleziona **Nuovo alias di dominio**.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. Inserisci il tuo **Alias di dominio.** La **Pagina predefinita** viene visualizzato se il visitatore non inserisce un URL. Inserisci dove dovrebbero andare in quel caso.

   >[!NOTE]
   >
   >Per la pagina predefinita, puoi selezionare una pagina di destinazione o un URL esterno, ad esempio il tuo sito web pubblico.

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. Inserisci il tuo **Pagina predefinita** e fai clic su **Crea**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

Bello! Ora sai cosa fare se vuoi aggiungere un CNAME.
