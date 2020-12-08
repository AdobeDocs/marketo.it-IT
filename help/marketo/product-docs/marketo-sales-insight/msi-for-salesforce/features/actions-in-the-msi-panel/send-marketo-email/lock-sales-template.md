---
unique-page-id: 12981050
description: Blocca modello di vendita - Documenti Marketo - Documentazione prodotto
title: Blocca modello di vendita
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
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

1. Vai ad **Admin**, quindi fai clic su **Sales Insight**.

   ![](assets/1.png)

1. In **Impostazioni**, fare clic su **Modifica**.

   ![](assets/2.png)

1. Selezionate **Abilita possibilità di bloccare i modelli**. Fate clic su **Salva**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Per impostazione predefinita, questa casella è selezionata e la possibilità di bloccare i modelli è abilitata. Deselezionando questa opzione, nell’editor e-mail verrà disattivata la funzione Blocca modello.

>[!NOTE]
>
>La modifica di questa impostazione come amministratore **non** influirà retroattivamente sui modelli esistenti; ad esempio, non li bloccherà automaticamente.

## Blocca modello nell’editor e-mail {#lock-template-in-the-email-editor}

1. Selezionate il messaggio e-mail da bloccare, quindi fate clic su **Modifica bozza**.

   ![](assets/5.png)

1. Nell’editor e-mail, fate clic su Impostazioni **e-** mail.

   ![](assets/6.png)

1. Se non è già selezionato, seleziona **Pubblica in Marketing** . Ora puoi deselezionare **Consenti agli utenti CRM di modificare le e-mail** per bloccare il modello. Fate clic su **Salva**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, questa casella è selezionata e agli utenti CRM è consentito modificare le e-mail.

