---
unique-page-id: 2360217
description: Modificare le impostazioni di attribuzione per Analytics - Documenti Marketo - Documentazione del prodotto
title: Modificare le impostazioni di attribuzione per Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Modificare le impostazioni di attribuzione per Analytics {#change-attribution-settings-for-analytics}

Puoi modificare il modo in cui Marketo collega i contatti alle opportunità per l’attribuzione primo e multi-touch, le metriche di conversione lead e il flag di opportunità influenzato dal marketing.

Queste impostazioni avranno un impatto sui rapporti di Revenue Explorer nelle aree [Program Opportunity Analysis](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Opportunity Analysis](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) e Lead Analysis. Questo influisce anche sul rapporto di Program Analyzer (Analisi programmi).

1. Nella sezione **Amministratore**, fai clic su **Analisi del ciclo dei ricavi**.

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. Fai clic sul collegamento **Modifica** in **Attribuzione**.

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >La modifica di questa impostazione non modifica alcun dato di Marketo; cambia semplicemente il modo in cui vengono eseguiti i rapporti. Questo può essere ripristinato in qualsiasi momento.

1. Seleziona un&#39;opzione e fai clic su **Salva**.

   ![](assets/image2014-9-24-11-3a57-3a39.png)

   >[!NOTE]
   >
   >**Definizione**
   >
   >**Esplicito**: Solo i contatti con i ruoli (impostazione predefinita).
   >
   >**Ibrido**: Contatti con ruoli, se disponibili. Se non sono disponibili, vengono utilizzati tutti i contatti presenti negli account.
   >
   >**Implicito**: Tutti i contatti indipendentemente dal ruolo.

>[!CAUTION]
>
>Quando utilizzi **Implicit**, Marketo esaminerà sempre tutti i contatti associati all&#39;account, indipendentemente dal ruolo. **Marketo consiglia vivamente di utilizzare la modalità** Esplicita. L&#39;utilizzo di Implicit può creare falsi positivi; persone che hanno il merito di avere un&#39;opportunità nonostante non abbiano una reale influenza nell&#39;opportunità. Usa Implicit con cautela.
