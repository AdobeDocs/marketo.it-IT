---
unique-page-id: 4719314
description: Mappatura predefinita del campo Salesforce - Documenti Marketo - Documentazione del prodotto
title: Mapping campo Salesforce predefinito
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 33%

---

# Mapping campo Salesforce predefinito {#default-salesforce-field-mapping}

Quando sincronizzi inizialmente il tuo account Marketo con Salesforce, Marketo crea automaticamente queste associazioni tra i campi Salesforce incorporati e Marketo. Marketo sincronizzerà anche i campi personalizzati sui lead, account, opportunità e contatti.

## Campi lead {#lead-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Entrata annuale | Entrata annuale |
| Città | Città |
| Azienda | Nome dell&#39;azienda |
| Data conversione | Data conversione SFDC |
| Paese | Paese |
| Data creazione | Data creazione SFDC |
| Descrizione | Note sulla persona |
| E-mail | Indirizzo e-mail |
| Fax | Numero di fax |
| Nome | Nome |
| Rifiuto e-mail | Annulla l&#39;iscrizione |
| Settore | Settore |
| Convertito | SFDC viene convertito |
| Eliminato | SFDC È Eliminato |
| Cognome | Cognome |
| Fonte Lead | Fonte |
| Punteggio Lead | Punteggio |
| Telefono cellulare | Numero di cellulare |
| Dipendenti | Numero dipendenti |
| Telefono | Numero di telefono |
| Codice postale | Codice postale |
| Valutazione | Valutazione |
| Formula di saluto | Formula di saluto |
| Provincia | Stato |
| Stato | Stato |
| Via | Indirizzo |
| Titolo | Professione |
| Sito web | Sito web |

## Campi di contatto {#contact-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Data di nascita | Data di nascita |
| Data creazione | Data creazione SFDC |
| Descrizione contatto | Note sulla persona |
| E-mail | Indirizzo e-mail |
| Fax ufficio | Numero di fax |
| Nome | Nome |
| Rifiuto e-mail | Annulla l&#39;iscrizione |
| Eliminato | SFDC È Eliminato |
| Cognome | Cognome |
| Fonte Lead | Fonte |
| Punteggio Lead | Punteggio |
| MailingCity | Città |
| MailingCountry | Paese |
| Codice postale | Codice postale |
| MailingState | Stato |
| MailingStreet | Indirizzo |
| Telefono cellulare | Numero di cellulare |
| Telefono ufficio | Numero di telefono |
| Formula di saluto | Formula di saluto |
| Titolo | Professione |

## Campi account {#account-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Entrata annuale | Entrata annuale |
| Città di fatturazione | Città di fatturazione |
| Paese di fatturazione | Paese di fatturazione |
| Codice postale/CAP di fatturazione | Codice postale di fatturazione |
| Provincia di fatturazione | Stato di fatturazione |
| Billing Street | Indirizzo di fatturazione |
| Descrizione account | Note aziendali |
| Settore | Settore |
| Eliminato | SFDC È Eliminato |
| Nome account | Nome dell&#39;azienda |
| Dipendenti | Numero dipendenti |
| Telefono account | Numero di telefono |
| Codice SIC (Standard Industrial Classification) | Codice SIC (Standard Industrial Classification) |
| Sito dell&#39;account | Sito |
| Tipo di conto | Tipo SFDC |
| Sito web | Sito web |

## Campi di sistema correlati a Salesforce in Marketo (sola lettura) {#salesforce-related-system-fields-in-marketo-read-only}

Questi campi vengono creati in Marketo ma non possono essere regolati dai clienti.

| Campo | Descrizione |
|---|---|
| ID SFDC | ID Salesforce a 18 caratteri |
| Tipo SFDC | Lead o contatto. Se vuoto, il lead esiste solo come persona in Marketo |
| Data creazione SFDC | Data di creazione in SFDC (può essere diversa da Creata in Marketo) |
| SFDC eliminato | Una persona era in SFDC ma è stata cancellata e ora vive solo in Marketo |
