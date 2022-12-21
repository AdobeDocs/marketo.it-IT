---
unique-page-id: 14352476
description: Campo Tipo di attività sulle attività (SFDC) - Documenti Marketo - Documentazione del prodotto
title: Campo Tipo di attività sulle attività (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Campo Tipo di attività sulle attività (SFDC) {#activity-type-field-on-tasks-sfdc}

Con l&#39;aiuto di Sales Connect è possibile registrare le e-mail e le chiamate come attività in Salesforce. Una parte chiave per avere dati importanti in Salesforce è che il campo Tipo compila il valore corretto.

>[!NOTE]
>
>La registrazione delle e-mail tramite CCN non verrà visualizzata nella lista di selezione Tipo di attività e verrà compilata automaticamente come campo di tipo &quot;e-mail&quot;, in quanto vengono consegnate a Salesforce tramite il tuo indirizzo CCN.

## Requisiti {#requirements}

* Connessione con Salesforce
* Nessun valore di tipo predefinito selezionato nell&#39;elenco a discesa Tipo task
* Chiamata, Risposta ed E-mail devono essere tutti presenti nell&#39;elenco a discesa Tipo di attività (questioni relative alla capitalizzazione)
* Nessun flusso di lavoro o attivatore che agisce sul valore del campo Tipo

## Configurazione {#setup}

Prima di tutto, controlla di avere i valori corretti per la selezione. Per apportare eventuali modifiche alla tua lista di selezione, ti servirà l’aiuto dell’amministratore Salesforce.

1. Passa a [Salesforce.com](https://salesforce.com) e fai clic su Configurazione nell&#39;angolo in alto a destra.
1. Fai clic su Personalizza.
1. Fai clic su Attività .
1. Fare clic su Campi attività.
1. Fare clic su Tipo.
1. Ora ti trovi nell’elenco a discesa Tipo di attività . Assicurati che non sia selezionato &quot;Predefinito&quot;.
1. Assicurati che sia presente un valore Tipo elencato per E-mail, Chiamata e Risposta.

Ora che è attivo, il campo Tipo compila il valore corrispondente per le e-mail registrate, le chiamate e le risposte. Questi valori **not** compilati nelle attività promemoria di Sales Connect.

>[!NOTE]
>
>Se non trovi &quot;Risposta&quot; come valore, aggiungilo facendo clic su **Nuovo**. &#39;Reply&#39; non è un valore standard in Salesforce.
