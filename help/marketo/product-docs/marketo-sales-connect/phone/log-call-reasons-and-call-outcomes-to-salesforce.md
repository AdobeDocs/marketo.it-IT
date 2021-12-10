---
description: Motivi delle chiamate e risultati delle chiamate a Salesforce - Marketo Docs - Documentazione del prodotto
title: Segnala i motivi delle chiamate e i risultati delle chiamate a Salesforce
hide: true
hidefromtoc: true
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
source-git-commit: 0fc2551ffc85260a282b64995c698098846eb10c
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

1. In Salesforce, fai clic su **Configurazione**.

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
   >Assicurati che il campo personalizzato sia visibile al profilo utilizzato dagli utenti di Sales Connect, insieme a qualsiasi altro campo desiderato.

1. Selezionare i layout di pagina a cui si desidera aggiungere il campo e fare clic su **Salva** (facoltativamente, puoi fare clic su **Salva e nuovo** e ripetere il processo per il campo Motivo della chiamata).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Aggiungi campo attività personalizzato al layout della pagina attività in Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Digitare &quot;Task&quot; nella casella Ricerca rapida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Fai clic su **Layout delle pagine attività**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Fai clic su **Modifica** accanto al layout della pagina attività a cui si desidera aggiungere questo campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Trascina il campo nel layout della pagina Attività.

   PICC

1. Fai clic su **Salva**.

   PICC

## Fulmine Salesforce {#salesforce-lightning}

### Crea campo attività personalizzato in fulmine di Salesforce {#create-custom-activity-field-in-salesforce-lightning}

1. In Salesforce, fai clic sull&#39;icona dell&#39;ingranaggio in alto a destra.

PICC

1. Fai clic su **Configurazione**.

PICC

1. Fai clic su **Gestione oggetti**.

PICC

1. Immetti Attività nella casella Ricerca rapida e fai clic sull’etichetta Attività per aprire la configurazione dell’oggetto.

PICC

1. Sul lato sinistro, fai clic su **Campi e correlazioni**.

PICC

1. Fai clic su **Nuovo**.

PICC

## Aggiungi campo attività personalizzato al layout della pagina attività in Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. In Salesforce, fai clic sull&#39;icona dell&#39;ingranaggio in alto a destra.

PICC

1. Fai clic su **Configurazione**.

PICC

1. Vai al programma di installazione????????

PICC

1. Digitare &quot;Task&quot; nella casella Ricerca rapida.

PICC

1. Fai clic su Attività.

PICC

1. Fare clic su Layout di pagina.

PICC

1. Fare clic sul layout della pagina attività a cui si desidera aggiungere il campo.

PICC

1. Trascina il campo nel layout della pagina Attività.

PICC

1. Fai clic su Salva.

PICC

>[!MORELIKETHIS]
>
>[Installa i campi evento Sales Connect nella cronologia delle attività](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
