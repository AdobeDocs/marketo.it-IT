---
description: Errori di sincronizzazione Salesforce - Documentazione Marketo - Documentazione del prodotto
title: Errori di sincronizzazione Salesforce
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 1%

---

# [!DNL Salesforce] errori di sincronizzazione {#salesforce-sync-errors}

Visualizza un riepilogo degli errori riscontrati durante il processo di sincronizzazione. Sono inclusi gli errori causati da errori di sincronizzazione dei dati non compatibili.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Visualizza errori di sincronizzazione {#view-sync-errors}

1. Fai clic su **[!UICONTROL Admin]**.

   ![](assets/salesforce-sync-errors-1.png)

1. In Integrazione, fare clic su **Salesforce**, quindi sulla scheda **[!UICONTROL Sync Errors]**.

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>Gli errori elencati vanno dall&#39;ora corrente ai cinque giorni precedenti la sincronizzazione corrente.

| Campo | Descrizione |
|---|---|
| Non riuscito il | Livello record _o_ livello processo |
| Data/ora dell’errore | Dettagli errore |
| Tipo di errore | Messaggio di ritorno SFDC |

>[!TIP]
>
>Facendo clic sul record a livello di record vengono visualizzati gli ID Marketo e [!DNL Salesforce] dell&#39;oggetto correlato. In alcuni casi, il messaggio sugli errori a livello di record e di processo proviene direttamente da [!DNL Salesforce]. Per ulteriori informazioni, vedere Ricerca in linea.

## Errori di sincronizzazione filtri {#filter-sync-errors}

1. Per filtrare i dati, fai clic sull’icona del filtro posta all’estrema destra della pagina.

   ![](assets/salesforce-sync-errors-3.png)

1. Seleziona l’intervallo di date e ore, quindi filtra per tipo di errore (livello processo o livello record). Al termine, fai clic su **[!UICONTROL Apply]**.

   ![](assets/salesforce-sync-errors-4.png)

**PASSAGGIO FACOLTATIVO**: per esportare gli errori di sincronizzazione, fare clic su **[!UICONTROL Export]**. I dati verranno esportati come file CSV.

![](assets/salesforce-sync-errors-5.png)
