---
unique-page-id: 2359644
description: Mostra modulo di HTML personalizzato per utenti noti - Documentazione di Marketo - Documentazione del prodotto
title: Mostra modulo HTML personalizzato per utenti noti
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Mostra modulo HTML personalizzato per utenti noti {#show-custom-html-form-for-known-people}

Se un visitatore è cookie (persona nota che ha fornito un indirizzo e-mail in passato), perché preoccuparsi del modulo? Date loro il pulsante per il download. Ecco come.

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-5.png)

1. Sotto **Attività di marketing**, seleziona il modulo e fai clic su **Modifica modulo**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Sotto **Impostazioni modulo**, fai clic su **Impostazioni**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Imposta se **Visitatore noto, Mostra**: a **Personalizza HTML**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Fai clic su ![—](assets/image2014-9-25-14-3a1-3a26.png) per modificare **Personalizza HTML** sarà mostrato a persone conosciute.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. È presente del contenuto predefinito, ma puoi modificarlo.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Token disponibili:

   | Token | Descrizione |
   |---|---|
   | `{{lead.FirstName}}` | In questo modo verrà visualizzato il nome della persona. |
   | `{{lead.LastName}}` | Verrà visualizzato il cognome della persona. |
   | `{{form.Button:default=Download}}` | Verrà visualizzato il pulsante del modulo. Sostituire l&#39;area dopo `=` per modificare il testo del pulsante. |
   | `{{form.NotYou:default=Not you?}}` | Se la persona è qualcun altro, verrà visualizzato un collegamento. Sostituire l&#39;area dopo `=` per modificare il testo del collegamento. |

   >[!CAUTION]
   >
   >È possibile utilizzare solo i quattro token indicati sopra. Qualsiasi altro token non funzionerà qui.

1. Clic **Fine**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Clic **Approva e chiudi**.

   >[!NOTE]
   >
   >Il modulo deve essere approvato per essere utilizzato nelle pagine di destinazione.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >Ricorda a [approva la bozza della pagina di destinazione](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) create dalle modifiche apportate al modulo.

   Un pezzo di torta! Scopri cosa vedrebbe una persona se tornasse allo stesso modulo:

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Per indirizzare il clic del pulsante alla risorsa, imposta la pagina di follow-up del modulo sull’URL del file.
