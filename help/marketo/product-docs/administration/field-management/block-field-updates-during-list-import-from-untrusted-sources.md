---
unique-page-id: 2360335
description: Aggiornamenti dei campi di blocco durante l’importazione dell’elenco da origini non attendibili - Documenti Marketo - Documentazione del prodotto
title: Aggiornamenti dei campi di blocco durante l'importazione dell'elenco da origini non attendibili
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Aggiornamenti dei campi di blocco durante l&#39;importazione dell&#39;elenco da origini non attendibili {#block-field-updates-during-list-import-from-untrusted-sources}

È possibile considerare attendibili i dati in alcuni elenchi più di altri. A volte si dispone di dati discutibili e si desidera accettarli se il campo è vuoto, ma non se esiste un valore esistente. Per eseguire questa operazione, blocca gli aggiornamenti dei campi sui campi chiave.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Blocco degli aggiornamenti dei campi da origini non attendibili {#blocking-field-updates-from-untrusted-sources}

1. Vai a **Amministratore** e fai clic su **Gestione campi**.

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. Trova il campo desiderato, selezionalo, quindi in **Azioni campo**, fai clic su **Blocca aggiornamenti campo**.

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. Selezionare **Importa elenco origine non attendibile** e fare clic su **Applica**.

   ![](assets/blockupdates.png)

>[!TIP]
>
>È possibile proteggere i campi da tutti gli elenchi, attendibili e non attendibili, anche selezionando **Importa origine attendibile**.

Ripetere i passaggi precedenti per tutti gli altri campi che si desidera proteggere dagli elenchi non attendibili.

## Esecuzione di un&#39;importazione elenco non attendibile {#running-an-untrusted-list-import}

1. Quando esegui l’importazione dell’elenco, assicurati di selezionare **Non attendibile** se desideri che tutti i campi impostati nel passaggio precedente siano sicuri.

   ![](assets/importpersondetails.jpg)

Per istruzioni dettagliate sull&#39;importazione degli elenchi, vedere [Importare un elenco di persone](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Ottimo lavoro! Ora è possibile proteggere i campi chiave da elenchi non attendibili.
