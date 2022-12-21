---
unique-page-id: 2360335
description: Aggiornamenti dei campi di blocco durante l’importazione dell’elenco da origini non attendibili - Documenti Marketo - Documentazione del prodotto
title: Aggiornamenti dei campi di blocco durante l'importazione dell'elenco da origini non attendibili
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Aggiornamenti dei campi di blocco durante l&#39;importazione dell&#39;elenco da origini non attendibili {#block-field-updates-during-list-import-from-untrusted-sources}

È possibile considerare attendibili i dati in alcuni elenchi più di altri. A volte si dispone di dati discutibili e si desidera accettarli se il campo è vuoto, ma non se esiste un valore esistente. Per eseguire questa operazione, blocca gli aggiornamenti dei campi sui campi chiave.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Blocco Degli Aggiornamenti Dei Campi Da Origini Non Attendibili {#blocking-field-updates-from-untrusted-sources}

1. Vai a **Amministratore** area.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Fai clic su **Gestione dei campi**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Trovare il campo desiderato, selezionarlo, quindi sotto **Azioni campo**, fai clic su **Aggiornamenti dei campi di blocco**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Controlla **Importa elenco sorgente non attendibile** e fai clic su **Applica**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>È possibile proteggere i campi da tutti gli elenchi, affidabili e non attendibili, anche selezionando **Importa elenco fonti attendibili**.

Ripetere i passaggi precedenti per tutti gli altri campi che si desidera proteggere dagli elenchi non attendibili.

## Esecuzione di un&#39;importazione di elenchi non attendibile {#running-an-untrusted-list-import}

1. Quando esegui l’importazione dell’elenco, assicurati di selezionare **Non attendibile** se desideri che tutti i campi impostati nel passaggio precedente siano sicuri.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Per istruzioni dettagliate sull’importazione degli elenchi, consulta [Importare un elenco di persone](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Ottimo lavoro! Ora è possibile proteggere i campi chiave da elenchi non attendibili.
