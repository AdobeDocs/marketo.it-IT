---
description: Parla dei tuoi dati sulle prestazioni con Coworker per Marketo Engage. Poni le tue domande in un linguaggio semplice e ottieni le risposte nel tuo ambiente Marketo Engage.
title: Informazioni sulla superficie
badge: Beta
hide: true
source-git-commit: 224dff93cda319bb6bb59fcbec4edb13cc940f4a
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Informazioni sulla superficie {#surface-insights}

Surface Insights ti consente di parlare dei dati delle prestazioni di Marketo. Poni le tue domande in un linguaggio semplice e ottieni le risposte nel tuo ambiente Marketo.

>[!PREREQUISITES]
>
>* Per utilizzare questa funzione devi prima accettare i [termini Gen-AI di base e i termini supplementari](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Per informazioni, contatta il team dell’account di Adobe (il tuo account manager).
>
>* È necessario avere accesso ai programmi e ai report di cui si desidera ottenere informazioni.

>[!AVAILABILITY]
>
>Questa funzione è attualmente in versione beta chiusa. Non divulgare questa documentazione.

## Come usare {#how-to-use}

1. Nel tuo My Marketo, fai clic sul riquadro **Collaboratore per Marketo Engage**.

1. Nella finestra del prompt, porre una domanda sulle prestazioni. Specifica l’intervallo di tempo o il programma, se ne hai in mente uno.

1. Rivedi il riepilogo delle restituzioni di Collaboratore per Marketo Engage. Includerà metriche chiave come tassi di apertura, tassi di clic, tassi di conversione e conteggi di lead a seconda delle domande.

1. Fai domande di follow-up per esplorare aree specifiche (ad esempio, &quot;Quale e-mail in quel programma ha avuto il click rate più alto?&quot; o &quot;Come si confronta con l&#39;ultimo trimestre?&quot;).

## Casi d’uso {#use-cases}

**Revisione trimestrale del programma**: un responsabile della generazione della domanda sta preparando una riunione di revisione della campagna. Chiedono: &quot;Come hanno fatto i miei programmi di nutrizione Q2 nel complesso?&quot; Il collaboratore di Marketo Engage restituisce i tassi di apertura, i tassi di clic per aprire, i tassi di annullamento dell’abbonamento e il numero di persone/lead che hanno progredito fino a MQL in tutti i programmi di crescita del secondo trimestre, con una nota su quali programmi hanno superato la media del gruppo.

**Confronto di due campagne**: un manager della campagna ha eseguito due versioni di una serie di inviti al webinar con argomenti diversi. Chiedono: &quot;Come è andato il programma del webinar di aprile rispetto a quello di marzo in termini di tasso di registrazione?&quot; Coworker for Marketo Engage restituisce i numeri di registrazione per ciascuno di essi ed evidenzia la differenza, in modo che possano vedere quale approccio ha funzionato meglio.

**Ricerca di contenuti dalle prestazioni migliori**: uno specialista di operazioni di marketing vuole sapere quali risorse e-mail hanno determinato il maggior coinvolgimento il mese scorso. Si chiedono: &quot;Quali e-mail hanno registrato i tassi di clic più elevati a maggio?&quot; Collaboratore per Marketo Engage restituisce un elenco classifica di risorse e-mail con percentuali di clic, in modo che possa identificare gli elementi che hanno avuto una risposta e influenzare le decisioni future sui contenuti.

## Aspetti da considerare {#things-to-note}

* Le informazioni di superficie si basano sui dati disponibili nell’istanza Marketo. Se non viene tracciato un programma o non viene acquisita una metrica, Collaboratore per Marketo Engage non sarà in grado di generare rapporti su di esso.
* Intervalli di date molto ampi o domande di ampia portata possono restituire riepiloghi di alto livello anziché dettagli granulari. Ad esempio, &quot;Come sono andati tutti i miei programmi negli ultimi due anni?&quot;
* Collaboratore per Marketo Engage può rendere visibili i dati, ma non può apportare modifiche ai programmi o ai rapporti in base a ciò che trova.
* Per rapporti personalizzati dettagliati con filtri e raggruppamenti specifici, potrebbe essere più appropriato utilizzare gli strumenti di reporting incorporati di Marketo o un’integrazione BI.
* L’attribuzione tra campagne multi-touch richiede una corretta configurazione del programma. Collaboratore per Marketo Engage genera rapporti su ciò che viene tracciato, non su attribuzioni non configurate.
