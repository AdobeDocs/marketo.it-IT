---
unique-page-id: 5472615
description: Informazioni sui campi gestiti del sistema - Documenti Marketo - Documentazione del prodotto
title: Informazioni sui campi gestiti di sistema
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---


# Informazioni sui campi gestiti di sistema {#understanding-system-managed-fields}

Potreste aver notato che la pagina [dei dettagli della](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) persona presenta una serie di campi non modificabili creati da Marketo. Questi dati provengono da varie fonti, e ci sono innumerevoli valori che possono essere visualizzati.

## Tipi di campi {#field-types}

| **Nome campo** | **Definizione** |
|---|---|
| Tipo origine originale | La posizione di una persona o di un visitatore del sito Web è stata scoperta per la prima volta (esempio: Importazione elenco, Visita pagina Web) |
| Informazioni origine originali | Specifiche relative a tale posizione (esempio: Nome dell’elenco, URL della pagina Web) |
| Motore di ricerca originale | Se applicabile, il motore di ricerca che ha indirizzato la persona all&#39;origine di ingresso originale |
| Frase di ricerca originale | Se applicabile, il termine utilizzato per la ricerca che ha riferito la persona all&#39;origine di ingresso originale |
| Referente originale | URL che ospita l’origine di ingresso originale |
| Tipo origine registrazione | La posizione in cui un&#39;attività è diventata per la prima volta una persona (esempio: Importazione elenco, Visita pagina Web) |
| Informazioni origine registrazione | Specifiche relative a tale posizione (esempio: Nome dell’elenco, URL della pagina Web) |
| IP anonimo | Indica l&#39;indirizzo IP di una persona |
| Società destinataria | La migliore ipotesi di Marketo (basata su IP) sulla società della persona |
| Città di provenienza | La migliore ipotesi di Marketo (basata su IP) sulla città della persona |
| Regione dello stato di provenienza | La migliore ipotesi di Marketo (basata su IP) sullo stato o la regione della persona |
| Codice postale | La migliore ipotesi di Marketo (basata su IP) del codice postale della persona |
| Paese di provenienza | La migliore ipotesi di Marketo (basata su IP) del paese della persona |
| Area metropolitana | La migliore ipotesi di Marketo (basata su IP) sull&#39;area metropolitana della persona |
| Codice area telefono | La migliore ipotesi di Marketo (basata su IP) sul codice di area della persona |

## Valori possibili per il tipo di origine originale e di registrazione {#possible-values-for-original-and-registration-source-type}

Sotto ci sono alcuni valori possibili e ciò che significano.

| **Tipo origine originale** | **Definizione** |
|---|---|
| Salesforce.com | Persona rilevata da una sincronizzazione Salesforce |
| Visite pagina Web | Persona scoperta da una pagina Web |
| Compilazione modulo Web | La persona è stata scoperta dopo la compilazione di un modulo |
| Importa elenco | Persona scoperta da un&#39;importazione di elenco |
| Nuova persona | La persona è stata inserita manualmente nel database |
| Clic collegamento web | Persona scoperta dopo aver fatto clic su un collegamento |
| E-mail di vendita | Alla persona è stato inviato un messaggio e-mail tramite il componente aggiuntivo e-mail di Sales Insight |
| Person | La persona è stata sincronizzata da Salesforce come persona |
| Contatto | La persona è stata sincronizzata da Salesforce come contatto |
| API Munchkin | Persona scoperta dall&#39;API Munchkin di Marketo |
| App Social | La persona è stata scoperta da un widget social |
| API Servizio Web | Persona scoperta da un&#39;API di servizio Web |
| Partner evento | Persona scoperta tramite un servizio webinar sincronizzato |
| Associa lead | Persona unita tramite la chiamata API Lead associata |

| **Tipo origine registrazione** | **Definizione** |
|---|---|
| Importa elenco | Diventare una persona attraverso un&#39;importazione di elenco |
| Salesforce.com | Diventa una persona tramite una sincronizzazione Salesforce |
| Compilazione modulo Web | Diventare una persona dopo aver compilato un modulo |
| E-mail di vendita | Alla persona è stato inviato un messaggio e-mail tramite il componente aggiuntivo e-mail di Sales Insight |
| API Servizio Web | La persona è stata creata tramite SOAP/REST API |
| Nuova persona | La persona è stata inserita manualmente nel database |
| API Munchkin | È diventata una persona tramite l&#39;API Munchkin di Marketo |
| App Social | Diventare una persona attraverso un widget social |
| Partner evento | Diventare una persona tramite un servizio webinar collegato |

