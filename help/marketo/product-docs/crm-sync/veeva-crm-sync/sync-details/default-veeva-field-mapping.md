---
description: Mappatura predefinita del campo Veeva - Documenti Marketo - Documentazione del prodotto
title: Mappatura predefinita del campo Veeva
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 27%

---

# Mappatura predefinita del campo Veeva {#default-veeva-field-mapping}

Quando si sincronizza inizialmente l&#39;account di Marketo Engage con Veeva, Marketo crea automaticamente queste associazioni tra i campi Veeva incorporati e Marketo. Marketo sincronizzerà anche i campi personalizzati sui tuoi account e contatti.

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
      <td>Data creazione</td>
      <td>Data creazione SFDC</td>
    </tr>
    <tr>
      <td>Descrizione contatto</td>
      <td>Note sulla persona</td>
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
      <td>Rifiuto e-mail</td>
      <td>Annulla l'iscrizione</td>
    </tr>
    <tr>
      <td>Eliminato</td>
      <td>SFDC È Eliminato</td>
    </tr>
    <tr>
      <td>Cognome</td>
      <td>Cognome</td>
    </tr>
    <tr>
      <td>Fonte Lead</td>
      <td>Fonte</td>
    </tr>
    <tr>
      <td>Punteggio Lead</td>
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
      <td>Codice postale</td>
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
      <td>Numero di cellulare</td>
    </tr>
    <tr>
      <td>Telefono ufficio</td>
      <td>Numero di telefono</td>
    </tr>
    <tr>
      <td>Formula di saluto</td>
      <td>Formula di saluto</td>
    </tr>
    <tr>
      <td>Titolo</td>
      <td>Professione</td>
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
      <td>Codice postale/CAP di fatturazione</td>
      <td>Codice postale di fatturazione</td>
    </tr>
    <tr>
      <td>Provincia di fatturazione</td>
      <td>Stato di fatturazione</td>
    </tr>
    <tr>
      <td>Billing Street</td>
      <td>Indirizzo di fatturazione</td>
    </tr>
    <tr>
      <td>Descrizione account</td>
      <td>Note aziendali</td>
    </tr>
    <tr>
      <td>Settore</td>
      <td>Settore</td>
    </tr>
    <tr>
      <td>Eliminato</td>
      <td>SFDC È Eliminato</td>
    </tr>
    <tr>
      <td>Nome account</td>
      <td>Nome dell'azienda</td>
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
      <td>Sito dell'account</td>
      <td>Sito</td>
    </tr>
    <tr>
      <td>Tipo di conto</td>
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
      <td>Id Veeva</td>
      <td>ID Salesforce a 18 caratteri</td>
    </tr>
    <tr>
      <td>Tipo di Veeva</td>
      <td>Contatta. Se vuoto, il lead esiste solo come persona in Marketo</td>
    </tr>
    <tr>
      <td>Data creazione veeva</td>
      <td>Data di creazione in SFDC (può essere diversa da Creata in Marketo)</td>
    </tr>
    <tr>
      <td>Veeva è soppresso</td>
      <td>Una persona era in SFDC ma è stata cancellata e ora vive solo in Marketo</td>
    </tr>
  </tbody>
</table>
