---
unique-page-id: 2359644
description: Mostra modulo HTML personalizzato per le persone note - Documenti Marketo - Documentazione prodotto
title: Mostra modulo HTML personalizzato per le persone note
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---


# Mostra modulo HTML personalizzato per le persone note {#show-custom-html-form-for-known-people}

Se un visitatore riceve un cookie (persona nota che in passato ha fornito un indirizzo e-mail), perché preoccuparsi del modulo? Basta dare loro il pulsante di download. Ecco come.

1. Andate a **Marketing** **Activities**.

   ![](assets/login-marketing-activities-5.png)

1. In **Marketing** **Attività**, selezionare il modulo e fare clic su **Modifica** **Modulo**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. In **Form** **Settings**, fare clic su **Settings**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Impostate Se **Noto** **Visitatore, Mostra**: su **Custom** **HTML**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Fare clic su ![—](assets/image2014-9-25-14-3a1-3a26.png) per modificare il **Custom** **HTML** che verrà mostrato alle persone conosciute.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Esistono contenuti predefiniti, ma non esitate a modificarli.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Token disponibili:

   | Token | Descrizione |
   |---|---|
   | `{{lead.FirstName}}` | Verrà visualizzato il nome della persona. |
   | `{{lead.LastName}}` | Verrà visualizzato il cognome della persona. |
   | `{{form.Button:default=Download}}` | Verrà visualizzato il pulsante del modulo. Sostituire l&#39;area dopo la `=` per modificare il testo del pulsante. |
   | `{{form.NotYou:default=Not you?}}` | In questo modo verrà visualizzato un collegamento nel caso in cui la persona sia qualcun altro. Sostituire l&#39;area dopo la `=` per modificare il testo del collegamento. |

   >[!CAUTION]
   >
   >È possibile utilizzare solo i quattro token indicati sopra. Qualsiasi altro token non funzionerà qui.

1. Fare clic su **Fine**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Fare clic su **Approva e Chiudi**.

   >[!NOTE]
   >
   >Il modulo deve essere approvato per essere utilizzato sulle pagine di destinazione.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >**Promemoria**
   >
   >
   >Ricordare di [approvare la bozza della pagina di destinazione](../../../../product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) creata dalle modifiche al modulo.

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Per indirizzare il clic del pulsante alla risorsa, impostare la pagina di follow-up del modulo sull’URL del file.

Pezzo di torta! Controlla cosa vedrebbe una persona se tornasse allo stesso modulo: