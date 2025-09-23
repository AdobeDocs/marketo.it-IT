---
description: Aggiornamento del campo Tipo di attività durante la registrazione delle attività in Salesforce - Documentazione di Marketo - Documentazione del prodotto
title: Aggiornare il campo Tipo di attività durante la registrazione delle attività in Salesforce
exl-id: 800323cb-2b99-42f1-ae30-0f87a9a1b4be
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 6%

---

# Aggiornare il campo Tipo di attività durante la registrazione delle attività in Salesforce {#update-activity-type-field-when-logging-activities-to-salesforce}

Le azioni possono sincronizzare automaticamente le attività e-mail e chiamate a Salesforce da utilizzare per la generazione di rapporti e aumentare la visibilità nella cronologia delle attività. Durante la registrazione delle attività, accertati che il campo Tipo di attività sia aggiornato correttamente in E-mail, Chiamata o Risposta, a seconda del tipo di attività registrata.

>[!NOTE]
>
>La registrazione delle e-mail tramite Ccn non viene eseguita nell’elenco a discesa Tipo di attività, ma viene automaticamente compilata come &quot;e-mail&quot; nel campo Tipo, poiché vengono inviate a Salesforce tramite il tuo indirizzo Ccn.

## Aspetti da comprendere {#things-to-know}

* È necessaria una connessione con Salesforce per aggiornare il Tipo di attività.
* Nell&#39;elenco a discesa Tipo di task non deve essere selezionato alcun valore Tipo predefinito.
* Chiamata, Risposta ed E-mail devono essere presenti nell&#39;elenco a discesa Tipo di task (le maiuscole sono importanti).
* I flussi di lavoro o i trigger in Salesforce che aggiornano il campo Tipo di attività possono interferire con questo processo.

## Configurazione {#setup}

Verifica innanzitutto di disporre dei valori corretti per l’elenco a discesa. Per apportare eventuali modifiche all’elenco a discesa è necessario l’aiuto dell’amministratore di Salesforce.

Verifica innanzitutto quali valori mancano nell’elenco a discesa Tipo di attività (da E-mail, Chiamata e Risposta). Potresti aver bisogno dell&#39;aiuto del tuo amministratore di Salesforce per rivedere e apportare modifiche all&#39;elenco a discesa Tipo di attività. Per apportare queste modifiche, l’amministratore di Salesforce può seguire la procedura riportata di seguito.

### In Salesforce Lightning {#salesforce-lightning}

1. Passa a [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Fai clic sull&#39;icona ingranaggio nell&#39;angolo in alto a destra e seleziona **Configurazione** > **Gestione oggetti**.
1. Digitare &quot;task&quot; nella casella Ricerca rapida.
1. Nel pannello a sinistra, fai clic su **Campi e relazioni**.
1. Fare clic sull&#39;etichetta del campo **Tipo**.
1. In Tipo di attività Valore elenco a discesa, fare clic su **Nuovo**.
1. Digita il nome dei valori mancanti nell’elenco a discesa Tipo di attività (&quot;E-mail, &quot;Chiamata&quot;, &quot;Risposta&quot;).
1. Fai clic su **Salva**.

### In Salesforce Classic {#salesforce-classic}

1. Passa a [Salesforce.com](https://salesforce.com){target="_blank"}.
1. Fai clic su **Configurazione** > **Build** > **Personalizza** > **Attività** > **Campi attività**.
1. Fare clic su **Tipo**.
1. In Tipo di attività Valore elenco a discesa, fare clic su **Nuovo**.
1. Digita il nome dei valori mancanti nell’elenco a discesa Tipo di attività (&quot;E-mail, &quot;Chiamata&quot;, &quot;Risposta&quot;).
1. Fai clic su **Salva**.

Ora che questa è attiva, inizierai a vedere che il campo Tipo popola il valore corrispondente per e-mail, chiamate e risposte registrate. Questi valori _non_ verranno inseriti nelle attività promemoria delle azioni di Sales Insight.

>[!NOTE]
>
>Se il valore &quot;Reply&quot; (Risposta) non è visualizzato, aggiungerlo facendo clic su **New**. &quot;Reply&quot; (Rispondi) non è un valore standard in Salesforce.

>[!MORELIKETHIS]
>
>* [Registrazione degli attributi dell&#39;attività di vendita in Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [Configura personalizzazione dettagli attività Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [Sincronizza attività di vendita con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
