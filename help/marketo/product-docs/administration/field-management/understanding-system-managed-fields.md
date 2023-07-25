---
unique-page-id: 5472615
description: Informazioni sui campi gestiti dal sistema - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sui campi gestiti dal sistema
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 8%

---

# Informazioni sui campi gestiti dal sistema {#understanding-system-managed-fields}

Potresti aver notato che il [pagina dettagli persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} dispone di una serie di campi non modificabili creati da Marketo. Questi dati provengono da varie fonti, e ci sono innumerevoli valori che potrebbero essere visualizzati.

## Tipi di campi {#field-types}

| **Nome campo** | **Definizione** |
|---|---|
| Tipo di sorgente originale | La posizione in cui una persona o un visitatore del sito Web è stato individuato per la prima volta (esempio: importazione elenco, visita pagina Web) |
| Informazioni sorgente originali | Informazioni specifiche sulla posizione (esempio: nome dell’elenco, URL della pagina web) |
| Motore di ricerca originale | Se del caso, il motore di ricerca che ha rinviato la persona alla fonte di ingresso originale |
| Frase di ricerca originale | Se applicabile, il termine di ricerca utilizzato che ha rinviato la persona alla sorgente di ingresso originale |
| Destinatario che inoltra originale | URL che ha ospitato l&#39;origine della voce originale |
| Tipo di origine registrazione | La posizione in cui un’attività è diventata per la prima volta una persona (esempio: importazione di elenchi, visita di pagine web) |
| Info origine registrazione | Informazioni specifiche sulla posizione (esempio: nome dell’elenco, URL della pagina web) |
| IP anonimo | Indica l&#39;indirizzo IP di una persona |
| Azienda dedotta | Migliore stima di Marketo (basata su IP) dell’azienda della persona |
| Città dedotta | Migliore stima di Marketo (basata su IP) della città della persona |
| Area geografica dello stato dedotta | Migliore stima di Marketo (basata su IP) dello stato o dell’area geografica della persona |
| Codice postale dedotto | Migliore stima di Marketo (basata su IP) del codice postale della persona |
| Paese dedotto | Migliore stima di Marketo (basata su IP) del paese della persona |
| Area metropolitana dedotta | L&#39;ipotesi migliore di Marketo (basata su IP) dell&#39;area metropolitana della persona |
| Prefisso telefonico dedotto | Migliore stima di Marketo (basata su IP) dell’indicativo di località della persona |

## Valori possibili per Origine e Tipo di origine registrazione {#possible-values-for-original-and-registration-source-type}

Di seguito sono riportati alcuni valori possibili e il loro significato.

| **Tipo di sorgente originale** | **Definizione** |
|---|---|
| Salesforce.com | Persona scoperta da un [!DNL Webhook] sincronizzazione |
| Visite alle pagine web | La persona è stata scoperta da una pagina web |
| Compilazione modulo web | La persona è stata scoperta dopo la compilazione di un modulo |
| Importazione elenco | Persona scoperta da un’importazione elenco |
| Nuova persona | La persona è stata inserita manualmente nel database |
| Clic collegamento web | La persona è stata scoperta dopo aver fatto clic su un collegamento |
| E-mail vendita | Alla persona è stata inviata un’e-mail tramite [!DNL Sales Insight] Componente aggiuntivo e-mail |
| Persona | La persona è stata sincronizzata da [!DNL Salesforce] come persona |
| Contatto | La persona è stata sincronizzata da [!DNL Webhook] come contatto |
| [!DNL Munchkin] API | Persona scoperta dal Marketo Engage [!DNL Munchkin] API |
| App social | La persona è stata scoperta da un widget sociale |
| API servizio Web | La persona è stata rilevata da un’API del servizio web |
| Partner evento | La persona è stata scoperta tramite un servizio di webinar sincronizzato |
| Associa lead | Persona unita tramite chiamata API del lead associato |

| **Tipo di origine registrazione** | **Definizione** |
|---|---|
| Importazione elenco | Diventare una persona tramite un’importazione di elenchi |
| Salesforce.com | È diventata una persona tramite un [!DNL Webhook] sincronizzazione |
| Compilazione modulo web | Diventare una persona dopo la compilazione di un modulo |
| E-mail vendita | Alla persona è stata inviata un’e-mail tramite [!DNL Webhook] Componente aggiuntivo e-mail |
| API servizio Web | La persona è stata creata tramite API SOAP/REST |
| Nuova persona | La persona è stata inserita manualmente nel database |
| [!DNL Munchkin] API | È diventata una persona grazie a Marketo [!DNL Munchkin] API |
| App social | Diventare una persona tramite un widget sociale |
| Partner evento | Diventare una persona tramite un servizio di webinar collegato |
