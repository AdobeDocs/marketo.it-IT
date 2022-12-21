---
unique-page-id: 2359644
description: Mostra modulo HTML personalizzato per utenti noti - Documenti Marketo - Documentazione del prodotto
title: Mostra modulo HTML personalizzato per persone note
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Mostra modulo HTML personalizzato per persone note {#show-custom-html-form-for-known-people}

Se un visitatore riceve un cookie (persona nota che in passato ha fornito un indirizzo e-mail), perché preoccuparsi del modulo? Date loro il pulsante di download. Ecco come.

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-5.png)

1. Sotto **Attività di marketing**, seleziona il modulo e fai clic su **Modifica modulo**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Sotto **Impostazioni modulo**, fai clic su **Impostazioni**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Imposta se **Visitatore noto, Mostra**: a **HTML personalizzato**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Fai clic sul pulsante ![—](assets/image2014-9-25-14-3a1-3a26.png) per modificare **HTML personalizzato** che verrà mostrato alle persone conosciute.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. C&#39;è del contenuto predefinito, ma sentitevi liberi di modificarlo.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Token disponibili:

   | Token | Descrizione |
   |---|---|
   | `{{lead.FirstName}}` | Verrà visualizzato il nome della persona. |
   | `{{lead.LastName}}` | Verrà visualizzato il cognome della persona. |
   | `{{form.Button:default=Download}}` | Verrà visualizzato il pulsante del modulo. Sostituisci l’area dopo la `=` per modificare il testo del pulsante. |
   | `{{form.NotYou:default=Not you?}}` | In questo modo verrà visualizzato un collegamento nel caso in cui la persona sia qualcun altro. Sostituisci l’area dopo la `=` per modificare il testo del collegamento. |

   >[!CAUTION]
   >
   >È possibile utilizzare solo i quattro token indicati sopra. Qualsiasi altro token non funzionerà qui.

1. Fai clic su **Fine**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Fai clic su **Approva e chiudi**.

   >[!NOTE]
   >
   >Il modulo deve essere approvato per essere utilizzato nelle pagine di destinazione.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >Ricorda di [approva la bozza della pagina di destinazione](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) creato dalle modifiche al modulo.

   Pezzo di torta! Controlla cosa vedrebbe una persona se tornasse allo stesso modulo:

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Puoi indirizzare il clic del pulsante alla risorsa impostando la pagina di follow-up del modulo sull’URL del file.
