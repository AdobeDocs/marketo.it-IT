---
unique-page-id: 2953373
description: Configurare i piè di pagina per l'annullamento della sottoscrizione a Marketo Sales Insight - Marketo Docs - Documentazione prodotto
title: Configurare i piè di pagina per l’annullamento della sottoscrizione in Marketing Cloud
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# Configurare i piè di pagina per l&#39;annullamento della sottoscrizione in Marketing Sales Insight {#configure-unsubscribe-footers-in-marketo-sales-insight}

Le e-mail di vendita inseriscono automaticamente il piè di pagina di annullamento sottoscrizione nella parte inferiore. Tuttavia, potete regolare le impostazioni in base alle vostre esigenze.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>**Definizione**
>
>**Le** e-mail di vendita sono quelle inviate da Sales Insight (non includono quelle inviate dal plug-in di Outlook di Marketo).

1. Andate all&#39;area **Admin**.

   ![](assets/one-1.png)

1. Fare clic su **Sales Insight**, quindi su **Edit Settings**.

   ![](assets/two-1.png)

   Ci sono diverse opzioni. Analizziamo innanzitutto i tipi di e-mail per cui potete modificare le impostazioni.

   ![](assets/three-1.png)

   * **Nessun modello** : composto manualmente dall&#39;utente di vendita.
   * **E-mail**  standard - E-mail basate su un modello.
   * **E-mail**  operativa: e-mail che ignorano i limiti di sottoscrizione non sottoscritti, sospensione del marketing e comunicazione (inviano indipendentemente da quale elemento).

   Potete impostare un comportamento diverso per ciascun tipo.

   >[!CAUTION]
   >
   >**Rispetta le impostazioni** di annullamento sottoscrizione: i lead non sottoscritti NON riceveranno l&#39;e-mail persino se l&#39;e-mail pubblicata è &quot;operativa&quot;
   >
   >**Ignora impostazioni** annullamento sottoscrizione: i lead non sottoscritti riceveranno l&#39;e-mail

1. Apportate le modifiche desiderate, quindi fate clic su **Salva**.

   >[!TIP]
   >
   >Le ultime due opzioni consentono di includere/escludere dinamicamente il piè di pagina per l’annullamento della sottoscrizione in base al numero di destinatari (maggiore di 1 o maggiore di 5).

   ![](assets/four-1.png)

Wow! Un po&#39; complicato, ma abbastanza flessibile, giusto?
