---
unique-page-id: 2360245
description: Rimuovi il testo dell’annullamento dell’abbonamento dalla sezione e-mail dell’amministratore - Documenti Marketo - Documentazione del prodotto
title: Rimuovi il testo dell’annullamento dell’abbonamento dalla sezione e-mail dell’amministratore
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Rimuovi il testo dell’annullamento dell’abbonamento dalla sezione e-mail dell’amministratore {#remove-unsubscribe-text-from-the-admin-email-section}

L’unico motivo per cui devi rimuovere completamente il contenuto dell’annullamento dell’abbonamento dall’area &quot;Amministratore > E-mail&quot; è la scelta di creare il collegamento per l’annullamento dell’abbonamento nei modelli e-mail stessi. La casella di testo presenta una convalida che non consente di salvare senza contenuto. È possibile aggirare questo problema aggiungendo un piccolo commento di HTML. Il commento di HTML non verrà visualizzato nel client e-mail, perché esegue il rendering dell’e-mail in HTML e i commenti vengono omessi. Ecco come farlo.

1. Vai a **Amministratore** area.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Fai clic su **E-mail**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Seleziona tutto il testo e premi il pulsante **Elimina** chiave.

   >[!CAUTION]
   >
   >Prima di eliminare, copiarlo/incollarlo in un documento di testo come backup.

1. Digitare in `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Fai clic su **Salva modifiche**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Per **Testo non registrato** è necessario aggiungere un singolo carattere. Utilizza un trattino o un punto.
