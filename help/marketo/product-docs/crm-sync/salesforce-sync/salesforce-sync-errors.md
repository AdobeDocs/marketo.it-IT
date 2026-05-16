---
description: Scopri come visualizzare e filtrare gli errori di sincronizzazione di Salesforce in Marketo. Vedi errori a livello di record e di processo e utilizza i dettagli dell’errore per risolvere i problemi di sincronizzazione.
title: Errori della sincronizzazione Salesforce
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/vEPgjXh8QKyzC1AiAhRqf4tF-MZpu9GETxrRAJHYVIo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 192
ht-degree: 6%

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
