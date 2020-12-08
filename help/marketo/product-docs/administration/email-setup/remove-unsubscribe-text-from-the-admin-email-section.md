---
unique-page-id: 2360245
description: Rimuovi il testo dell'annullamento della sottoscrizione dalla sezione "Amministratore -> E-mail" - Documenti Marketo - Documentazione del prodotto
title: Rimuovi il testo dell'annullamento della sottoscrizione dalla sezione "Amministratore -> E-mail"
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Rimuovi il testo dell&#39;annullamento della sottoscrizione dalla sezione &quot;Amministratore -> E-mail&quot; {#remove-unsubscribe-text-from-the-admin-email-section}

L’unico motivo per cui devi rimuovere completamente il contenuto dell’iscrizione dall’area &quot;Amministratore > E-mail&quot; è che stai scegliendo di creare il collegamento per l’annullamento della sottoscrizione nei modelli e-mail stessi. La casella di testo dispone di una convalida che non consente di salvare senza contenuto. Per ovviare a questo problema, aggiungete un piccolo commento HTML. Il commento HTML non viene visualizzato nel client di posta elettronica, perché esegue il rendering dell&#39;e-mail in HTML e i commenti vengono omessi. Ecco come farlo.

1. Vai ad **Admin** e fai clic su **E-mail**.

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. Selezionare tutto il testo e premere il tasto **Delete **key.

   >[!CAUTION]
   >
   >Prima di procedere all’eliminazione, copiate/incollate questo elemento in un documento di testo come backup.

1. Digitare **<!--This is a comment -->**.

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. Fate clic su **Salva modifiche**.

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>Per **Unsubscription Text **devi aggiungere un singolo carattere. Usate un trattino o un punto.

