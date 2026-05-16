---
unique-page-id: 42762519
description: Scopri come configurare Marketo Sales Insight per i clienti Salesforce esistenti. Aggiorna da pacchetti precedenti o aggiungi Azioni.
title: Configurazione per clienti esistenti
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/kdiRnqpm3kJXIPz2QLQS-AF3f04UIPuOS6c836EXlxo
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 158
ht-degree: 10%

---

# Configurazione per clienti esistenti {#configuration-for-existing-customers}

Imposta la seguente configurazione per iniziare a utilizzare la nuova dashboard di Insights.

>[!PREREQUISITES]
>
>Assicurarsi di aver aggiornato il pacchetto [!DNL Salesforce] alla versione più recente

## Configura [!DNL Sales Insight] in Marketo {#configure-sales-insight-in-marketo}

1. Apri una nuova scheda nel browser per ottenere le credenziali di [!DNL Marketo Sales Insights] dal tuo account Marketo.

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/configuration-for-existing-customers-1.png)

1. Fai clic su **[!UICONTROL Sales Insight]**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Fare clic su **[!UICONTROL View]** per popolare le credenziali API REST.

   ![](assets/configuration-for-existing-customers-3.png)

1. Viene visualizzata una finestra a comparsa di conferma. Fai clic su **[!UICONTROL OK]**.

## Configura [!DNL Sales Insight] in [!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. In Salesforce, fare clic su **[!UICONTROL Setup]**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Cercare e selezionare **[!UICONTROL Remote Site Settings]**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Fai clic su **[!UICONTROL New Remote Site]**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Immetti [!UICONTROL Remote Site Name] (può essere ad esempio &quot;MarketoRestAPI&quot;) e [!UICONTROL Remote Site URL] (l&#39;URL API dal pannello Configurazione API REST in Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/configuration-for-existing-customers-8.png)

   Ora hai creato l’impostazione per il sito remoto per l’API Rest.

## Accedi a Marketo Sales Insight {#access-marketo-sales-insight}

1. Copiare le credenziali dal pannello API REST nella pagina di amministrazione di [!DNL Marketo’s Sales Insight]. Incollali nella sezione API REST della pagina di configurazione [!DNL Sales Insight] di Salesforce.

1. Immettere [!UICONTROL API Secret Key].

   ![](assets/configuration-for-existing-customers-9.png)
