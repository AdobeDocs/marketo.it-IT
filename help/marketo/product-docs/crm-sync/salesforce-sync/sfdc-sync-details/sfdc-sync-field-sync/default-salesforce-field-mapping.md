---
unique-page-id: 4719314
description: Mappatura campo Salesforce predefinita - Documenti Marketo - Documentazione prodotto
title: Mapping campo Salesforce predefinito
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# Mapping campo Salesforce predefinito {#default-salesforce-field-mapping}

Quando sincronizzate inizialmente l’account Marketo con Salesforce, Marketo crea automaticamente queste associazioni tra i campi Salesforce e Marketo incorporati. Marketo sincronizzerà anche i campi personalizzati su Lead, Account, Opportunità e Contatti.

## Campi lead {#lead-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Entrate annuali | Entrate annuali |
| Città | Città |
| Azienda | Nome società |
| Data di conversione | Data di conversione SFDC |
| Paese | Paese |
| Data di creazione | Data creazione SFDC |
| Descrizione | Note sulla persona |
| E-mail | Indirizzo e-mail |
| Fax | Numero fax |
| Nome | Nome |
| Rifiuto e-mail | Annulla sottoscrizione |
| Industria | Industria |
| Convertito | SFDC Convertito |
| Eliminato | SFDC eliminato |
| Cognome | Cognome |
| Origine lead | Origine |
| Punteggio lead | Punteggio |
| Cellulare | Numero di telefono cellulare |
| Dipendenti | Num Dipendenti |
| Telefono | Numero di telefono |
| CAP | Codice postale |
| Valutazione | Valutazione |
| Saluto | Saluto |
| Provincia | Stato |
| Stato | Stato |
| Via | Indirizzo |
| Titolo | Titolo processo |
| Sito Web | Sito Web |

## Campi contatto {#contact-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Data di nascita | Data di nascita |
| Data di creazione | Data creazione SFDC |
| Descrizione contatto | Note sulla persona |
| E-mail | Indirizzo e-mail |
| Fax ufficio | Numero fax |
| Nome | Nome |
| Rifiuto e-mail | Annulla sottoscrizione |
| Eliminato | SFDC eliminato |
| Cognome | Cognome |
| Origine lead | Origine |
| Punteggio lead | Punteggio |
| MailingCity | Città |
| MailingCountry | Paese |
| MailingPostalCode | Codice postale |
| MailingState | Stato |
| MailingStreet | Indirizzo |
| Cellulare | Numero di telefono cellulare |
| Business Phone | Numero di telefono |
| Saluto | Saluto |
| Titolo | Titolo processo |

## Campi account {#account-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Entrate annuali | Entrate annuali |
| Città di fatturazione | Città di fatturazione |
| Paese di fatturazione | Paese di fatturazione |
| Codice postale di fatturazione | Codice postale fatturazione |
| Provincia di fatturazione | Stato fatturazione |
| Via di fatturazione | Indirizzo di fatturazione |
| Descrizione account | Note sulla società |
| Industria | Industria |
| Eliminato | SFDC eliminato |
| Nome account | Nome società |
| Dipendenti | Num Dipendenti |
| Telefono account | Telefono principale |
| Codice SIC | Codice SIC |
| Sito account | Sito |
| Tipo di account | Tipo SFDC |
| Sito Web | Sito Web |

## Campi di sistema correlati a Salesforce in Marketo (sola lettura) {#salesforce-related-system-fields-in-marketo-read-only}

Questi campi vengono creati in Marketo ma non possono essere modificati dai clienti.

| Field | Descrizione |
|---|---|
| ID SFDC | ID Salesforce a 18 caratteri |
| Tipo SFDC | Lead o Contatto. Se vuoto, il lead esiste solo come persona in Marketo |
| Data creazione SFDC | Data di creazione in SFDC (può essere diversa da Data di creazione in Marketo) |
| SFDC eliminato | Una volta la persona era nella DSC ma era stata eliminata e ora vive solo a Marketo |
