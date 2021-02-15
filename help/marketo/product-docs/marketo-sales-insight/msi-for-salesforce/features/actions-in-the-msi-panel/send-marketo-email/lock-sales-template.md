---
unique-page-id: 12981050
description: Blocca modello di vendita - Documenti Marketo - Documentazione prodotto
title: Blocca modello di vendita
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Blocca modello di vendita {#lock-sales-template}

Per impedire agli utenti CRM di modificare i modelli di vendita, gli amministratori possono abilitare la possibilità di bloccare i modelli, che quindi consente agli utenti di bloccare i modelli singolarmente dall&#39;editor e-mail.

>[!CAUTION]
>
>Questa funzione funziona solo per Salesforce e non è compatibile con Microsoft Dynamics o altri CRM. I modelli a cui si accede dai plug-in di Outlook o Gmail non verranno bloccati, in quanto l&#39;editor non è controllato da Marketo.

## Abilita Blocca modello {#enable-lock-template}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai a **Admin**, quindi fai clic su **Sales Insight**.

   ![](assets/1.png)

1. In **Impostazioni**, fare clic su **Modifica**.

   ![](assets/2.png)

1. Selezionare **Abilita la possibilità di bloccare i modelli**. Fare clic su **Salva**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Per impostazione predefinita, questa casella è selezionata e la possibilità di bloccare i modelli è abilitata. Deselezionando questa opzione, nell’editor e-mail verrà disattivata la funzione Blocca modello.

>[!NOTE]
>
>La modifica di questa impostazione come amministratore non avrà effetti retroattivi sui modelli esistenti; ad esempio, non li bloccherà automaticamente.****

## Blocca modello nell&#39;Editor e-mail {#lock-template-in-the-email-editor}

1. Selezionare l&#39;e-mail che si desidera bloccare, quindi fare clic su **Modifica bozza**.

   ![](assets/5.png)

1. Nell&#39;editor e-mail, fare clic su **Impostazioni e-mail**.

   ![](assets/6.png)

1. Selezionare **Pubblica in Marketing Sales Insight** se non è già selezionato. Ora puoi deselezionare **Consenti all&#39;utente CRM di modificare l&#39;e-mail** per bloccare il modello. Fare clic su **Salva**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, questa casella è selezionata e agli utenti CRM è consentito modificare le e-mail.
