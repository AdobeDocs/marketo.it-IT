---
unique-page-id: 13795727
description: Interrompere la consegna dei programmi e-mail pianificati con il fuso orario del destinatario - Documentazione di Marketo - Documentazione del prodotto
title: Interrompi la consegna dei programmi e-mail pianificati con il fuso orario del destinatario
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Interrompi la consegna dei programmi e-mail pianificati con il fuso orario del destinatario {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

In casi di emergenza, puoi interrompere la consegna di un programma e-mail già avviato con il Fuso orario del destinatario abilitato.

Poiché i programmi e-mail pianificati con il fuso orario del destinatario possono essere eseguiti per un massimo di 24 ore, l’interruzione della consegna del programma annullerà tutti gli invii successivi dopo tale momento.

1. Selezionare il programma di posta elettronica che si desidera annullare, quindi fare clic su **[!UICONTROL Abort Delivery]** nella sezione [!UICONTROL Approval] del pannello di controllo.

   ![](assets/ptz-abortdelivery.png)

1. Confermare l&#39;annullamento della consegna facendo clic su **[!UICONTROL Abort]**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Dopo l&#39;annullamento, la griglia **[!UICONTROL Results]** del programma di posta elettronica sarà simile a quella riportata di seguito. Tutti gli invii successivi vengono annullati e verranno visualizzati come &quot;E-mail non recapitate&quot; nella colonna **[!UICONTROL Activity Type]**.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Le e-mail annullate **non** verranno visualizzate come mancati recapiti non permanenti *fino a* l&#39;ora originariamente pianificata per la consegna nei rispettivi fusi orari. Fino a quel momento, visualizzeranno comunque il messaggio &quot;Send Email&quot; (Invia e-mail).

1. Dalla griglia, puoi fare clic su qualsiasi e-mail per visualizzare i dettagli dell’attività. Per un invio annullato, la finestra a comparsa dei dettagli si presenta così:

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Informazioni sul fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Programmazione di programmi e-mail con fuso orario destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
