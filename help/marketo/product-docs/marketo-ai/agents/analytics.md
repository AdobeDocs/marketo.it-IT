---
description: Parla con Marketo AI dei tuoi dati sulle prestazioni di Marketo Engage. Poni le tue domande in un linguaggio semplice e ottieni le risposte nel tuo ambiente Marketo.
title: Analisi
beta: true
hide: true
source-git-commit: cb30495d71d5b4d4fe86d33eed0677eaee882c5e
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Analisi {#analytics}

Analytics ti consente di parlare dei dati sulle prestazioni di Marketo. Poni le tue domande in un linguaggio semplice e ottieni le risposte nel tuo ambiente Marketo.

>[!PREREQUISITES]
>
>È necessario avere accesso ai programmi e ai report di cui si desidera ottenere informazioni.

## Come usare {#how-to-use}

1. In Il mio Marketo, fai clic sul riquadro **Genera con IA**.

1. Nella finestra del prompt, porre una domanda sulle prestazioni. Specifica l’intervallo di tempo o il programma, se ne hai in mente uno.

1. Rivedi il riepilogo delle restituzioni di Marketo AI. Includerà metriche chiave come tassi di apertura, tassi di clic, tassi di conversione e conteggi di lead a seconda delle domande.

1. Fai domande di follow-up per esplorare aree specifiche (ad esempio, &quot;Quale e-mail in quel programma ha avuto il click rate più alto?&quot; o &quot;Come si confronta con l&#39;ultimo trimestre?&quot;).

## Casi d’uso {#use-cases}

**Revisione trimestrale del programma**: un responsabile della generazione della domanda sta preparando una riunione di revisione della campagna. Chiedono: &quot;Come hanno fatto i miei programmi di nutrizione Q2 nel complesso?&quot; Marketo AI restituisce i tassi aperti, i tassi di clic per aprire, i tassi di annullamento dell’abbonamento e il numero di persone/lead che hanno progredito verso MQL in tutti i programmi di crescita del secondo trimestre, con una nota su quali programmi hanno superato la media del gruppo.

**Confronto di due campagne**: un manager della campagna ha eseguito due versioni di una serie di inviti al webinar con argomenti diversi. Chiedono: &quot;Come è andato il programma del webinar di aprile rispetto a quello di marzo in termini di tasso di registrazione?&quot; Marketo AI restituisce i numeri di registrazione per ciascuno di essi ed evidenzia la differenza, in modo che possano vedere quale approccio ha funzionato meglio.

**Ricerca di contenuti dalle prestazioni migliori**: uno specialista di operazioni di marketing vuole sapere quali risorse e-mail hanno determinato il maggior coinvolgimento il mese scorso. Si chiedono: &quot;Quali e-mail hanno registrato i tassi di clic più elevati a maggio?&quot; IA per Marketo restituisce un elenco classificato di risorse e-mail con percentuali di clic, in modo che possa identificare la risposta e informare le future decisioni sui contenuti.

## Aspetti da considerare {#things-to-note}

* **Le risposte di Analytics si basano sui dati disponibili nell&#39;istanza di Marketo**: se non si tiene traccia di un programma o non si acquisisce una metrica, Marketo AI non sarà in grado di generare report su di esso.
* **Intervalli di date molto grandi o domande generiche possono restituire riepiloghi di alto livello anziché dettagli granulari**: Ad esempio, &quot;Come sono stati eseguiti tutti i programmi negli ultimi due anni?&quot;
* **Marketo AI può rendere visibili i dati ma non può apportare modifiche** ai programmi o ai report in base a ciò che trova.
* **Per rapporti personalizzati dettagliati con filtri e raggruppamenti specifici**, gli strumenti di reporting incorporati di Marketo o un&#39;integrazione BI potrebbero essere più appropriati.
* **L&#39;attribuzione in campagne multi-touch richiede la corretta configurazione del programma**: Marketo AI segnalerà ciò che è stato tracciato, non dedurrà l&#39;attribuzione che non è stata configurata.
