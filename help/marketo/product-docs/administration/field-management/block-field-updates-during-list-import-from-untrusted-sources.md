---
unique-page-id: 2360335
description: Blocca aggiornamenti dei campi durante l’importazione dell’elenco da origini non attendibili - Documentazione di Marketo - Documentazione del prodotto
title: Bloccare aggiornamenti dei campi durante l’importazione degli elenchi da origini non attendibili
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 13%

---

# Bloccare aggiornamenti dei campi durante l’importazione degli elenchi da origini non attendibili {#block-field-updates-during-list-import-from-untrusted-sources}

In alcuni elenchi è possibile considerare attendibili i dati più di altri. A volte si hanno dati discutibili e si desidera accettarli se il campo è vuoto, ma non se è presente un valore esistente. Per farlo, blocca gli aggiornamenti dei campi nei campi chiave.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Blocco Degli Aggiornamenti Dei Campi Da Origini Non Attendibili {#blocking-field-updates-from-untrusted-sources}

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Fai clic su **[!UICONTROL Field Management]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Individuare il campo desiderato, selezionarlo, quindi in **[!UICONTROL Field Actions]** fare clic su **[!UICONTROL Block Field Updates]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Selezionare **[!UICONTROL List Import untrusted source]** e fare clic su **[!UICONTROL Apply]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>È possibile proteggere i campi da tutti gli elenchi, attendibili e non attendibili, selezionando anche **[!UICONTROL List Import trusted source]**.

Ripetere i passaggi precedenti per tutti gli altri campi che si desidera proteggere dagli elenchi non attendibili.

## Esecuzione di un&#39;importazione di elenchi non attendibili {#running-an-untrusted-list-import}

1. Quando esegui l&#39;importazione dell&#39;elenco, assicurati di selezionare **[!UICONTROL Untrusted]** se desideri che tutti i campi configurati nel passaggio precedente siano sicuri.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Per istruzioni dettagliate sull&#39;importazione degli elenchi, vedere [Importare un elenco di persone](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Ottimo lavoro. Ora sai come proteggere i campi chiave dagli elenchi non attendibili.
