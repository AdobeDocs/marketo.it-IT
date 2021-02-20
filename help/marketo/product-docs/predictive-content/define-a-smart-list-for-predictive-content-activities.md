---
unique-page-id: 10097873
description: Definire un elenco avanzato per le attività di Predictive Content - Marketo Docs - Documentazione prodotto
title: Definire un elenco avanzato per le attività relative ai contenuti predittivi
translation-type: tm+mt
source-git-commit: f1d7b270454ba41db5197a069e0dcc2caebdec63
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# Definire un elenco avanzato per le attività relative ai contenuti predittivi {#define-a-smart-list-for-predictive-content-activities}

Potete utilizzare le attività di contenuto predittivo in attivatori e filtri quando definite un elenco smart in una campagna intelligente. È possibile attivare un&#39;azione per chiunque faccia clic sul contenuto predittivo tramite il [modello di contenuti multimediali avanzati](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), la [barra delle raccomandazioni sui contenuti](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md) o in un [messaggio e-mail](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md).

1. Nella campagna intelligente, andate alla scheda **Smart List**.

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >Gli elenchi intelligenti possono fare cose straordinarie. Per saperne di più, consulta la sezione [smart list deep dive](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Cercare l&#39;attivatore, quindi trascinarlo e rilasciarlo sul quadro.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Una campagna intelligente con trigger viene eseguita in modalità Trigger. Viene eseguito su una persona alla volta in base agli eventi attivati e ai filtri aggiunti.

1. Fare clic sul menu a discesa **Nome** e selezionare un operatore.

   ![](assets/smart-list-dropdown-hands.png)

1. Definire il trigger.

   ![](assets/smart-lislt-select-content-hands.png)

1. Aggiungete il vincolo **Type**.

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Selezionare l&#39;origine desiderata per l&#39;elenco avanzato.

   ![](assets/pc-add-constraint.png)

1. Se utilizzate l&#39;origine e-mail per il contenuto predittivo, aggiungete il trigger **Clic su Collega in E-mail**. Selezionate l&#39;e-mail e aggiungete il vincolo **Predictive**, definito come **true**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Aggiungete eventuali altri filtri in base alle esigenze.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >In una campagna intelligente con attivatori e filtri, i trigger si trovano nella parte superiore. Quando viene attivato, solo gli utenti che soddisfano i criteri del filtro passano attraverso il flusso.

   >[!NOTE]
   >
   >Con più attivatori, una persona passa al flusso se QUALSIASI attivatore viene attivato.

   Per eseguire la campagna su un insieme di persone allo stesso tempo, imparare a [definire un elenco smart per una campagna batch intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [Definisci elenco avanzato per Smart Campaign | Batch](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [Aggiunta di un passaggio di flusso a una campagna intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Definire un elenco avanzato per le attività di personalizzazione Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Abilita contenuto predittivo per contenuti multimediali Web](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [Abilita la barra delle raccomandazioni del contenuto](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)

