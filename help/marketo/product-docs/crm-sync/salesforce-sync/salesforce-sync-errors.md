---
description: Errori di sincronizzazione Salesforce - Documentazione Marketo - Documentazione del prodotto
title: Errori di sincronizzazione Salesforce
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
feature: Salesforce Integration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 1%

---

# Errori di sincronizzazione Salesforce {#salesforce-sync-errors}

Visualizza un riepilogo degli errori riscontrati durante il processo di sincronizzazione. Sono inclusi gli errori causati da errori di sincronizzazione dei dati non compatibili.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Visualizza errori di sincronizzazione {#view-sync-errors}

1. Clic **Amministratore**.

   ![](assets/salesforce-sync-errors-1.png)

1. In Integrazione, fai clic su **Salesforce**, quindi **Errori di sincronizzazione** scheda.

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>Gli errori elencati vanno dall&#39;ora corrente ai cinque giorni precedenti la sincronizzazione corrente.

| Campo | Descrizione |
|---|---|
| Non riuscito il | Livello record _o_ Livello di lavoro |
| Data/ora dell’errore | Dettagli errore |
| Tipo di errore | Messaggio restituito SFDC |

>[!TIP]
>
>Facendo clic sul record a livello di record vengono visualizzati gli ID Marketo e Salesforce dell&#39;oggetto correlato. In alcuni casi, il messaggio sul record e gli errori a livello di processo provengono direttamente da Salesforce. Per ulteriori informazioni, vedere Ricerca in linea.

## Errori di sincronizzazione filtri {#filter-sync-errors}

1. Per filtrare i dati, fai clic sull’icona del filtro posta all’estrema destra della pagina.

   ![](assets/salesforce-sync-errors-3.png)

1. Seleziona l’intervallo di date e ore, quindi filtra per tipo di errore (livello processo o livello record). Clic **Applica** al termine.

   ![](assets/salesforce-sync-errors-4.png)

**PASSAGGIO FACOLTATIVO**: per esportare gli errori di sincronizzazione, fai clic su **Esporta**. I dati verranno esportati come file CSV.

![](assets/salesforce-sync-errors-5.png)
