---
unique-page-id: 2359644
description: Mostra Modulo HTML personalizzato per persone conosciute - Marketo Docs - Product Documentazione
title: Mostra modulo HTML personalizzato per persone conosciute
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 55964499f5d49258539492f952513833af5692b5
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 1%

---

# Mostra modulo HTML personalizzato per persone conosciute {#show-custom-html-form-for-known-people}

Se un visitatore ha fornito il proprio nome completo e indirizzo e-mail in passato e non si desidera che riceva l&#39;intero modulo, scopri come mostrargli un HTML personalizzato (ad esempio, solo un scaricare pulsante).

1. Vai ad Attività&#x200B;**di** marketing.

   ![](assets/login-marketing-activities-5.png)

1. In **Attività** marketing selezionare il modulo e fare clic su **Modifica modulo**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. In **Impostazioni** modulo, fare clic su **Impostazioni**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Imposta se **visitatore conosciuto, Mostra**: su **HTML** personalizzato.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Fai clic su ![--](assets/image2014-9-25-14-3a1-3a26.png) per modificare il **codice HTML** personalizzato che verrà mostrato alle persone conosciute.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. C&#39;è qualche contenuto predefinita, ma sentiti gratuito di cambiarla.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Token disponibili:

   | Token | Descrizione |
   |---|---|
   | `{{lead.FirstName}}` | Verrà visualizzato il nome della persona. |
   | `{{lead.LastName}}` | Verrà visualizzato il cognome della persona. |
   | `{{form.Button:default=Download}}` | Il modulo verrà visualizzato pulsante. Sostituisci l&#39;area dopo il per `=` modificare il testo pulsante. |
   | `{{form.NotYou:default=Not you?}}` | Verrà visualizzato un collegare nel caso in cui la persona sia qualcun altro. Sostituisci l&#39;area dopo il per `=` modificare il testo collegare. |

   >[!CAUTION]
   >
   >È possibile utilizzare solo i quattro token di cui sopra. Qualsiasi altro token non funzionerà qui.

1. Fai clic su **Fine**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Fai clic su **Approva e Chiudi**.

   >[!NOTE]
   >
   >Il modulo deve essere approvato per essere utilizzato nelle pagine di destinazione.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >Ricordati di [approvare la bozza](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) della pagina di destinazione creata dalle modifiche al modulo.

   Gioco da ragazzi! Scopri cosa vedrebbe una persona se tornasse allo stesso modulo:

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >È possibile indirizzare il clic del pulsante al risorsa impostando la pagina di seguire up del modulo sul URL del file.
