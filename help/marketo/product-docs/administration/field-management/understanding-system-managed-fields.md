---
unique-page-id: 5472615
description: Informazioni sui campi gestiti del sistema - Documenti Marketo - Documentazione del prodotto
title: Informazioni sui campi gestiti del sistema
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---

# Informazioni sui campi gestiti del sistema {#understanding-system-managed-fields}

Potresti aver notato che la [pagina di dettaglio della persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) presenta una serie di campi non modificabili creati da Marketo. Questi dati provengono da varie fonti, e ci sono innumerevoli valori che possono essere visualizzati.

## Tipi di campi {#field-types}

| **Nome campo** | **Definizione** |
|---|---|
| Tipo di origine originale | La posizione di una persona o di un visitatore del sito web è stata scoperta per la prima volta (Esempio: Importazione elenco, Visita pagina web) |
| Informazioni origine originali | Specifiche relative a tale posizione (Esempio: Nome dell’elenco, URL della pagina web) |
| Motore di ricerca originale | Se del caso, il motore di ricerca che ha indirizzato la persona alla fonte di ingresso originale |
| Frase di ricerca originale | Se del caso, il termine utilizzato per la ricerca che ha fatto riferimento alla persona alla fonte di ingresso originale |
| Referrer originale | URL in cui è ospitata la sorgente di ingresso originale |
| Tipo di origine registrazione | La posizione in cui un’attività è diventata per la prima volta una persona (esempio: Importazione elenco, Visita pagina web) |
| Informazioni origine registrazione | Specifiche relative a tale posizione (Esempio: Nome dell’elenco, URL della pagina web) |
| IP anonimo | Indica l’indirizzo IP di una persona |
| Azienda in oggetto | Indovina migliore (basata su IP) Marketo dell&#39;azienda della persona |
| Città di riferimento | Migliore stima (basata su IP) della città della persona su Marketo |
| Regione dello Stato di provenienza | Migliore stima (basata su IP) dello stato o della regione della persona in Marketo |
| Codice postale trasferito | Migliore stima (basata su IP) del codice postale della persona in Marketo |
| Paese in oggetto | Migliore stima Marketo (basata su IP) del paese della persona |
| Area metropolitana | Indovina migliore (basata su IP) Marketo dell&#39;area metropolitana della persona |
| Codice di area del telefono | Migliore stima (basata su IP) del codice di area della persona in Marketo |

## Valori possibili per il tipo di origine originale e di registrazione {#possible-values-for-original-and-registration-source-type}

Di seguito sono riportati alcuni possibili valori e cosa intendono.

| **Tipo di origine originale** | **Definizione** |
|---|---|
| Salesforce.com | La persona è stata scoperta da una sincronizzazione Salesforce |
| Visite a una pagina web | Persona scoperta da una pagina web |
| Compilazione modulo web | Persona scoperta dopo la compilazione di un modulo |
| Importazione elenco | Persona scoperta da un&#39;importazione di elenchi |
| Nuova persona | La persona è stata immessa manualmente nel database |
| Clic su collegamento web | Persona scoperta dopo aver fatto clic su un collegamento |
| E-mail di vendita | Alla persona è stato inviato un messaggio e-mail tramite il componente aggiuntivo e-mail di Sales Insight |
| Persona | La persona è stata sincronizzata da Salesforce come persona |
| Contatto | La persona è stata sincronizzata da Salesforce come contatto |
| API Munchkin | Persona scoperta dall&#39;API Munchkin di Marketo |
| App social | Persona scoperta da un widget social |
| API del servizio Web | Persona rilevata da un&#39;API di servizio Web |
| Partner evento | Persona scoperta tramite un servizio webinar sincronizzato |
| Associa lead | Persona unita tramite chiamata API lead associata |

| **Tipo di origine registrazione** | **Definizione** |
|---|---|
| Importazione elenco | È diventata una persona tramite un’importazione di elenchi |
| Salesforce.com | Diventa una persona tramite una sincronizzazione Salesforce |
| Compilazione modulo web | Diventa una persona dopo aver compilato un modulo |
| E-mail di vendita | Alla persona è stato inviato un messaggio e-mail tramite il componente aggiuntivo e-mail di Sales Insight |
| API del servizio Web | La persona è stata creata tramite API SOAP/REST |
| Nuova persona | La persona è stata immessa manualmente nel database |
| API Munchkin | È diventata una persona tramite l&#39;API Munchkin di Marketo |
| App social | Diventa una persona attraverso un widget social |
| Partner evento | È diventata una persona tramite un servizio webinar collegato |
