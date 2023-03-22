---
unique-page-id: 2359798
description: Aggiungere CNAME aggiuntivi per le pagine di destinazione - Documenti Marketo - Documentazione del prodotto
title: Aggiungi CNAME aggiuntivi per pagine di destinazione
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: tm+mt
source-wordcount: '234'
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

1. Vai a **Amministratore** area.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Fai clic su **Il mio account**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Scorri verso il basso fino a &quot;Informazioni di supporto&quot; e copia il tuo Munchkin ID.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Invia richiesta all&#39;IT {#send-request-to-it}

1. Chiedi al tuo reparto IT di configurare il seguente CNAME: (Sostituisci la parola [CNAME] con il CNAME di tua scelta e [ID Munchkin] con il testo del passaggio precedente).

   [CNAME].YourCompany.com > [ID Munchkin].mktoweb.com

## Aggiungi un nuovo CNAME {#add-a-new-cname}

1. Una volta che il reparto IT ha creato il CNAME, vai al **Amministratore** area.

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Fai clic su **Pagine di destinazione**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Fai clic su **Nuovo** quindi seleziona **Nuovo alias di dominio**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Inserisci il tuo **Alias di dominio.** La **Pagina predefinita** viene visualizzato se il visitatore non inserisce un URL. Inserisci dove dovrebbero andare in quel caso.

   >[!NOTE]
   >
   >Per la pagina predefinita, puoi selezionare una pagina di destinazione o un URL esterno, ad esempio il tuo sito web pubblico.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Inserisci il tuo **Pagina predefinita** e fai clic su **Crea**.

   ![](assets/add-additional-landing-page-cnames-8.png)

Bello! Ora sai cosa fare se vuoi aggiungere un CNAME.
