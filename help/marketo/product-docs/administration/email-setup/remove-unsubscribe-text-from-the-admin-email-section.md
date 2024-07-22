---
unique-page-id: 2360245
description: Rimuovi il testo per l’annullamento dell’iscrizione dalla sezione E-mail per amministratori - Documentazione di Marketo - Documentazione del prodotto
title: Rimuovi il testo per l’annullamento dell’iscrizione dalla sezione E-mail amministratore
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: d635fbd4807890266429d4a257cf7d6588736bb5
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Rimuovi il testo per annullare l’iscrizione dalla sezione Amministratore > E-mail {#remove-unsubscribe-text-from-the-admin-email-section}

L&#39;unico motivo per cui dovresti rimuovere completamente il contenuto per l&#39;annullamento dell&#39;iscrizione dall&#39;area **[!UICONTROL Amministratore]** > **[!UICONTROL E-mail]** è che stai scegliendo di creare il collegamento per l&#39;annullamento dell&#39;iscrizione nei modelli e-mail stessi. La convalida della casella di testo non consente il salvataggio senza contenuto. Per ovviare a questo problema, aggiungi un piccolo commento HTML. Il commento di HTML non verrà visualizzato nel client e-mail, perché esegue il rendering dell’e-mail in HTML e i commenti vengono omessi. Ecco come farlo.

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Fai clic su **[!UICONTROL E-mail]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Selezionare tutto il testo e premere il tasto **[!UICONTROL Elimina]**.

   >[!CAUTION]
   >
   >Prima di eliminarlo, copiatelo/incollatelo in un documento di testo come backup.

1. Digitare in `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Fai clic su **[!UICONTROL Salva modifiche]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Per il **Testo per annullamento sottoscrizione** è necessario aggiungere un singolo carattere. Utilizza un trattino o un punto.
