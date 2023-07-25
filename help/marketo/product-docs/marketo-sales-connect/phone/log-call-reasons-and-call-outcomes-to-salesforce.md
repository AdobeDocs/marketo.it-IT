---
description: Registra i motivi delle chiamate e gli esiti delle chiamate a Salesforce - Documenti Marketo - Documentazione del prodotto
title: Registra i motivi e gli esiti delle chiamate a Salesforce
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Registra i motivi e gli esiti delle chiamate a Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Se desideri registrare i risultati delle chiamate e i motivi delle chiamate a Salesforce a scopo di reporting o visibilità, puoi creare un campo attività personalizzato per ciascuno di essi. Ogni campo deve utilizzare un nome API specifico (noto come &quot;Nome campo&quot; in Salesforce).

* Nome campo risultati chiamata: mktosales_call_result
* Nome campo motivi chiamata: mktosales_call_reason

Per utilizzare questi campi, devi innanzitutto crearli come campo attività personalizzato. Per renderlo visibile agli utenti, è necessario aggiungerlo al layout della pagina dell&#39;oggetto attività.

## Salesforce Classic {#salesforce-classic}

### Creare un campo attività personalizzato in Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Digita &quot;Attività&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Clic **Campi personalizzati attività**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Clic **Nuovo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Seleziona il tipo di dati &quot;Text&quot; e fai clic su **Successivo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Assegna al campo personalizzato il nome del campo come definito in precedenza. La lunghezza del campo è limitata a 255 caratteri. Etichetta campo sarà il campo visibile al team di vendita e può essere personalizzato in base alle esigenze del team.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. Le altre impostazioni sono facoltative. Dopo aver completato la configurazione, fai clic su **Successivo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Seleziona le impostazioni di sicurezza a livello di campo desiderate per questo campo e fai clic su **Successivo** (l’immagine qui sotto è solo un esempio).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Accertarsi che il campo personalizzato sia visibile al profilo utilizzato dagli utenti Sales Connect, insieme a qualsiasi altro punto che si desidera rendere visibile.

1. Seleziona i layout di pagina a cui aggiungere il campo e fai clic su **Salva** (facoltativamente, puoi fare clic su **Salva e nuovo** e ripetere la procedura per il campo Motivo chiamata).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Aggiungere un campo attività personalizzato al layout della pagina attività in Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>Segui questi passaggi solo se non hai selezionato il layout di pagina desiderato nel passaggio 9 precedente.

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Digitare &quot;Task&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Clic **Layout di pagina attività**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Clic **Modifica** accanto al layout della pagina attività a cui si desidera aggiungere questo campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Trascinare e rilasciare il campo nella sezione desiderata del layout della pagina Attività.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. Clic **Salva**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## Salesforce Lightning {#salesforce-lightning}

### Creare un campo attività personalizzato in Salesforce Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. In Salesforce, fai clic sull’icona a forma di ingranaggio in alto a destra e seleziona **Configurazione**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. Clic **Gestione oggetti**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. Digitare &quot;Activity&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. Fai clic su **Attività** etichetta.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. Clic **Campi e relazioni**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. Clic **Nuovo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### Aggiungere un campo attività personalizzato al layout della pagina attività in Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. In Salesforce, fai clic sull’icona a forma di ingranaggio in alto a destra e seleziona **Configurazione**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. Clic **Gestione oggetti**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. Digitare &quot;Task&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. Fai clic su **Attività** etichetta.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. Clic **Layout di pagina**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. Fare clic sul layout della pagina dell&#39;attività a cui si desidera aggiungere il campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. Trascinare e rilasciare il campo nella sezione desiderata del layout della pagina Attività.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. Clic **Salva**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>[Installa campi evento Sales Connect nella cronologia attività](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
