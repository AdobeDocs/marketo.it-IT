---
unique-page-id: 4719314
description: Mappatura dei campi Salesforce predefinita - Documenti Marketo - Documentazione del prodotto
title: Mappatura campo Salesforce predefinita
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 43%

---

# Mappatura campo Salesforce predefinita {#default-salesforce-field-mapping}

Quando sincronizzi inizialmente l’account Marketo con Salesforce, Marketo crea automaticamente queste associazioni tra i campi Salesforce e Marketo incorporati. Marketo sincronizzerà inoltre i campi personalizzati sui lead, gli account, le opportunità e i contatti.

## Campi lead {#lead-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Entrata annuale | Entrata annuale |
| Città | Città |
| Azienda | Nome azienda |
| Data di conversione | Data di conversione SFDC |
| Paese | Paese |
| Data di creazione | Data di creazione SFDC |
| Descrizione | Note della persona |
| E-mail | Indirizzo e-mail |
| Fax | Numero di fax |
| Nome | Nome |
| Rinuncia e-mail | Annulla l&#39;iscrizione |
| Settore | Settore |
| Convertito | SFDC è stato convertito |
| Eliminato | SFDC è stato eliminato |
| Cognome | Cognome |
| Fonte lead | Origine |
| Punteggio lead | Punteggio |
| Telefono cellulare | Numero di telefono |
| Dipendenti | Numero dipendenti |
| Telefono | Numero di telefono |
| CAP | Codice postale |
| Valutazione | Valutazione |
| Formula di saluto | Formula di saluto |
| Stato/Provincia | Stato |
| Stato | Stato |
| Via | Indirizzo |
| Titolo | Qualifica |
| Sito web | Sito web |

## Campi contatto {#contact-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Data di nascita | Data di nascita |
| Data di creazione | Data di creazione SFDC |
| Descrizione contatto | Note della persona |
| E-mail | Indirizzo e-mail |
| Fax ufficio | Numero di fax |
| Nome | Nome |
| Rinuncia e-mail | Annulla l&#39;iscrizione |
| Eliminato | SFDC è stato eliminato |
| Cognome | Cognome |
| Fonte lead | Origine |
| Punteggio lead | Punteggio |
| MailingCity | Città |
| MailingCountry | Paese |
| CodicePostaleMailing | Codice postale |
| MailingState | Stato |
| MailingStreet | Indirizzo |
| Telefono cellulare | Numero di telefono |
| Telefono (uff.) | Numero di telefono |
| Formula di saluto | Formula di saluto |
| Titolo | Qualifica |

## Campi account {#account-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Entrata annuale | Entrata annuale |
| Città di fatturazione | Città di fatturazione |
| Paese di fatturazione | Paese di fatturazione |
| CAP fatturazione | Codice postale di fatturazione |
| Provincia di fatturazione | Stato di fatturazione |
| Via di fatturazione | Indirizzo di fatturazione |
| Descrizione account | Note società |
| Settore | Settore |
| Eliminato | SFDC è stato eliminato |
| Nome account | Nome azienda |
| Dipendenti | Numero dipendenti |
| Telefono account | Numero di telefono |
| Codice SIC (Standard Industrial Classification) | Codice SIC (Standard Industrial Classification) |
| Sito dell’account | Sito |
| Tipo di account | Tipo SFDC |
| Sito web | Sito web |

## Campi di sistema correlati a Salesforce in Marketo (sola lettura) {#salesforce-related-system-fields-in-marketo-read-only}

Questi campi vengono creati in Marketo ma non possono essere regolati dai clienti.

| Campo | Descrizione |
|---|---|
| ID SFDC | ID Salesforce di 18 caratteri |
| Tipo SFDC | Lead o contatto. Se vuoto, il lead esiste solo come persona in Marketo |
| Data di creazione SFDC | Data di creazione in SFDC (può essere diversa da Creato in Marketo) |
| SFDC eliminato | La persona era in SFDC ma è stata eliminata e ora risiede solo in Marketo |
