---
unique-page-id: 10097873
description: Definire un elenco avanzato per le attività di contenuti predittivi - Documenti Marketo - Documentazione del prodotto
title: Definire un elenco avanzato per le attività di contenuti predittivi
exl-id: 2c72b215-8c0b-48b4-8492-8e3fe832fae9
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Definire un elenco avanzato per le attività di contenuti predittivi {#define-a-smart-list-for-predictive-content-activities}

Puoi utilizzare le attività di contenuto predittivo nei trigger e nei filtri quando definisci un elenco avanzato in una campagna avanzata. Puoi attivare un&#39;azione per chiunque faccia clic su contenuti predittivi tramite il [modello Rich Media](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), la [Barra dei contenuti consigliati](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md) o un [messaggio e-mail](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md).

1. Nella tua campagna avanzata, passa alla scheda **[!UICONTROL Smart List]**.

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >Gli elenchi avanzati possono fare cose straordinarie. Ulteriori informazioni sono disponibili in [immersione approfondita elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Cerca il trigger, quindi trascinalo e rilascialo sull’area di lavoro.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Una campagna avanzata con trigger viene eseguita in modalità Trigger. Viene eseguito su una persona alla volta in base agli eventi attivati e ai filtri aggiunti.

1. Fare clic sul menu a discesa **[!UICONTROL Name]** e selezionare un operatore.

   ![](assets/smart-list-dropdown-hands.png)

1. Definisci il trigger.

   ![](assets/smart-lislt-select-content-hands.png)

1. Aggiungere il vincolo **[!UICONTROL Type]**.

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Selezionare l&#39;origine necessaria per l&#39;elenco avanzato.

   ![](assets/pc-add-constraint.png)

1. Se utilizzi l&#39;origine e-mail per il contenuto predittivo, aggiungi il trigger **[!UICONTROL Clicks Link in Email]**. Selezionare l&#39;e-mail e aggiungere il vincolo **[!UICONTROL Is Predictive]**, definito come **[!UICONTROL true]**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Aggiungi altri filtri, se necessario.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >In una campagna intelligente con trigger e filtri, i trigger si trovano in alto. Quando viene attivato, solo le persone che soddisfano i criteri di filtro passano attraverso il flusso.

   >[!NOTE]
   >
   >Con più trigger, una persona passa al flusso se viene attivato UNO QUALSIASI dei trigger.

   Per eseguire la campagna su un gruppo di persone contemporaneamente, scopri come [definire un elenco smart per una campagna smart batch](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [Definisci elenco avanzato per Smart Campaign | Batch](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Definire un elenco avanzato per le attività di Web Personalization](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Abilita contenuto predittivo per contenuti multimediali avanzati Web](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [Attiva la barra dei contenuti](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)
