---
description: Registra i motivi delle chiamate e gli esiti delle chiamate a Salesforce - Documentazione Marketo - Documentazione del prodotto
title: Registrare i motivi e gli esiti delle chiamate in Salesforce
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 4%

---

# Registra i motivi e gli esiti delle chiamate a [!DNL Salesforce] {#log-call-reasons-and-call-outcomes-to-salesforce}

Se desideri registrare i risultati delle chiamate e i motivi delle chiamate a [!DNL Salesforce] a scopo di reporting o visibilità, puoi creare un campo attività personalizzato per ciascuno di essi. Ogni campo deve utilizzare un nome API specifico (noto come &quot;Nome campo&quot; in [!DNL Salesforce]).

* Nome campo risultati chiamata: mktosales_call_result
* Nome campo motivi chiamata: mktosales_call_reason

Per utilizzare questi campi, devi innanzitutto crearli come campo attività personalizzato. Per renderlo visibile agli utenti, è necessario aggiungerlo al layout della pagina dell&#39;oggetto attività.

## [!DNL Salesforce] Classic {#salesforce-classic}

### Crea campo attività personalizzato in [!DNL Salesforce] Classic  {#create-custom-activity-field-in-salesforce-classic}

1. In [!DNL Salesforce], fare clic su **[!UICONTROL Setup]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Digita &quot;Attività&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Fai clic su **[!UICONTROL Activity Custom Fields]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Fai clic su **[!UICONTROL New]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Selezionare il tipo di dati &quot;[!UICONTROL Text]&quot; e fare clic su **[!UICONTROL Next]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Assegna al campo personalizzato il nome del campo come definito in precedenza. La lunghezza del campo è limitata a 255 caratteri. Etichetta campo sarà il campo visibile al team di vendita e può essere personalizzato in base alle esigenze del team.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. Le altre impostazioni sono facoltative. Dopo aver completato la configurazione, fare clic su **[!UICONTROL Next]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Selezionare le impostazioni di protezione a livello di campo desiderate per il campo e fare clic su **[!UICONTROL Next]** (l&#39;immagine seguente è solo un esempio).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Assicurati che il campo personalizzato sia visibile al profilo utilizzato dagli utenti di [!DNL Sales Connect], insieme a qualsiasi altro elemento che desideri rendere visibile.

1. Selezionare i layout di pagina a cui si desidera aggiungere il campo e fare clic su **[!UICONTROL Save]** (facoltativamente, è possibile fare clic su **[!UICONTROL Save & New]** e ripetere la procedura per il campo Motivo chiamata).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Aggiungi Campo Attività Personalizzato Al Layout Della Pagina Attività In [!DNL Salesforce] Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>Segui questi passaggi solo se non hai selezionato il layout di pagina desiderato nel passaggio 9 precedente.

1. In [!DNL Salesforce], fare clic su **[!UICONTROL Setup]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Digitare &quot;Task&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Fai clic su **[!UICONTROL Task Page Layouts]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Fare clic su **[!UICONTROL Edit]** accanto al layout della pagina attività a cui si desidera aggiungere il campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Trascinare e rilasciare il campo nella sezione desiderata del layout della pagina Attività.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## [!DNL Salesforce] fulmine {#salesforce-lightning}

### Crea campo attività personalizzato in [!DNL Salesforce] Fulmine {#create-custom-activity-field-in-salesforce-lightning}

1. In [!DNL Salesforce], fare clic sull&#39;icona ingranaggio in alto a destra e selezionare **[!UICONTROL Setup]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. Fai clic su **[!UICONTROL Object Manager]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. Digitare &quot;[!UICONTROL Activity]&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. Fare clic sull&#39;etichetta **[!UICONTROL Activity]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. Fai clic su **[!UICONTROL Fields & Relationships]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. Fai clic su **[!UICONTROL New]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### Aggiungi campo attività personalizzato al layout della pagina attività in [!DNL Salesforce] Fulmine {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. In [!DNL Salesforce], fare clic sull&#39;icona ingranaggio in alto a destra e selezionare **[!UICONTROL Setup]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. Fai clic su **[!UICONTROL Object Manager]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. Digitare &quot;[!UICONTROL Task]&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. Fare clic sull&#39;etichetta **[!UICONTROL Task]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. Fai clic su **[!UICONTROL Page Layouts]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. Fare clic sul layout della pagina dell&#39;attività a cui si desidera aggiungere il campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. Trascinare e rilasciare il campo nella sezione desiderata del layout della pagina Attività.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>[Installa i campi evento Sales Connect nella cronologia attività](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
