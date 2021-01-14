---
unique-page-id: 2360245
description: Rimuovi Testo Di Annulla Iscrizione Dalla Sezione E-Mail Amministratore - Documenti Marketo - Documentazione Del Prodotto
title: Rimuovi Testo Da Annulla Iscrizione Dalla Sezione E-Mail Dell’Amministratore
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Rimuovi testo di annullamento sottoscrizione dalla sezione e-mail amministratore {#remove-unsubscribe-text-from-the-admin-email-section}

L’unico motivo per cui devi rimuovere completamente il contenuto dell’iscrizione dall’area &quot;Amministratore > E-mail&quot; è che stai scegliendo di creare il collegamento per l’annullamento della sottoscrizione nei modelli e-mail stessi. La casella di testo dispone di una convalida che non consente di salvare senza contenuto. Per ovviare a questo problema, aggiungete un piccolo commento HTML. Il commento HTML non viene visualizzato nel client di posta elettronica, perché esegue il rendering dell&#39;e-mail in HTML e i commenti vengono omessi. Ecco come farlo.

1. Accedete a **Admin** e fate clic su **Email**.

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. Selezionare tutto il testo e premere il tasto **Elimina**.

   >[!CAUTION]
   >
   >Prima di procedere all’eliminazione, copiate/incollate questo elemento in un documento di testo come backup.

1. Digitare `<!--This is a comment -->`.

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. Fare clic su **Salva modifiche**.

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>Per **Annulla sottoscrizione testo** è necessario aggiungere un singolo carattere. Usate un trattino o un punto.
