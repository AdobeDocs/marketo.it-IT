---
unique-page-id: 14352476
description: Campo Tipo di attività sulle attività (SFDC) - Documentazione di Marketo - Documentazione del prodotto
title: Campo Tipo di attività sulle attività (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Campo Tipo di attività sulle attività (SFDC) {#activity-type-field-on-tasks-sfdc}

Con l’aiuto di Sales Connect puoi registrare le tue e-mail e chiamate come attività in Salesforce. Una parte fondamentale per avere dati importanti in Salesforce è far sì che il campo Tipo compili il valore corretto.

>[!NOTE]
>
>La registrazione delle e-mail tramite Ccn non viene eseguita nell’elenco a discesa Tipo di attività, ma viene automaticamente compilata come &quot;e-mail&quot; nel campo Tipo, poiché le e-mail vengono inviate a Salesforce tramite il tuo indirizzo Ccn.

## Requisiti {#requirements}

* Connessione con Salesforce
* Nessun valore Tipo predefinito selezionato nell&#39;elenco a discesa Tipo di task
* Chiamata, Risposta ed E-mail devono essere presenti nell&#39;elenco a discesa Tipo di task (le maiuscole sono importanti)
* Nessun flusso di lavoro o trigger che interviene sul valore del campo Tipo

## Configurazione {#setup}

Verifica innanzitutto di disporre dei valori corretti per l’elenco a discesa. Per apportare qualsiasi modifica alla tua lista di selezione dovrai chiedere aiuto all’amministratore Salesforce.

1. Accedi a [Salesforce.com](https://salesforce.com) e fai clic su Configurazione nell’angolo in alto a destra.
1. Fai clic su Personalizza.
1. Fai clic su Attività.
1. Fare clic su Campi attività.
1. Fare clic su Tipo.
1. Ora ti trovi nell’elenco a discesa Tipo di attività. Assicurati che non sia selezionato &quot;Predefinito&quot;.
1. Assicurati che sia elencato un valore Tipo per E-mail, Chiamata e Risposta.

Ora che questa è attiva, inizierai a vedere che il campo Tipo popola il valore corrispondente per e-mail, chiamate e risposte registrate. Questi valori _non_ essere compilati nelle attività promemoria di Sales Connect.

>[!NOTE]
>
>Se il valore &quot;Reply&quot; (Risposta) non è visibile, aggiungerlo facendo clic su **Nuovo**. &quot;Reply&quot; (&quot;Risposta&quot;) non è un valore standard in Salesforce.
