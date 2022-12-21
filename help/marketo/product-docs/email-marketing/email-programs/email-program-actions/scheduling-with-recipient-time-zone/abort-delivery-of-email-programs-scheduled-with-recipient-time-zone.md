---
unique-page-id: 13795727
description: Interrompi la consegna di programmi e-mail pianificati con il fuso orario del destinatario - Marketo Docs - Documentazione del prodotto
title: Interrompi la consegna di programmi e-mail pianificati con il fuso orario del destinatario
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Interrompi la consegna di programmi e-mail pianificati con il fuso orario del destinatario {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

In casi di emergenza, puoi interrompere la consegna di un programma e-mail già in esecuzione con l’opzione Fuso orario destinatario abilitata.

Poiché i programmi e-mail pianificati con il fuso orario destinatario possono essere eseguiti per un massimo di 24 ore, l’interruzione della consegna del programma annullerà gli invii successivi dopo tale punto.

1. Selezionare il programma e-mail che si desidera annullare, quindi fare clic su **Interrompi consegna** nella sezione Approvazione del pannello di controllo.

   ![](assets/ptz-abortdelivery.png)

1. Conferma l’annullamento della consegna facendo clic su **Interrompere**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Dopo la cancellazione, il **Risultati** la griglia del tuo programma email sarà simile a quella sottostante. Eventuali invii successivi vengono annullati e verranno visualizzati come &quot;Soft rimbalzato e-mail&quot; nel **Tipo di attività** colonna.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Le e-mail annullate verranno cancellate **not** apparire come un rimbalzo morbido *fino a* l&#39;ora originariamente prevista per la consegna nei rispettivi fusi orari. Fino a quel momento, verranno comunque visualizzati come &quot;Invia e-mail&quot;.

1. Dalla griglia, puoi fare clic su qualsiasi e-mail per visualizzare i dettagli dell’attività. Per un&#39;invio annullato, il pop-up dei dettagli sarà simile al seguente:

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Informazioni sul fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Pianificare programmi e-mail con il fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)

