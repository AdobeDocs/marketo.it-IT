---
description: Mappatura predefinita dei campi di Dynamics - Documenti Marketo - Documentazione del prodotto
title: Mappatura predefinita dei campi di Dynamics
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
source-git-commit: d87809e12f153d025f8d013ea52e06c0b6530154
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 13%

---

# Mappatura predefinita dei campi di Dynamics {#default-dynamics-field-mapping}

Quando si sincronizza inizialmente l’account Marketo con Microsoft, Marketo crea automaticamente queste associazioni tra i campi incorporati di Dynamics e Marketo.  Marketo sincronizzerà anche i campi personalizzati sui lead, account, opportunità e contatti.

## Campi lead {#lead-fields}

<table>
  <colgroup>
    <col>
    <col>
    <col>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo Marketo</th>
      <th>Campo MS Dynamics</th>
      <th>Nome API di MS Dynamics</th>
    </tr>
    <tr>
      <td>Data creazione Microsoft</td>
      <td>Creato il</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>Formula di saluto</td>
      <td>Formula di saluto</td>
      <td>saluto</td>
    </tr>
    <tr>
      <td>Primo</td>
      <td>Nome</td>
      <td>nome</td>
    </tr>
    <tr>
      <td>Medio</td>
      <td>Secondo nome</td>
      <td>nomeintermedio</td>
    </tr>
    <tr>
      <td>Ultimo</td>
      <td>Cognome</td>
      <td>cognome</td>
    </tr>
    <tr>
      <td>E-mail</td>
      <td>E-mail</td>
      <td>indirizzo e-mail1</td>
    </tr>
    <tr>
      <td>Professione</td>
      <td>Titolo del processo</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>Telefono</td>
      <td>Telefono ufficio</td>
      <td>telefono1</td>
    </tr>
    <tr>
      <td>Mobile</td>
      <td>Telefono cellulare</td>
      <td>cellulare</td>
    </tr>
    <tr>
      <td>Fax</td>
      <td>Fax</td>
      <td>fax</td>
    </tr>
    <tr>
      <td>Indirizzo</td>
      <td>Via 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Città</td>
      <td>Città</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Stato</td>
      <td>Provincia</td>
      <td>address1_stateorprovince</td>
    </tr>
    <tr>
      <td>Paese</td>
      <td>Paese/Regione</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Codice postale</td>
      <td>Codice postale</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Origine persona</td>
      <td>Fonte Lead</td>
      <td>leadsourcecode</td>
    </tr>
    <tr>
      <td>Stato persona</td>
      <td>Stato</td>
      <td>codice di stato</td>
    </tr>
    <tr>
      <td>Motivo dello stato</td>
      <td>Motivo dello stato</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>Note sulla persona</td>
      <td>Descrizione</td>
      <td>descrizione</td>
    </tr>
    <tr>
      <td>Non effettuare la chiamata</td>
      <td>Non consentire chiamate telefoniche</td>
      <td>telefonino</td>
    </tr>
    <tr>
      <td>Annulla l'iscrizione</td>
      <td>Non inviare e-mail in blocco</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Valutazione persona</td>
      <td>Valutazione</td>
      <td>leadqualitycode</td>
    </tr>
    <tr>
      <td>Indirizzo Microsoft 2</td>
      <td>Via 2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Indirizzo Microsoft 3</td>
      <td>Via 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Microsoft non invia e-mail</td>
      <td>Non consentire e-mail</td>
      <td>donotemale</td>
    </tr>
    <tr>
      <td>Microsoft Non Fax</td>
      <td>Non Consentire I Fax</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Microsoft Non Invia Materiale Di Marketing</td>
      <td>Materiale di marketing</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>Telefono abitazione Microsoft</td>
      <td>Telefono abitazione</td>
      <td>telefono2</td>
    </tr>
    <tr>
      <td>Metodo Di Contatto Preferito Di Microsoft</td>
      <td>Metodo di contatto preferito</td>
      <td>preferredcontactmetodcode</td>
    </tr>
    <tr>
      <td>Argomento Microsoft</td>
      <td>Argomento</td>
      <td>soggetto</td>
    </tr>
    <tr>
      <td>Data ultimo momento interessante</td>
      <td>Data ultimo momento interessante</td>
      <td>mkt_lastinteressante_momentingdate</td>
    </tr>
    <tr>
      <td>Ultimo interessante desc momento</td>
      <td>Ultimo interessante desc momento</td>
      <td>mkt_lastinteressante ingmomentdesc</td>
    </tr>
    <tr>
      <td>Ultima fonte di momento interessante</td>
      <td>Ultima fonte di momento interessante</td>
      <td>mkt_leadinteressante momentingsource</td>
    </tr>
    <tr>
      <td>Ultimo tipo di momento interessante</td>
      <td>Ultimo tipo di momento interessante</td>
      <td>mkt_lastinteressantemomenttype</td>
    </tr>
    <tr>
      <td>Azienda</td>
      <td>Nome dell'azienda</td>
      <td>nome azienda</td>
    </tr>
    <tr>
      <td>Punteggio relativo</td>
      <td>Punteggio relativo</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>Priorità</td>
      <td>Priorità</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Urgenza relativa</td>
      <td>urgenza</td>
      <td>mkt_urgy</td>
    </tr>
    <tr>
      <td>Oggetto</td>
      <td>Argomento</td>
      <td>soggetto</td>
    </tr>
    <tr>
      <td>Entrata annuale</td>
      <td>Entrata annuale</td>
      <td>entrate</td>
    </tr>
  </tbody>
</table>

I campi Lead riportati di seguito sono sincronizzati per uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo MS Dynamics</th>
      <th>Nome API di MS Dynamics</th>
    </tr>
    <tr>
      <td>Proprietario </td>
      <td>proprietario</td>
    </tr>
    <tr>
      <td>creato il</td>
      <td>createdon</td>
    </tr>
  </tbody>
</table>

## Campi contatto {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo Marketo</th>
      <th>Campo MS Dynamics</th>
      <th>Nome API di MS Dynamics</th>
    </tr>
    <tr>
      <td>Data creazione Microsoft</td>
      <td>Creato il</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>Formula di saluto</td>
      <td>Formula di saluto</td>
      <td>saluto</td>
    </tr>
    <tr>
      <td>Primo</td>
      <td>Nome</td>
      <td>nome</td>
    </tr>
    <tr>
      <td>Medio</td>
      <td>Secondo nome</td>
      <td>nomeintermedio</td>
    </tr>
    <tr>
      <td>Ultimo</td>
      <td>Cognome</td>
      <td>cognome</td>
    </tr>
    <tr>
      <td>E-mail</td>
      <td>E-mail</td>
      <td>indirizzo e-mail1</td>
    </tr>
    <tr>
      <td>Professione</td>
      <td>Professione</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>Telefono</td>
      <td>Telefono ufficio</td>
      <td>telefono1</td>
    </tr>
    <tr>
      <td>Mobile</td>
      <td>Telefono cellulare</td>
      <td>cellulare</td>
    </tr>
    <tr>
      <td>Indirizzo</td>
      <td>Indirizzo 1: Via 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Città</td>
      <td>Indirizzo 1: Città</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Stato</td>
      <td>Indirizzo 1: Provincia</td>
      <td>address1_stateorprovince</td>
    </tr>
    <tr>
      <td>Paese</td>
      <td>Indirizzo 1: Paese/Regione</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Codice postale</td>
      <td>Indirizzo 1: Codice postale</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Stato persona</td>
      <td>Stato</td>
      <td>codice di stato</td>
    </tr>
    <tr>
      <td>Motivo dello stato</td>
      <td>Motivo dello stato</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>Non effettuare la chiamata</td>
      <td>Non consentire chiamate telefoniche</td>
      <td>telefonino</td>
    </tr>
    <tr>
      <td>Annulla l'iscrizione</td>
      <td>Non inviare e-mail in blocco</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Indirizzo Microsoft 2</td>
      <td>Indirizzo 1: Via 2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Indirizzo Microsoft 3</td>
      <td>Indirizzo 1: Via 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Microsoft non invia e-mail</td>
      <td>Non consentire e-mail</td>
      <td>donotemale</td>
    </tr>
    <tr>
      <td>Telefono abitazione Microsoft</td>
      <td>Telefono abitazione</td>
      <td>telefono2</td>
    </tr>
    <tr>
      <td>Metodo Di Contatto Preferito Di Microsoft</td>
      <td>Metodo Di Contatto Preferito</td>
      <td>preferredcontactmetodcode</td>
    </tr>
    <tr>
      <td>Data ultimo momento interessante</td>
      <td>Data ultimo momento interessante</td>
      <td>mkt_lastinteressante_momentingdate</td>
    </tr>
    <tr>
      <td>Ultimo tipo di momento interessante</td>
      <td>Ultimo tipo di momento interessante</td>
      <td>mkt_lastinteressantemomenttype</td>
    </tr>
    <tr>
      <td>Ultima fonte di momento interessante</td>
      <td>Ultima fonte di momento interessante</td>
      <td>mkt_leadinteressante momentingsource</td>
    </tr>
    <tr>
      <td>Ultimo interessante desc momento</td>
      <td>Ultimo interessante desc momento</td>
      <td>mkt_lastinteressante ingmomentdesc</td>
    </tr>
    <tr>
      <td>Microsoft Non Invia Materiale Di Marketing</td>
      <td>Materiale di marketing</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>Microsoft Non Fax</td>
      <td>Microsoft Non Fax</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Priorità</td>
      <td>Priorità</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Urgenza relativa</td>
      <td>urgenza</td>
      <td>mkt_urgy</td>
    </tr>
    <tr>
      <td>Punteggio relativo</td>
      <td>Punteggio relativo</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>Note sulla persona</td>
      <td>Descrizione</td>
      <td>descrizione </td>
    </tr>
    <tr>
      <td>Punteggio persona</td>
      <td>Punteggio Lead</td>
      <td>mkt_leadscore</td>
    </tr>
    <tr>
      <td>Note sulla persona</td>
      <td>Descrizione</td>
      <td>descrizione </td>
    </tr>
  </tbody>
</table>

I campi Contatto riportati di seguito sono sincronizzati per uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo MS Dynamics</th>
      <th>Nome API di MS Dynamics</th>
    </tr>
    <tr>
      <td>Proprietario </td>
      <td>proprietario</td>
    </tr>
    <tr>
      <td>creato il</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>gencustomerid</td>
      <td>Nome dell'azienda</td>
    </tr>
  </tbody>
</table>

## Campi account {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo Marketo</th>
      <th>Campo MS Dynamics</th>
      <th>Nome API di MS Dynamics</th>
    </tr>
    <tr>
      <td>Conto (a)</td>
      <td>Account</td>
      <td>contabile</td>
    </tr>
    <tr>
      <td>Indirizzo di fatturazione</td>
      <td>Indirizzo 1: Via 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Città di fatturazione</td>
      <td>Indirizzo 1: Città</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Paese di fatturazione</td>
      <td>Indirizzo 1: Paese/Regione</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Codice postale di fatturazione</td>
      <td>Indirizzo 1: Codice postale</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Indirizzo di fatturazione Microsoft 2</td>
      <td>Indirizzo 1: Via 2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Indirizzo di fatturazione Microsoft 3</td>
      <td>Indirizzo 1: Via 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Numero di telefono</td>
      <td>Numero di telefono</td>
      <td>telefono1</td>
    </tr>
    <tr>
      <td>Tipo di business</td>
      <td>Tipo di business</td>
      <td>codice di fabbrica</td>
    </tr>
    <tr>
      <td>Numero account Microsoft</td>
      <td>Numero di conto</td>
      <td>numero contabile</td>
    </tr>
    <tr>
      <td>Stato dell'azienda Microsoft</td>
      <td>Stato</td>
      <td>codice di stato</td>
    </tr>
    <tr>
      <td>Entrata annuale</td>
      <td>Entrata annuale</td>
      <td>entrate</td>
    </tr>
    <tr>
      <td>Note aziendali</td>
      <td>Descrizione</td>
      <td>descrizione</td>
    </tr>
    <tr>
      <td>Settore</td>
      <td>Settore</td>
      <td>industrycode</td>
    </tr>
    <tr>
      <td>Codice SIC (Standard Industrial Classification)</td>
      <td>Codice SIC (Standard Industrial Classification)</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Sito web</td>
      <td>Sito web</td>
      <td>sito web</td>
    </tr>
    <tr>
      <td>Numero dipendenti</td>
      <td>Numero di dipendenti</td>
      <td>numberofdipendenti</td>
    </tr>
    <tr>
      <td>Codice SIC (Standard Industrial Classification)</td>
      <td>Codice SIC (Standard Industrial Classification)</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Azienda</td>
      <td>name</td>
      <td>Nome account</td>
    </tr>
    <tr>
      <td>Numero dipendenti</td>
      <td>Numero di dipendenti</td>
      <td>numberofdipendenti</td>
    </tr>
  </tbody>
</table>

I campi Account di seguito sono sincronizzati per uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo MS Dynamics</th>
      <th>Nome API di MS Dynamics</th>
    </tr>
    <tr>
      <td>Proprietario </td>
      <td>proprietario</td>
    </tr>
    <tr>
      <td>creato il</td>
      <td>createdon</td>
    </tr>
  </tbody>
</table>

## Campi opportunità {#opportunity-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo Marketo</th>
      <th>Campo MS Dynamics</th>
      <th>Nome API di MS Dynamics</th>
    </tr>
    <tr>
      <td>Probabilità di chiusura</td>
      <td>Probabilità</td>
      <td>probabilità di chiusura</td>
    </tr>
    <tr>
      <td>Stage</td>
      <td>status</td>
      <td>codice di stato</td>
    </tr>
    <tr>
      <td>Data di chiusura effettiva</td>
      <td>Data di chiusura effettiva</td>
      <td>attualclosedato</td>
    </tr>
    <tr>
      <td>Nome</td>
      <td>Argomento</td>
      <td>name</td>
    </tr>
    <tr>
      <td>Valore stimato</td>
      <td>Est Entrate</td>
      <td>evaluateValue</td>
    </tr>
    <tr>
      <td>Descrizione</td>
      <td>Descrizione</td>
      <td>descrizione</td>
    </tr>
  </tbody>
</table>

I campi Account di seguito sono sincronizzati per uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo MS Dynamics</th>
      <th>Nome API di MS Dynamics</th>
    </tr>
    <tr>
      <td>Proprietario </td>
      <td>proprietario</td>
    </tr>
    <tr>
      <td>Opportunità</td>
      <td>opportunitàId</td>
    </tr>
    <tr>
      <td>Cliente potenziale</td>
      <td>customerId</td>
    </tr>
  </tbody>
</table>

## Campi di sistema correlati a Microsoft in Marketo (sola lettura) {#microsoft-related-system-fields}

I campi seguenti vengono creati in Marketo ma non possono essere regolati dagli utenti.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo Marketo</th>
      <th>Descrizione</th>
    </tr>
    <tr>
      <td>Tipo Microsoft</td>
      <td>Lead o contatto. Se vuoto, il lead esiste solo come persona in Marketo</td>
    </tr>
    <tr>
      <td>Data creazione Microsoft</td>
      <td>Data di creazione in MS Dynamics (può essere diversa da quella creata in Marketo)</td>
    </tr>
    <tr>
      <td>Microsoft viene eliminato</td>
      <td>Una persona era in Microsoft ma è stata eliminata e ora vive solo in Marketo</td>
    </tr>
  </tbody>
</table>
