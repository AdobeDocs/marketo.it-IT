---
unique-page-id: 10097873
description: Definire un elenco avanzato per le attività di Predictive Content - Marketo Docs - Documentazione prodotto
title: Definire un elenco avanzato per le attività relative ai contenuti predittivi
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---


# Definire un elenco avanzato per le attività relative ai contenuti predittivi {#define-a-smart-list-for-predictive-content-activities}

>[!NOTE]
>
>A seconda della data di acquisto, l’iscrizione a Marketo può includere contenuti predittivi di marketing o contenuti`<sup>AI</sup>`. Per gli utenti che utilizzano contenuti predittivi, Marketo attiva le funzioni di analisi dei contenuti`<sup>AI</sup>` fino al 30 aprile 2018. Per mantenere queste funzionalità oltre tale data, contatta il tuo Customer Success Manager di Marketo per effettuare l&#39;aggiornamento al contenuto`<sup>AI</sup>`di Marketo.

Potete utilizzare le attività di contenuto predittivo in attivatori e filtri quando definite un elenco smart in una campagna intelligente. Potete attivare un’azione per chiunque faccia clic sul contenuto predittivo tramite il modello [](enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)Contenuti multimediali avanzati, la barra [delle raccomandazioni sul](enabling-predictive-content/enable-the-content-recommendation-bar.md)contenuto o un messaggio e-mail.

1. Nella campagna intelligente, andate alla scheda Elenco **** avanzato.

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >**Tubo profondo**
   >
   >
   >Gli elenchi intelligenti possono fare cose straordinarie. Ulteriori informazioni sono disponibili nella sezione approfondita dell&#39;elenco [avanzato](../../product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Cercare l&#39;attivatore, quindi trascinarlo e rilasciarlo sul quadro.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Una campagna intelligente con trigger viene eseguita in modalità Trigger. Viene eseguito su una persona alla volta in base agli eventi attivati e ai filtri aggiunti.

1. Fare clic sul menu a discesa **Nome** e selezionare un operatore.

   ![](assets/smart-list-dropdown-hands.png)

1. Definire il trigger.

   ![](assets/smart-lislt-select-content-hands.png)

1. Aggiungete il vincolo **Tipo** .

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Selezionare l&#39;origine desiderata per l&#39;elenco avanzato.

   ![](assets/pc-add-constraint.png)

1. Se utilizzate l&#39;origine e-mail per il contenuto predittivo, aggiungete l&#39;attivatore **Click Link in Email*. Selezionate il messaggio e-mail e aggiungete il vincolo **Predictive** , definito come **true**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Aggiungete eventuali altri filtri in base alle esigenze.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >In una campagna intelligente con attivatori e filtri, gli attivatori si trovano nella parte superiore. Quando viene attivato, solo gli utenti che soddisfano i criteri del filtro passano attraverso il flusso.

   >[!NOTE]
   >
   >Con più attivatori, una persona passa al flusso se QUALSIASI attivatore viene attivato.

   [definire un elenco smart per una campagna smart batch](../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)

   >[!NOTE]
   >
   >**Articoli correlati**
   >
   >    
   >    
   >    * [Definisci elenco avanzato per Smart Campaign | Batch](../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >    * [Aggiunta di un passaggio di flusso a una campagna intelligente](../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >    * [Definire un elenco avanzato per le attività di personalizzazione Web](../../product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >    * [Abilita contenuto predittivo per contenuti multimediali Web](enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >    * [Abilita la barra delle raccomandazioni del contenuto](enabling-predictive-content/enable-the-content-recommendation-bar.md)


Per eseguire la campagna su un insieme di persone allo stesso tempo, scopri come .