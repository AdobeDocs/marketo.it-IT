---
unique-page-id: 12981050
description: Blocca modello di vendita - Documentazione Marketo - Documentazione del prodotto
title: Blocca modello vendite
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 1%

---

# Blocca modello vendite {#lock-sales-template}

Per impedire agli utenti di CRM di modificare i modelli di vendita, gli amministratori possono abilitare la possibilità di bloccare i modelli, che quindi consente agli utenti di bloccare i modelli singolarmente dall’editor e-mail.

>[!CAUTION]
>
>Questa funzionalità funziona solo per [!DNL Salesforce] e non è compatibile con [!DNL Microsoft Dynamics] o altri CRM. I modelli a cui si accede dai plug-in [!DNL Outlook] o Gmail non verranno bloccati, in quanto l&#39;editor non è controllato da Marketo.

## Abilita modello di blocco {#enable-lock-template}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai a **[!UICONTROL Admin]**, quindi fai clic su **[!UICONTROL Sales Insight]**.

   ![](assets/1.png)

1. In **[!UICONTROL Settings]**, fare clic su **[!UICONTROL Edit]**.

   ![](assets/2.png)

1. Seleziona **[!UICONTROL Enable ability to lock templates]**. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Per impostazione predefinita, questa casella è selezionata e la possibilità di bloccare i modelli è abilitata. Deselezionandola, verrà disabilitata la funzione di blocco del modello nell’editor e-mail.

>[!NOTE]
>
>La modifica di questa impostazione come amministratore **non** influirà retroattivamente sui modelli esistenti, ovvero non li bloccherà automaticamente.

## Blocca modello nell’editor e-mail {#lock-template-in-the-email-editor}

1. Selezionare l&#39;e-mail che si desidera bloccare, quindi fare clic su **[!UICONTROL Edit Draft]**.

   ![](assets/5.png)

1. Nell&#39;editor di posta elettronica fare clic su **[!UICONTROL Email Settings]**.

   ![](assets/6.png)

1. Selezionare **[!UICONTROL Publish to Marketo Sales Insight]** se non è già selezionato. È ora possibile deselezionare **[!UICONTROL Allow CRM user to edit email]** per bloccare il modello. Fai clic su **[!UICONTROL Save]**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, questa casella è selezionata e gli utenti CRM possono modificare le e-mail.
