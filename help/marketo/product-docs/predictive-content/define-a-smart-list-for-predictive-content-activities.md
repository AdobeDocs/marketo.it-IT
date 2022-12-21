---
unique-page-id: 10097873
description: Definire un elenco avanzato per le attività relative ai contenuti predittivi - Documenti Marketo - Documentazione del prodotto
title: Definire un elenco avanzato per le attività relative ai contenuti predittivi
exl-id: 2c72b215-8c0b-48b4-8492-8e3fe832fae9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Definire un elenco avanzato per le attività relative ai contenuti predittivi {#define-a-smart-list-for-predictive-content-activities}

Puoi utilizzare le attività di contenuto predittivo in attivatori e filtri quando definisci un elenco smart in una campagna intelligente. Puoi attivare un’azione per chiunque faccia clic su contenuto predittivo tramite la [Modello Rich Media](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), [Barra delle raccomandazioni del contenuto](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)o in un [email](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md).

1. Nella campagna intelligente, passa alla pagina **Elenco avanzato** scheda .

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >Gli elenchi intelligenti possono fare cose incredibili. Ulteriori informazioni nel [immersione profonda in elenchi smart](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Cerca il trigger, quindi trascinalo e rilascialo nell’area di lavoro.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Una campagna intelligente con trigger viene eseguita in modalità Trigger. Viene eseguito su una persona alla volta in base agli eventi attivati e ai filtri aggiunti.

1. Fai clic sul pulsante **Nome** e seleziona un operatore .

   ![](assets/smart-list-dropdown-hands.png)

1. Definisci il trigger.

   ![](assets/smart-lislt-select-content-hands.png)

1. Aggiungi il **Tipo** vincolo.

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Selezionare l&#39;origine necessaria per l&#39;elenco smart.

   ![](assets/pc-add-constraint.png)

1. Se utilizzi l’origine e-mail per il contenuto predittivo, aggiungi la **Clic su Collega in e-mail** attivatore. Seleziona l’e-mail e aggiungi il **Predictive** vincolo, definito come **true**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Aggiungi altri filtri in base alle esigenze.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >In una campagna avanzata con trigger e filtri, i trigger si trovano nella parte superiore. Quando viene attivato, solo le persone che soddisfano i criteri del filtro passano attraverso il flusso.

   >[!NOTE]
   >
   >Con più attivatori, una persona passa al flusso se QUALSIASI attivatore viene attivato.

   Per eseguire la campagna su un insieme di persone tutte contemporaneamente, scopri come [definire un elenco smart per una campagna smart batch](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [Definire un elenco avanzato per Smart Campaign | Batch](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Definire un elenco avanzato per le attività di personalizzazione web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Abilita contenuti predittivi per contenuti multimediali web](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [Abilita la barra delle raccomandazioni del contenuto](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)

