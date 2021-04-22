---
unique-page-id: 2360245
description: Rimuovi il testo dell’annullamento dell’abbonamento dalla sezione e-mail dell’amministratore - Documenti Marketo - Documentazione del prodotto
title: Rimuovi il testo dell’annullamento dell’abbonamento dalla sezione e-mail dell’amministratore
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# Rimuovi il testo dell’annullamento dell’abbonamento dalla sezione e-mail dell’amministratore {#remove-unsubscribe-text-from-the-admin-email-section}

L’unico motivo per cui devi rimuovere completamente il contenuto dell’annullamento dell’abbonamento dall’area &quot;Amministratore > E-mail&quot; è la scelta di creare il collegamento per l’annullamento dell’abbonamento nei modelli e-mail stessi. La casella di testo presenta una convalida che non consente di salvare senza contenuto. Per aggirare questo problema, aggiungi un piccolo commento HTML. Il commento HTML non viene visualizzato nel client e-mail, perché esegue il rendering dell’e-mail in HTML e i commenti vengono omessi. Ecco come farlo.

1. Vai a **Amministratore** e fai clic su **E-mail**.

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. Seleziona tutto il testo e premi il tasto **Elimina**.

   >[!CAUTION]
   >
   >Prima di eliminare, copiarlo/incollarlo in un documento di testo come backup.

1. Digita `<!--This is a comment -->`.

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. Fare clic su **Salva modifiche**.

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>Per il **Annulla sottoscrizione testo** è necessario aggiungere un singolo carattere. Utilizza un trattino o un punto.
