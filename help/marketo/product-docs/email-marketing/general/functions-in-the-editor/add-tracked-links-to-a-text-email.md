---
unique-page-id: 1900589
description: Scopri come aggiungere collegamenti tracciati alle e-mail di solo testo. Abilita il tracciamento dei collegamenti in modo da poter misurare i clic nei rapporti e-mail.
title: Aggiungere collegamenti tracciati a un messaggio e-mail di testo
exl-id: 10b4e029-de23-4054-83f7-b68fea68c838
feature: Email Editor
TQID: https://experienceleague.adobe.com/zz5DkOWG-x3y-oq-E77xRAZtcNdmimbwKsctKSChnXM
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 174
ht-degree: 8%

---

# Aggiungere collegamenti tracciati a un messaggio e-mail di testo {#add-tracked-links-to-a-text-email}

>[!PREREQUISITES]
>
>* [Crea un&#39;e-mail di solo testo](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-a-text-only-email.md)
>* [Modifica elementi in un messaggio e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/edit-elements-in-an-email.md)

I collegamenti e-mail di testo possono essere tracciati in Marketo. Vediamo come funziona.

1. Seleziona l&#39;e-mail e fai clic su **Modifica bozza**.

1. Selezionare l&#39;indirizzo di posta elettronica e fare clic su **[!UICONTROL Edit Draft]**.

   ![](assets/one-9.png)

1. Fare doppio clic sull&#39;area modificabile a cui si desidera aggiungere il collegamento.

   ![](assets/two-8.png)

1. Immettere l&#39;URL tra parentesi quadre, come segue: `[[www.domain.com/path/page.html]]`.

   ![](assets/three-8.png)

   >[!CAUTION]
   >
   >Se un&#39;e-mail è stata inviata più di 365 giorni fa **e** nessuno ha fatto clic su uno dei collegamenti negli ultimi 180 giorni, Marketo Engage elimina la route all&#39;URL dal nostro database, causando l&#39;interruzione del collegamento. Se il collegamento deve essere permanente, non utilizzare il tracciamento.

1. Chiudi l’editor e non dimenticare di approvare la bozza.

   ![](assets/four-6.png)

>[!NOTE]
>
>La funzionalità di classe mktNoTok non funziona con collegamenti tracciabili nelle e-mail di testo. Solo per e-mail HTML.
