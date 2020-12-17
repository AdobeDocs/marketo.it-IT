---
unique-page-id: 2360335
description: Blocca aggiornamenti dei campi durante l'importazione di elenchi da origini non attendibili - Documenti Marketo - Documentazione prodotto
title: Blocca aggiornamenti dei campi durante l'importazione dell'elenco da origini non attendibili
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# Blocca aggiornamenti dei campi durante l&#39;importazione degli elenchi da origini non affidabili {#block-field-updates-during-list-import-from-untrusted-sources}

È possibile considerare affidabili i dati in alcuni elenchi più di altri. A volte si dispone di dati discutibili e si desidera utilizzarli se il campo è vuoto, ma non se esiste un valore esistente. È possibile eseguire questa operazione bloccando gli aggiornamenti dei campi sui campi chiave.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Blocco degli aggiornamenti dei campi da origini non attendibili {#blocking-field-updates-from-untrusted-sources}

1. Accedete a **Admin** e fate clic su **Field Management**.

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. Trovare il campo desiderato, selezionarlo, quindi in **Azioni campo** fare clic su **Blocca aggiornamenti campo**.

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. Selezionare **List Import untrusted source** e fare clic su **Apply**.

   ![](assets/blockupdates.png)

>[!TIP]
>
>È possibile mantenere i campi al sicuro da tutti gli elenchi, attendibili e non attendibili, anche selezionando **Origine attendibile importazione elenco**.

Ripetere i passaggi indicati sopra per tutti gli altri campi che si desidera mantenere al sicuro dagli elenchi non attendibili.

## Esecuzione di un&#39;importazione elenco non attendibile {#running-an-untrusted-list-import}

1. Durante l&#39;importazione dell&#39;elenco, assicurarsi di selezionare **Non attendibile **se si desidera che tutti i campi impostati nel passaggio precedente siano sicuri.

   ![](assets/importpersondetails.jpg)

Per istruzioni dettagliate sull&#39;importazione di elenchi, vedere [Importare un elenco di persone](../../../getting-started/quick-wins/import-a-list-of-people.md).

Bel lavoro! Ora sai come proteggere i campi chiave da elenchi non attendibili.
