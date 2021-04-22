---
description: Errori di sincronizzazione Salesforce - Documenti Marketo - Documentazione del prodotto
title: Errori di sincronizzazione Salesforce
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Errori di sincronizzazione Salesforce {#salesforce-sync-errors}

Visualizza un riepilogo degli errori riscontrati durante il processo di sincronizzazione. Sono inclusi gli errori causati da errori di sincronizzazione dei dati non compatibili.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Visualizza errori di sincronizzazione {#view-sync-errors}

1. Fai clic su **Amministratore**.

   ![](assets/salesforce-sync-errors-1.png)

1. In Integrazione, fai clic su **Salesforce**, quindi sulla scheda **Errori di sincronizzazione**.

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>Gli errori elencati vanno dall’ora corrente ai cinque giorni precedenti la sincronizzazione corrente.

| Campo | Descrizione |
|---|---|
| Non riuscito | Livello record _o_ Livello processo |
| Data/ora dell’errore | Dettagli errore |
| Tipo di errore | Messaggio di ritorno SFDC |

>[!TIP]
>
>Facendo clic sul record a livello di record vengono visualizzati gli ID Marketo e Salesforce dell’oggetto correlato. In alcuni casi, il messaggio sugli errori a livello di record e di processo proviene direttamente da Salesforce. La ricerca online può fornire ulteriori dettagli.

## Errori di sincronizzazione del filtro {#filter-sync-errors}

1. Per filtrare i dati, fai clic sull’icona del filtro posta all’estrema destra della pagina.

   ![](assets/salesforce-sync-errors-3.png)

1. Seleziona il tuo intervallo di date e ore, quindi filtra per Tipo di errore (Livello di lavoro o Livello di record). Al termine, fai clic su **Applica**.

   ![](assets/salesforce-sync-errors-4.png)

**Passaggio** facoltativo: Per esportare gli errori di sincronizzazione, fai clic su  **Esporta**. I dati verranno esportati come CSV.

![](assets/salesforce-sync-errors-5.png)
