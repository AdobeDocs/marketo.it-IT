---
unique-page-id: 2360335
description: Blocca aggiornamenti dei campi durante l’importazione dell’elenco da origini non attendibili - Documentazione di Marketo - Documentazione del prodotto
title: Blocca aggiornamenti dei campi durante l'importazione degli elenchi da origini non attendibili
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Blocca aggiornamenti dei campi durante l&#39;importazione degli elenchi da origini non attendibili {#block-field-updates-during-list-import-from-untrusted-sources}

In alcuni elenchi è possibile considerare attendibili i dati più di altri. A volte si hanno dati discutibili e si desidera accettarli se il campo è vuoto, ma non se è presente un valore esistente. Per farlo, blocca gli aggiornamenti dei campi nei campi chiave.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Blocco Degli Aggiornamenti Dei Campi Da Origini Non Attendibili {#blocking-field-updates-from-untrusted-sources}

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Fare clic su **[!UICONTROL Gestione campi]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Trova il campo desiderato, selezionalo, quindi in **[!UICONTROL Azioni campo]** fai clic su **[!UICONTROL Blocca aggiornamenti campo]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Controlla **[!UICONTROL Origine non attendibile importazione elenchi]** e fai clic su **[!UICONTROL Applica]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>È possibile proteggere i campi da tutti gli elenchi, attendibili e non attendibili, selezionando anche **[!UICONTROL Origine attendibile importazione elenchi]**.

Ripetere i passaggi precedenti per tutti gli altri campi che si desidera proteggere dagli elenchi non attendibili.

## Esecuzione di un&#39;importazione di elenchi non attendibili {#running-an-untrusted-list-import}

1. Quando esegui l&#39;importazione dell&#39;elenco, assicurati di selezionare **[!UICONTROL Non attendibile]** se desideri che tutti i campi configurati nel passaggio precedente siano sicuri.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Per istruzioni dettagliate sull&#39;importazione degli elenchi, vedere [Importare un elenco di persone](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Ottimo lavoro. Ora sai come proteggere i campi chiave dagli elenchi non attendibili.
