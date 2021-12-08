---
description: Motivi delle chiamate e risultati delle chiamate a Salesforce - Marketo Docs - Documentazione del prodotto
title: Segnala i motivi delle chiamate e i risultati delle chiamate a Salesforce
hide: true
hidefromtoc: true
source-git-commit: 1dd4a4f6bfac0b101f85f3776396aeef1a1f7182
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Segnala i motivi delle chiamate e i risultati delle chiamate a Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Se desideri registrare i risultati delle chiamate e chiamare i motivi a Salesforce a scopo di reporting o visibilità, puoi creare un campo di attività personalizzato per ciascuno di essi. Ogni campo deve utilizzare un nome API specifico.

* Nome API dei risultati della chiamata: mktosales_call_result
* Nome API dei motivi della chiamata: mktosales_call_reason

Per utilizzare questi campi, devi innanzitutto creare il campo come campo di attività personalizzato. Per renderlo visibile agli utenti, è necessario aggiungerlo al layout della pagina dell&#39;oggetto attività.

## Crea campo attività personalizzato in Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. In Salesforce, vai a Configurazione.

PICC

1. Immettere &quot;Attività&quot; nella casella Ricerca rapida.

PICC

1. Fai clic su **Campi personalizzati dell’attività**.

PICC

1. Fai clic su **Nuovo**.

PICC

## Crea campo attività personalizzato in fulmine di Salesforce {#create-custom-activity-field-in-salesforce-lightning}

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

## Aggiungi campo attività personalizzato al layout della pagina attività in Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

PASSAGGI

## Aggiungi campo attività personalizzato al layout della pagina attività in Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

PASSAGGI

>[!MORELIKETHIS]
>
>[Installa i campi evento Sales Connect nella cronologia delle attività](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
