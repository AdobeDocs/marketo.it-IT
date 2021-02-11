---
unique-page-id: 14352476
description: Campo Tipo di attività sulle attività (SFDC) - Documenti Marketo - Documentazione prodotto
title: Campo Tipo di attività sulle attività (SFDC)
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Campo Tipo di attività sulle attività (SFDC) {#activity-type-field-on-tasks-sfdc}

Con l&#39;aiuto di Sales Connect potete far registrare e-mail e chiamate come attività in Salesforce. Una parte chiave per avere dati importanti in Salesforce è che il campo Tipo compili il valore corretto.

>[!NOTE]
>
>Le e-mail di registrazione tramite CCN non verranno visualizzate nell&#39;elenco di selezione Tipo attività, ma verranno automaticamente compilate come &quot;email&quot; dal momento che vengono inviate a Salesforce tramite il tuo indirizzo CCN.

## Requisiti {#requirements}

* Connessione con Salesforce
* Nessun valore Tipo predefinito selezionato nell&#39;elenco di selezione Tipo attività
* Call, Reply e Email devono essere tutti presenti nella casella di controllo Tipo task (maiuscole)
* Nessun flusso di lavoro o trigger che interviene sul valore del campo Tipo

## Configurazione {#setup}

Innanzitutto verificate di disporre dei valori corretti per la selezione. Avrai bisogno dell&#39;aiuto dell&#39;amministratore Salesforce per apportare eventuali modifiche all&#39;elenco di selezione.

1. Andate su [Salesforce.com](https://salesforce.com) e fate clic su Configurazione nell&#39;angolo in alto a destra.
1. Fate clic su Personalizza.
1. Fate clic su Attività.
1. Fare clic su Campi attività.
1. Fate clic su Tipo.
1. Ora ti trovi nell&#39;elenco dei suggerimenti per il tipo di attività. Assicurarsi che non sia selezionata l&#39;opzione &quot;Predefinito&quot;.
1. Accertatevi che sia elencato un valore Tipo per E-mail, Chiamata e Risposta.

Ora che è già presente, il campo Tipo compila il valore corrispondente per le e-mail registrate, le chiamate e le risposte. Questi valori **non** verranno inseriti nelle attività promemoria di Sales Connect.

>[!NOTE]
>
>Se non viene visualizzato il valore &quot;Rispondi&quot;, aggiungilo facendo clic su **Nuovo**. &#39;Reply&#39; non è un valore standard in Salesforce.
