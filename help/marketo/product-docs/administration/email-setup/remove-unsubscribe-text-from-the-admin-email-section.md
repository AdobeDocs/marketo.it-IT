---
unique-page-id: 2360245
description: Rimuovi il testo per l’annullamento dell’iscrizione dalla sezione E-mail per amministratori - Documentazione di Marketo - Documentazione del prodotto
title: Rimuovi il testo per l’annullamento dell’iscrizione dalla sezione E-mail amministratore
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
source-git-commit: 81ee349dbbe48c70b040751cae750c3684b71c78
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Rimuovi il testo per l’annullamento dell’iscrizione dalla sezione E-mail amministratore {#remove-unsubscribe-text-from-the-admin-email-section}

L’unico motivo per cui dovresti mai rimuovere completamente il contenuto per cui hai annullato l’abbonamento dal **[!UICONTROL Amministratore]** > **[!UICONTROL E-mail]** L’area è utile per creare il collegamento di annullamento all’abbonamento nei modelli e-mail stessi. La convalida della casella di testo non consente il salvataggio senza contenuto. Per ovviare a questo problema, aggiungi un piccolo commento HTML. Il commento di HTML non verrà visualizzato nel client e-mail, perché esegue il rendering dell’e-mail in HTML e i commenti vengono omessi. Ecco come farlo.

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Clic **[!UICONTROL E-mail]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Selezionare tutto il testo e premere il tasto **[!UICONTROL Elimina]** chiave.

   >[!CAUTION]
   >
   >Prima di eliminarlo, copiatelo/incollatelo in un documento di testo come backup.

1. Digitare in `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Clic **[!UICONTROL Salva modifiche]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Per **Testo per annullamento iscrizione** devi aggiungere un singolo carattere. Utilizza un trattino o un punto.
