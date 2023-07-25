---
unique-page-id: 13795727
description: Interrompere la consegna dei programmi e-mail pianificati con il fuso orario del destinatario - Documentazione di Marketo - Documentazione del prodotto
title: Interrompi la consegna dei programmi e-mail pianificati con il fuso orario del destinatario
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Interrompi la consegna dei programmi e-mail pianificati con il fuso orario del destinatario {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

In casi di emergenza, puoi interrompere la consegna di un programma e-mail già avviato con il Fuso orario del destinatario abilitato.

Poiché i programmi e-mail pianificati con il fuso orario del destinatario possono essere eseguiti per un massimo di 24 ore, l’interruzione della consegna del programma annullerà tutti gli invii successivi dopo tale momento.

1. Seleziona il programma e-mail da annullare, quindi fai clic su **Interrompi consegna** nel riquadro Approvazione del Pannello di controllo Campaign.

   ![](assets/ptz-abortdelivery.png)

1. Conferma di voler annullare la consegna facendo clic su **Interrompi**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Dopo la cancellazione, il **Risultati** griglia del programma e-mail avrà un aspetto simile a quello riportato di seguito. Eventuali invii successivi vengono annullati e visualizzati come &quot;E-mail non recapitate&quot; nel **Tipo di attività** colonna.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Le e-mail annullate **non** viene visualizzato come messaggio non recapitato *fino a* l’ora prevista per la consegna nel rispettivo fuso orario. Fino a quel momento, visualizzeranno comunque il messaggio &quot;Send Email&quot; (Invia e-mail).

1. Dalla griglia, puoi fare clic su qualsiasi e-mail per visualizzare i dettagli dell’attività. Per un invio annullato, la finestra a comparsa dei dettagli sarà simile alla seguente:

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Informazioni sul fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Pianificazione dei programmi e-mail con fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
