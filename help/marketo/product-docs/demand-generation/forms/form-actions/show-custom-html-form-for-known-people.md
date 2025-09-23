---
unique-page-id: 2359644
description: Mostra HTML Form personalizzato per utenti noti - Documentazione di Marketo - Documentazione del prodotto
title: Mostrare un modulo HTML personalizzato per utenti noti
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 7%

---

# Mostrare un modulo HTML personalizzato per utenti noti {#show-custom-html-form-for-known-people}

Se in passato un visitatore ha fornito il suo nome completo e il suo indirizzo e-mail e non vuoi che riceva l’intero modulo, scopri come mostrare loro un HTML personalizzato (ad esempio, un pulsante per il download).

1. Vai a **[!UICONTROL Marketing Activities]**.

   ![](assets/login-marketing-activities-5.png)

1. In **[!UICONTROL Marketing Activities]**, selezionare il modulo e fare clic su **[!UICONTROL Edit Form]**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. In **[!UICONTROL Form Settings]**, fare clic su **[!UICONTROL Settings]**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Imposta se **[!UICONTROL Known Visitor, Show]**: su **[!UICONTROL Custom HTML]**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Fai clic su ![—](assets/image2014-9-25-14-3a1-3a26.png) per modificare **[!UICONTROL Custom HTML]** che verrà mostrato a persone note.

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

1. Fai clic su **[!UICONTROL Finish]**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Fai clic su **[!UICONTROL Approve and Close]**.

   >[!NOTE]
   >
   >Il modulo deve essere approvato per essere utilizzato nelle pagine di destinazione.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >Ricorda di [approvare la bozza della pagina di destinazione](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) creata dalle modifiche del modulo.

   Un pezzo di torta! Scopri cosa vedrebbe una persona se tornasse allo stesso modulo:

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Per indirizzare il clic del pulsante alla risorsa, imposta la pagina di follow-up del modulo sull’URL del file.
