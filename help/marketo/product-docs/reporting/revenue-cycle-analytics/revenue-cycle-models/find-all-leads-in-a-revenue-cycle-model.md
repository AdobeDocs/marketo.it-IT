---
unique-page-id: 2360423
description: Trovare tutti i lead in un modello di ciclo dei ricavi - Documenti Marketo - Documentazione del prodotto
title: Trovare tutti i lead in un modello del ciclo dei ricavi
exl-id: 428dbfa1-2f19-41ce-bfc6-e63edfdaba17
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 9%

---

# Trovare tutti i lead in un modello del ciclo dei ricavi {#find-all-leads-in-a-revenue-cycle-model}

Utilizzando gli elenchi avanzati, puoi trovare facilmente tutti i membri del modello del ciclo dei ricavi.

>[!PREREQUISITES]
>
>[Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Dopo aver selezionato la smart list, fare clic sulla scheda **[!UICONTROL Smart List]**.

   ![](assets/image2015-4-29-14-3a6-3a36.png)

1. Trovare il filtro **[!UICONTROL Member of Revenue Model]** e trascinarlo nell&#39;area di lavoro.

   ![](assets/image2015-4-29-14-3a12-3a33.png)

1. Seleziona **[!UICONTROL Model]**.

   ![](assets/image2015-5-13-18-3a2-3a23.png)

   Questo ti darebbe tutti i contatti in quel modello, indipendentemente dallo stadio. In genere è necessario un passaggio specifico. Utilizza invece il seguente filtro.

1. Trovare il filtro **[!UICONTROL Revenue Stage]** e trascinarlo nell&#39;area di lavoro.

   ![](assets/image2015-5-13-17-3a27-3a0.png)

1. Seleziona **[!UICONTROL Stage]**.

   ![](assets/image2015-5-13-17-3a31-3a9.png)

1. Passa alla scheda **[!UICONTROL Leads]** per visualizzare i risultati.

   ![](assets/2.png)

   >[!TIP]
   >
   >Non sono necessari entrambi i filtri, è sufficiente scegliere quello desiderato. Vi stiamo solo mostrando entrambi di essere scrupolosi.

   >[!CAUTION]
   >
   >Se la fase di un lead viene modificata da una campagna esterna durante la creazione iniziale del lead, un’attività non viene registrata nel database. Questo significa che il lead non verrà incluso dal filtro elenco avanzato.
