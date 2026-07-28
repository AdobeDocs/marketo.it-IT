---
description: Scopri in che modo i criteri di conservazione dei dati di 25 mesi e 90 giorni di Marketo influiscono sui rapporti di Analytics, con un raggruppamento per rapporto e suggerimenti per la conservazione dei dati più a lungo.
title: Conservazione dei dati
feature: Reporting
source-git-commit: 8eb9fd285e5dd055603579fbb5e7a4c4eb681172
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 5%

---

# Criteri di conservazione dei dati sulle attività di Marketo - Impatto sul reporting

Marketo conserva i dati dell’attività di marketing su base continua. I dati relativi all’attività e all’iscrizione alla campagna vengono memorizzati per un periodo continuo di 25 mesi oltre la data dell’attività e i dati relativi all’attività per un volume elevato vengono conservati per un periodo continuo di 90 giorni oltre la data dell’attività per impostazione predefinita, che può essere regolato per utente. Oltre questi periodi di conservazione, i dati non sono più disponibili tramite l’interfaccia utente di Marketo.

## Rapporti di Marketo Analytics

Poiché i dati delle attività vengono conservati per un massimo di 25 mesi, alcuni rapporti di Marketo Analytics sono interessati da questo criterio, mentre altri no. I rapporti che estraggono dati dai registri di attività della persona mostreranno dati solo per un massimo di 25 mesi. I rapporti che non fanno assolutamente riferimento all’attività della persona non vengono interessati.

Tuttavia, anche i rapporti che non fanno riferimento all’attività della persona per impostazione predefinita possono essere interessati se vengono aggiunti filtri all’elenco avanzato del rapporto. I filtri che fanno riferimento agli attributi della persona (informazioni nei campi del record persona) non causano alcuna modifica al rapporto. I filtri che cercano le attività che la persona ha intrapreso possono accedere solo alle attività all’interno dell’intervallo di conservazione, quindi se l’attività si è verificata più tempo di così, i risultati del rapporto verranno modificati.

La tabella seguente riepiloga il comportamento di ogni rapporto, inclusi gli scenari di filtro comuni.

## Riferimento report

| Tipo di report | Filtra scenario | Interessato dai criteri di conservazione? |
|---|---|---|
| **Rapporti di Revenue Cycle Explorer** | Nessun filtro disponibile | No: gli utenti di Revenue Cycle Explorer e Advanced Analytics sono completamente esenti da questi limiti di conservazione. I dati RCE vengono inviati durante la notte in un server di database separato che gestisce il reporting RCE. Poiché è memorizzato separatamente e non nei registri di attività di persona, questi rapporti non sono interessati da questo criterio. La funzione di gestione del ciclo dei ricavi non estrae dati direttamente dal database delle persone, pertanto i filtri non sono disponibili. |
| **Rapporto prestazioni persone** | Nessun filtro elenco avanzato | No |
| | Filtri per attributi persona (Esempio: Nome) | No |
| | Filtri sulle attività personali negli ultimi 25 mesi | No |
| | Filtri per attività persona senza vincoli di data | Sì |
| **Persone per stato** | Nessun filtro elenco avanzato | No |
| | Filtri per attributi persona (Esempio: Nome) | No |
| | Filtri sulle attività personali negli ultimi 25 mesi | No |
| | Filtri per attività persona senza vincoli di data | Sì |
| **Persone per fase ricavi** | Nessun filtro elenco avanzato | No |
| | Filtri per attributi persona (Esempio: Nome) | No |
| | Filtri sulle attività personali negli ultimi 25 mesi | No |
| | Filtri per attività persona senza vincoli di data | Sì |
| **Analisi del percorso di successo** | Non include elenchi avanzati | N/D |
| **Rapporto di influenza social network** | Nessun filtro elenco avanzato | Sì |
| | Filtri per attributi persona (Esempio: Nome) | Sì |
| | Filtri sulle attività personali negli ultimi 25 mesi | Sì |
| | Filtri per attività persona senza vincoli di data | Sì |
| **Analisi influenza opportunità** | Non include elenchi avanzati | No |
| **Prestazioni e-mail** | Nessun filtro elenco avanzato | No |
| | Filtri per attributi persona (Esempio: Nome) | No |
| | Filtri sulle attività personali negli ultimi 25 mesi | No |
| | Filtri per attività persona senza vincoli di data | Sì |
| **Prestazioni collegamento e-mail** | Nessun filtro elenco avanzato | No |
| | Filtri per attributi persona (Esempio: Nome) | No |
| | Filtri sulle attività personali negli ultimi 25 mesi | No |
| | Filtri per attività persona senza vincoli di data | Sì |
| **Informazioni e-mail** | Non utilizza elenchi avanzati | No |
| **Prestazioni e-mail Insight per vendite** | Nessun filtro elenco avanzato | No |
| | Filtri per attributi persona (Esempio: Nome) | No |
| | Filtri sulle attività personali negli ultimi 25 mesi | No |
| | Filtri per attività persona senza vincoli di data | Sì |
| **Prestazioni Pagina Di Destinazione** | Nessun filtro elenco avanzato | No: i dati sulle prestazioni della pagina di destinazione vengono conservati a tempo indeterminato e non sono soggetti ai criteri di conservazione. |
| | Filtri per attributi persona (Esempio: Nome) | No |
| | Filtri sulle attività personali negli ultimi 25 mesi | No |
| | Filtri per attività persona senza vincoli di data | No |
| **Attività pagina Web** | Nessun filtro elenco avanzato | Sì: soggetto al periodo di conservazione predefinito di 90 giorni (regolabile per utente) |
| | Filtri per attributi persona (Esempio: Nome) | Sì |
| | Filtri sulle attività personali negli ultimi 25 mesi | Sì |
| | Filtri per attività persona senza vincoli di data | Sì |
| **Attività Web della società** | Nessun filtro elenco avanzato | Sì |
| | Filtri per attributi persona (Esempio: Nome) | Sì |
| | Filtri sulle attività personali negli ultimi 25 mesi | Sì |
| | Filtri per attività persona senza vincoli di data | Sì |
| **Prestazioni Programma** | Nessun filtro elenco avanzato | No |
| | Filtri per attributi persona (Esempio: Nome) | No |
| | Filtri sulle attività personali negli ultimi 25 mesi | No |
| | Filtri per attività persona senza vincoli di data | Sì |
| **Prestazioni flusso di coinvolgimento** | Nessun filtro elenco avanzato | No |
| | Filtri per attributi persona (Esempio: Nome) | No |
| | Filtri sulle attività personali negli ultimi 25 mesi | No |
| | Filtri per attività persona senza vincoli di data | Sì |
| **Analizzatore di programmi** | Non utilizza elenchi avanzati | No |
| **Attività campagna** | Nessun filtro elenco avanzato | No |
| | Filtri per attributi persona (Esempio: Nome) | No |
| | Filtri sulle attività personali negli ultimi 25 mesi | No |
| | Filtri per attività persona senza vincoli di data | Sì |
| **Prestazioni e-mail campagna** | Nessun filtro elenco avanzato | Sì |
| | Filtri per attributi persona (Esempio: Nome) | Sì |
| | Filtri sulle attività personali negli ultimi 25 mesi | Sì |
| | Filtri per attività persona senza vincoli di data | Sì |

## Soluzioni per la generazione di rapporti

I dati relativi alle attività precedenti alla finestra di conservazione possono essere considerati obsoleti da molti utenti. Tuttavia, puoi avere un caso d’uso in cui queste informazioni sono necessarie. Di seguito sono riportati alcuni modi per conservare questi dati oltre il periodo di conservazione standard.

## Esportare i dati

Marketo offre l&#39;[API REST Bulk Extract](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/bulk-extract/bulk-extract), che consente di esportare le attività delle persone e ospitarle localmente. Una volta estratti i dati tramite l’API, puoi memorizzarli e ordinarli in base alle esigenze del caso d’uso.

>[!TIP]
>
>Esporta i dati personali in base a una pianificazione regolare, non una sola volta. Le attività della persona vengono mantenute su un ciclo continuo di 25 mesi. Imposta un promemoria per esportare di nuovo _prima_ della fine dell&#39;intervallo di 25 mesi.

## Usa campi personalizzati

I valori dei campi della persona non sono interessati dai criteri di conservazione dei dati. È possibile utilizzare le campagne avanzate per popolare i campi personalizzati con valori basati sulle attività intraprese dalle persone. Questo consente di filtrare le persone in base a questi attributi personali (non soggetti ai criteri di conservazione) anziché in base alle attività stesse (soggette ai criteri di conservazione).

Un ulteriore vantaggio di questo approccio è che la ricerca per attributi di persona è più veloce della ricerca attraverso i registri delle attività di persona.
