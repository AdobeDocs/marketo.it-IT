---
description: Mappatura campo Veeva predefinita - Documentazione Marketo - Documentazione del prodotto
title: Mappatura campo Veeva predefinita
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 33%

---

# Mappatura campo Veeva predefinita {#default-veeva-field-mapping}

Quando sincronizzi inizialmente l’account di Marketo Engage con Veeva, Marketo crea automaticamente queste associazioni tra i campi incorporati di Veeva e Marketo. Marketo sincronizzerà inoltre i campi personalizzati sugli account e sui contatti.

## Campi contatto {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Campo SFDC</th>
      <th>Campo Marketo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Data di nascita</td>
      <td>Data di nascita</td>
    </tr>
    <tr>
      <td>Data di creazione</td>
      <td>Data di creazione SFDC</td>
    </tr>
    <tr>
      <td>Descrizione contatto</td>
      <td>Note della persona</td>
    </tr>
    <tr>
      <td>E-mail</td>
      <td>Indirizzo e-mail</td>
    </tr>
    <tr>
      <td>Fax ufficio</td>
      <td>Numero di fax</td>
    </tr>
    <tr>
      <td>Nome</td>
      <td>Nome</td>
    </tr>
    <tr>
      <td>Rinuncia e-mail</td>
      <td>Annulla l'iscrizione</td>
    </tr>
    <tr>
      <td>Eliminato</td>
      <td>SFDC è stato eliminato</td>
    </tr>
    <tr>
      <td>Cognome</td>
      <td>Cognome</td>
    </tr>
    <tr>
      <td>Fonte lead</td>
      <td>Origine</td>
    </tr>
    <tr>
      <td>Punteggio lead</td>
      <td>Punteggio</td>
    </tr>
    <tr>
      <td>MailingCity</td>
      <td>Città</td>
    </tr>
    <tr>
      <td>MailingCountry</td>
      <td>Paese</td>
    </tr>
    <tr>
      <td>CodicePostaleMailing</td>
      <td>Codice postale</td>
    </tr>
    <tr>
      <td>MailingState</td>
      <td>Stato</td>
    </tr>
    <tr>
      <td>MailingStreet</td>
      <td>Indirizzo</td>
    </tr>
    <tr>
      <td>Telefono cellulare</td>
      <td>Numero di telefono</td>
    </tr>
    <tr>
      <td>Telefono (uff.)</td>
      <td>Numero di telefono</td>
    </tr>
    <tr>
      <td>Formula di saluto</td>
      <td>Formula di saluto</td>
    </tr>
    <tr>
      <td>Titolo</td>
      <td>Qualifica</td>
    </tr>
  </tbody>
</table>

## Campi account {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Campo SFDC</th>
      <th>Campo Marketo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Entrata annuale</td>
      <td>Entrata annuale</td>
    </tr>
    <tr>
      <td>Città di fatturazione</td>
      <td>Città di fatturazione</td>
    </tr>
    <tr>
      <td>Paese di fatturazione</td>
      <td>Paese di fatturazione</td>
    </tr>
    <tr>
      <td>CAP fatturazione</td>
      <td>Codice postale di fatturazione</td>
    </tr>
    <tr>
      <td>Provincia di fatturazione</td>
      <td>Stato di fatturazione</td>
    </tr>
    <tr>
      <td>Via di fatturazione</td>
      <td>Indirizzo di fatturazione</td>
    </tr>
    <tr>
      <td>Descrizione account</td>
      <td>Note società</td>
    </tr>
    <tr>
      <td>Settore</td>
      <td>Settore</td>
    </tr>
    <tr>
      <td>Eliminato</td>
      <td>SFDC è stato eliminato</td>
    </tr>
    <tr>
      <td>Nome account</td>
      <td>Nome azienda</td>
    </tr>
    <tr>
      <td>Dipendenti</td>
      <td>Numero dipendenti</td>
    </tr>
    <tr>
      <td>Telefono account</td>
      <td>Numero di telefono</td>
    </tr>
    <tr>
      <td>Codice SIC (Standard Industrial Classification)</td>
      <td>Codice SIC (Standard Industrial Classification)</td>
    </tr>
    <tr>
      <td>Sito dell’account</td>
      <td>Sito</td>
    </tr>
    <tr>
      <td>Tipo di account</td>
      <td>Tipo SFDC</td>
    </tr>
    <tr>
      <td>Sito web</td>
      <td>Sito web</td>
    </tr>
  </tbody>
</table>

## Campi di sistema correlati a Veeva in Marketo (sola lettura) {#veeva-related-system-fields-in-marketo}

Questi campi vengono creati in Marketo ma non possono essere regolati dai clienti.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Campo</th>
      <th>Descrizione</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>ID Veeva</td>
      <td>ID Salesforce di 18 caratteri</td>
    </tr>
    <tr>
      <td>Tipo Veeva</td>
      <td>Contatto. Se vuoto, il lead esiste solo come persona in Marketo</td>
    </tr>
    <tr>
      <td>Data creazione Veeva</td>
      <td>Data di creazione in SFDC (può essere diversa da Creato in Marketo)</td>
    </tr>
    <tr>
      <td>Veeva è eliminato</td>
      <td>La persona era in SFDC ma è stata eliminata e ora risiede solo in Marketo</td>
    </tr>
  </tbody>
</table>
