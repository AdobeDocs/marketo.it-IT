---
unique-page-id: 12981050
description: Blocca modello di vendita - Documenti Marketo - Documentazione del prodotto
title: Blocca modello di vendita
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Blocca modello di vendita {#lock-sales-template}

Per impedire agli utenti CRM di modificare i modelli di vendita, gli amministratori possono abilitare la possibilità di bloccare i modelli, che quindi consente agli utenti di bloccare i modelli singolarmente dall&#39;editor e-mail.

>[!CAUTION]
>
>Questa funzione funziona solo per Salesforce e non è compatibile con Microsoft Dynamics o altri CRM. I modelli a cui si accede dai plug-in di Outlook o Gmail non verranno bloccati, in quanto l&#39;editor non è controllato da Marketo.

## Abilita modello di blocco {#enable-lock-template}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai a **Amministratore**, quindi fai clic su **Approfondimenti vendite**.

   ![](assets/1.png)

1. Sotto **Impostazioni**, fai clic su **Modifica**.

   ![](assets/2.png)

1. Controlla **Abilitare il blocco dei modelli**. Fai clic su **Salva**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Per impostazione predefinita, questa casella è selezionata e la possibilità di bloccare i modelli è abilitata. Deselezionando questa opzione, la funzione Blocca modello verrà disabilitata nell’editor e-mail.

>[!NOTE]
>
>La modifica di questa impostazione come amministratore **not** incidere retroattivamente sui modelli esistenti; Ad esempio, non li blocca automaticamente.

## Blocca modello nell’editor e-mail {#lock-template-in-the-email-editor}

1. Seleziona l&#39;e-mail che desideri bloccare, quindi fai clic su **Modifica bozza**.

   ![](assets/5.png)

1. Nell’editor e-mail, fai clic su **Impostazioni e-mail**.

   ![](assets/6.png)

1. Controlla **Pubblicare su Marketo Sales Insight** se non è già controllato. Ora puoi deselezionare **Consenti all&#39;utente CRM di modificare l&#39;e-mail** per bloccare il modello. Fai clic su **Salva**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, questa casella è selezionata e gli utenti CRM sono autorizzati a modificare le e-mail.
