---
description: Aggiorna il campo del tipo di attività durante la registrazione delle attività in Salesforce - Documenti Marketo - Documentazione del prodotto
title: Aggiorna il campo del tipo di attività durante la registrazione delle attività in Salesforce
exl-id: 800323cb-2b99-42f1-ae30-0f87a9a1b4be
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 1%

---

# Aggiorna il campo del tipo di attività durante la registrazione delle attività in Salesforce {#update-activity-type-field-when-logging-activities-to-salesforce}

Le azioni possono sincronizzare automaticamente le e-mail e richiamare le attività in Salesforce per utilizzarle a scopo di reporting e aumentare la visibilità nella cronologia delle attività. Durante la registrazione delle attività, accertati che il campo Tipo di attività sia aggiornato correttamente in E-mail, Chiamata o Risposta, a seconda del tipo di attività registrata.

>[!NOTE]
>
>La registrazione delle e-mail tramite Ccn non viene eseguita nella lista di selezione Tipo di attività, ma viene automaticamente compilata come &quot;e-mail&quot; nel campo Tipo, poiché le e-mail vengono inviate a Salesforce tramite il tuo indirizzo Ccn.

## Aspetti da considerare {#things-to-know}

* È necessaria una connessione con Salesforce per aggiornare il Tipo di attività.
* Nell&#39;elenco a discesa Tipo di task non deve essere selezionato alcun valore Tipo predefinito.
* Chiamata, Risposta ed E-mail devono essere presenti nell&#39;elenco a discesa Tipo di task (le maiuscole sono importanti).
* I flussi di lavoro o i trigger in Salesforce che aggiornano il campo Tipo di attività possono interferire con questo processo.

## Configurazione {#setup}

Verifica innanzitutto di disporre dei valori corretti per l’elenco a discesa. Per apportare qualsiasi modifica alla tua lista di selezione dovrai chiedere aiuto all’amministratore Salesforce.

Verifica innanzitutto quali valori mancano nell’elenco a discesa Tipo di attività (da E-mail, Chiamata e Risposta). Potresti aver bisogno dell&#39;aiuto del tuo amministratore Salesforce per rivedere questo e apportare modifiche al tuo elenco a discesa Tipo di attività. Per apportare queste modifiche, l’amministratore Salesforce può seguire la procedura riportata di seguito.

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

Ora che questa è attiva, inizierai a vedere che il campo Tipo popola il valore corrispondente per e-mail, chiamate e risposte registrate. Questi valori _non_ verranno inseriti nelle attività promemoria delle azioni di approfondimento vendite.

>[!NOTE]
>
>Se il valore &quot;Reply&quot; (Risposta) non è visualizzato, aggiungerlo facendo clic su **New**. &quot;Reply&quot; (&quot;Risposta&quot;) non è un valore standard in Salesforce.

>[!MORELIKETHIS]
>
>* [Registrazione degli attributi dell&#39;attività di vendita in Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/logging-sales-activity-attributes-to-salesforce.md){target="_blank"}
>* [Configura Personalizzazione Dettagli Attività Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md){target="_blank"}
>* [Sincronizza attività di vendita con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md){target="_blank"}
