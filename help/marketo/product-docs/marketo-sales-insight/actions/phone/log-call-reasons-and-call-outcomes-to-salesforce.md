---
description: Motivi delle chiamate e risultati delle chiamate a Salesforce - Marketo Docs - Documentazione del prodotto
title: Segnala i motivi delle chiamate e i risultati delle chiamate a Salesforce
source-git-commit: 0864f784d193bfc6dd7a087c9f89ce59bdff710c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Segnala i motivi delle chiamate e i risultati delle chiamate a Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Se desideri registrare i risultati delle chiamate e chiamare i motivi a Salesforce a scopo di reporting o visibilità, puoi creare un campo di attività personalizzato per ciascuno di essi. Ogni campo deve utilizzare un nome API specifico (noto come &quot;Nome campo&quot; in Salesforce).

* Nome campo risultati chiamata: mktosales_call_result
* Nome campo motivi chiamata: mktosales_call_reason

Per utilizzare questi campi, devi innanzitutto creare il campo come campo di attività personalizzato. Per renderlo visibile agli utenti, è necessario aggiungerlo al layout della pagina dell&#39;oggetto attività.

## Salesforce Classic {#salesforce-classic}

### Crea campo attività personalizzato in Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Digitare &quot;Attività&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Fai clic su **Campi personalizzati dell’attività**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Fai clic su **Nuovo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Seleziona il tipo di dati &quot;Testo&quot; e fai clic su **Successivo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Assegnare al campo personalizzato il nome del campo come definito in precedenza. La lunghezza del campo ha un limite di 255 caratteri. Etichetta campo sarà il campo visibile al team di vendita e può essere personalizzato per soddisfare le esigenze del team.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. Il resto delle impostazioni è facoltativo. Una volta completata la configurazione, fai clic su **Successivo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Selezionare le impostazioni di protezione a livello di campo desiderate per questo campo e fare clic su **Successivo** (l’immagine seguente è solo un esempio).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Assicurati che il campo personalizzato sia visibile al profilo utilizzato dagli utenti per le azioni Approfondimenti vendite, insieme a qualsiasi altro campo desiderato.

1. Selezionare i layout di pagina a cui si desidera aggiungere il campo e fare clic su **Salva** (facoltativamente, puoi fare clic su **Salva e nuovo** e ripetere il processo per il campo Motivo della chiamata).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Aggiungi campo attività personalizzato al layout della pagina attività in Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>Sarà necessario seguire questi passaggi solo se non hai selezionato il layout di pagina desiderato nel passaggio 9 precedente.

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Digitare &quot;Task&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Fai clic su **Layout delle pagine attività**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Fai clic su **Modifica** accanto al layout della pagina attività a cui si desidera aggiungere questo campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Trascina il campo nella sezione desiderata del layout della pagina Attività.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. Fai clic su **Salva**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## Fulmine Salesforce {#salesforce-lightning}

### Crea campo attività personalizzato in fulmine di Salesforce {#create-custom-activity-field-in-salesforce-lightning}

1. In Salesforce, fai clic sull&#39;icona dell&#39;ingranaggio in alto a destra e seleziona **Configurazione**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. Fai clic su **Gestione oggetti**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. Digitare &quot;Attività&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. Fai clic sul pulsante **Attività** etichetta.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. Fai clic su **Campi e correlazioni**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. Fai clic su **Nuovo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### Aggiungi campo attività personalizzato al layout della pagina attività in Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. In Salesforce, fai clic sull&#39;icona dell&#39;ingranaggio in alto a destra e seleziona **Configurazione**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. Fai clic su **Gestione oggetti**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. Digitare &quot;Task&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. Fai clic sul pulsante **Attività** etichetta.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. Fai clic su **Layout di pagina**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. Fare clic sul layout della pagina attività a cui si desidera aggiungere il campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. Trascina il campo nella sezione desiderata del layout della pagina Attività.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. Fai clic su **Salva**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>* [Risultati chiamata](/help/marketo/product-docs/marketo-sales-insight/actions/phone/call-outcomes.md)
>* [Motivi della chiamata](/help/marketo/product-docs/marketo-sales-insight/actions/phone/call-reasons.md)

