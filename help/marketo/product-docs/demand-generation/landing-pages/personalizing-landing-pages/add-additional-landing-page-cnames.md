---
unique-page-id: 2359798
description: Aggiungere ulteriori CNAME per la pagina di destinazione - Documentazione Marketo - Documentazione del prodotto
title: Aggiungere altri CNAME alla pagina di destinazione
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 4%

---

# Aggiungere altri CNAME alla pagina di destinazione {#add-additional-landing-page-cnames}

Puoi aggiungere i CNAME della pagina di destinazione per consentire a URL diversi di puntare alle pagine di destinazione di Marketo. Segui i passaggi seguenti per gestire più domini.

>[!CAUTION]
>
>I cookie non sono condivisibili tra domini diversi.

>[!TIP]
>
>**Stesso dominio di primo livello - Buono! I cookie sono condivisi**.<br/> **vai**.mycompany.com > **info**.mycompany.com
>
>**Domini di primo livello diversi - non validi! I cookie sono _non_ condivisi**.<br/> vai.**società**.com > vai.**mionuova società**.com

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai all&#39;area **Amministratore**.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Fai clic su **Il mio account**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Scorri verso il basso fino a &quot;Informazioni di supporto&quot; e copia il tuo Munchkin ID.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Invia richiesta al reparto IT {#send-request-to-it}

1. Chiedi al tuo reparto IT di configurare il seguente CNAME: (sostituisci la parola [CNAME] con il CNAME desiderato e [Munchkin ID] con il testo del passaggio precedente).

   [CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Aggiungi un nuovo CNAME {#add-a-new-cname}

1. Una volta che il reparto IT ha creato il CNAME, vai all&#39;area **Amministratore**.

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Fai clic su **Pagine di destinazione**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Fai clic su **[!UICONTROL New]**, quindi seleziona **[!UICONTROL New Domain Alias]**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Immetti **[!UICONTROL Domain Alias].** **[!UICONTROL Default Page]** viene visualizzato se il visitatore non inserisce un URL. In tal caso, specifica il percorso da seguire.

   >[!NOTE]
   >
   >Per [!UICONTROL Default Page], è possibile selezionare una pagina di destinazione o un URL esterno, ad esempio il sito Web pubblico.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Immetti **[!UICONTROL Default Page]** e fai clic su **[!UICONTROL Create]**.

   ![](assets/add-additional-landing-page-cnames-8.png)

Bello! Ora sai cosa fare se mai vorrai aggiungere un CNAME.
