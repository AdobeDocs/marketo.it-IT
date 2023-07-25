---
description: Mappatura campo Dynamics predefinita - Documenti Marketo - Documentazione del prodotto
title: Mappatura campo Dynamics predefinita
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 18%

---

# Mappatura campo Dynamics predefinita {#default-dynamics-field-mapping}

Quando sincronizzi inizialmente l’account Marketo con Microsoft, Marketo crea automaticamente queste associazioni tra i campi Dynamics e Marketo incorporati.  Marketo sincronizzerà inoltre i campi personalizzati sui lead, gli account, le opportunità e i contatti.

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
      <th>Nome API MS Dynamics</th>
    </tr>
    <tr>
      <td>Data di creazione Microsoft</td>
      <td>Creato il</td>
      <td>creato il</td>
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
      <td>In mezzo</td>
      <td>Secondo nome</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>Ultimo</td>
      <td>Cognome</td>
      <td>cognome</td>
    </tr>
    <tr>
      <td>E-mail</td>
      <td>E-mail</td>
      <td>emailaddress1</td>
    </tr>
    <tr>
      <td>Qualifica</td>
      <td>Qualifica</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>Telefono</td>
      <td>Telefono (uff.)</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>Mobile</td>
      <td>Telefono cellulare</td>
      <td>telefono cellulare</td>
    </tr>
    <tr>
      <td>Fax</td>
      <td>Fax</td>
      <td>fax</td>
    </tr>
    <tr>
      <td>Indirizzo</td>
      <td>Strada 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Città</td>
      <td>Città</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Stato</td>
      <td>Stato/Provincia</td>
      <td>address1_stateorprovince</td>
    </tr>
    <tr>
      <td>Paese</td>
      <td>Paese</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Codice postale</td>
      <td>CAP</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Origine persona</td>
      <td>Fonte lead</td>
      <td>lead sourcecode</td>
    </tr>
    <tr>
      <td>Stato della persona</td>
      <td>Stato</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>Motivo dello stato</td>
      <td>Motivo dello stato</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>Note della persona</td>
      <td>Descrizione</td>
      <td>descrizione</td>
    </tr>
    <tr>
      <td>Non effettuare la chiamata</td>
      <td>Non consentire telefonate</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>Annulla l'iscrizione</td>
      <td>Non inviare e-mail in blocco</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Valutazione della persona</td>
      <td>Valutazione</td>
      <td>lead qualitycode</td>
    </tr>
    <tr>
      <td>Indirizzo Microsoft 2</td>
      <td>Strada 2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Indirizzo Microsoft 3</td>
      <td>Strada 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Microsoft Do Not Email</td>
      <td>Non Consentire Le E-Mail</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>Microsoft Do Not Fax</td>
      <td>Non consentire fax</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Microsoft - Non inviare materiale di marketing</td>
      <td>Materiale di marketing</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>Telefono Microsoft (ab.)</td>
      <td>Telefono abitazione</td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>Metodo Di Contatto Preferito Da Microsoft</td>
      <td>Metodo di contatto preferito</td>
      <td>preferredcontactmethod code</td>
    </tr>
    <tr>
      <td>Argomento Microsoft</td>
      <td>Argomento</td>
      <td>oggetto</td>
    </tr>
    <tr>
      <td>Data ultimo momento di interesse</td>
      <td>Data ultimo momento di interesse</td>
      <td>mkt_lastengmomentdate</td>
    </tr>
    <tr>
      <td>Ultimo momento di interesse desc</td>
      <td>Ultimo momento di interesse desc</td>
      <td>mkt_lastinteressanti momentdesc</td>
    </tr>
    <tr>
      <td>Sorgente ultimo momento di interesse</td>
      <td>Sorgente ultimo momento di interesse</td>
      <td>mkt_leadingInteressomomentsource</td>
    </tr>
    <tr>
      <td>Ultimo tipo di momento di interesse</td>
      <td>Ultimo tipo di momento di interesse</td>
      <td>mkt_lastinteressante momenttype</td>
    </tr>
    <tr>
      <td>Azienda</td>
      <td>Nome azienda</td>
      <td>nome società</td>
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
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Oggetto</td>
      <td>Argomento</td>
      <td>oggetto</td>
    </tr>
    <tr>
      <td>Entrata annuale</td>
      <td>Entrata annuale</td>
      <td>ricavi</td>
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
      <th>Nome API MS Dynamics</th>
    </tr>
    <tr>
      <td>Proprietario </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>creato il</td>
      <td>creato il</td>
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
      <th>Nome API MS Dynamics</th>
    </tr>
    <tr>
      <td>Data di creazione Microsoft</td>
      <td>Creato il</td>
      <td>creato il</td>
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
      <td>In mezzo</td>
      <td>Secondo nome</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>Ultimo</td>
      <td>Cognome</td>
      <td>cognome</td>
    </tr>
    <tr>
      <td>E-mail</td>
      <td>E-mail</td>
      <td>emailaddress1</td>
    </tr>
    <tr>
      <td>Qualifica</td>
      <td>Qualifica</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>Telefono</td>
      <td>Telefono (uff.)</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>Mobile</td>
      <td>Telefono cellulare</td>
      <td>telefono cellulare</td>
    </tr>
    <tr>
      <td>Indirizzo</td>
      <td>Indirizzo 1: via 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Città</td>
      <td>Indirizzo 1: città</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Stato</td>
      <td>Indirizzo 1: Stato/Provincia</td>
      <td>address1_stateorprovince</td>
    </tr>
    <tr>
      <td>Paese</td>
      <td>Indirizzo 1: Paese</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Codice postale</td>
      <td>Indirizzo 1: CAP</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Stato della persona</td>
      <td>Stato</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>Motivo dello stato</td>
      <td>Motivo dello stato</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>Non effettuare la chiamata</td>
      <td>Non consentire telefonate</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>Annulla l'iscrizione</td>
      <td>Non inviare e-mail in blocco</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Indirizzo Microsoft 2</td>
      <td>Indirizzo 1: via 2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Indirizzo Microsoft 3</td>
      <td>Indirizzo 1: via 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Microsoft Do Not Email</td>
      <td>Non Consentire Le E-Mail</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>Telefono Microsoft (ab.)</td>
      <td>Telefono abitazione</td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>Metodo Di Contatto Preferito Da Microsoft</td>
      <td>Metodo Di Contatto Preferito</td>
      <td>preferredcontactmethod code</td>
    </tr>
    <tr>
      <td>Data ultimo momento di interesse</td>
      <td>Data ultimo momento di interesse</td>
      <td>mkt_lastengmomentdate</td>
    </tr>
    <tr>
      <td>Ultimo tipo di momento di interesse</td>
      <td>Ultimo tipo di momento di interesse</td>
      <td>mkt_lastinteressante momenttype</td>
    </tr>
    <tr>
      <td>Sorgente ultimo momento di interesse</td>
      <td>Sorgente ultimo momento di interesse</td>
      <td>mkt_leadingInteressomomentsource</td>
    </tr>
    <tr>
      <td>Ultimo momento di interesse desc</td>
      <td>Ultimo momento di interesse desc</td>
      <td>mkt_lastinteressanti momentdesc</td>
    </tr>
    <tr>
      <td>Microsoft - Non inviare materiale di marketing</td>
      <td>Materiale di marketing</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>Microsoft Do Not Fax</td>
      <td>Microsoft Do Not Fax</td>
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
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Punteggio relativo</td>
      <td>Punteggio relativo</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>Note della persona</td>
      <td>Descrizione</td>
      <td>descrizione </td>
    </tr>
    <tr>
      <td>Punteggio della persona</td>
      <td>Punteggio lead</td>
      <td>mkt_leadingScore</td>
    </tr>
    <tr>
      <td>Note della persona</td>
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
      <th>Nome API MS Dynamics</th>
    </tr>
    <tr>
      <td>Proprietario </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>creato il</td>
      <td>creato il</td>
    </tr>
    <tr>
      <td>parentcustomerid</td>
      <td>Nome azienda</td>
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
      <th>Nome API MS Dynamics</th>
    </tr>
    <tr>
      <td>Conto (a)</td>
      <td>Account</td>
      <td>accounttid</td>
    </tr>
    <tr>
      <td>Indirizzo di fatturazione</td>
      <td>Indirizzo 1: via 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Città di fatturazione</td>
      <td>Indirizzo 1: città</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Paese di fatturazione</td>
      <td>Indirizzo 1: Paese</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Codice postale di fatturazione</td>
      <td>Indirizzo 1: CAP</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Indirizzo di fatturazione Microsoft 2</td>
      <td>Indirizzo 1: via 2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Indirizzo di fatturazione Microsoft 3</td>
      <td>Indirizzo 1: via 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Numero di telefono</td>
      <td>Numero di telefono</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>Tipo di azienda</td>
      <td>Tipo di azienda</td>
      <td>businesstypecode</td>
    </tr>
    <tr>
      <td>Numero account Microsoft</td>
      <td>Numero account</td>
      <td>numero account</td>
    </tr>
    <tr>
      <td>Stato società Microsoft</td>
      <td>Stato</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>Entrata annuale</td>
      <td>Entrata annuale</td>
      <td>ricavi</td>
    </tr>
    <tr>
      <td>Note società</td>
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
      <td>numero di dipendenti</td>
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
      <td>numero di dipendenti</td>
    </tr>
  </tbody>
</table>

I campi Account riportati di seguito sono sincronizzati per uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo MS Dynamics</th>
      <th>Nome API MS Dynamics</th>
    </tr>
    <tr>
      <td>Proprietario </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>creato il</td>
      <td>creato il</td>
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
      <th>Nome API MS Dynamics</th>
    </tr>
    <tr>
      <td>Probabilità di chiusura</td>
      <td>Probabilità</td>
      <td>closeprobability</td>
    </tr>
    <tr>
      <td>Fase</td>
      <td>stato</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>Data di chiusura effettiva</td>
      <td>Data di chiusura effettiva</td>
      <td>actualclosedate</td>
    </tr>
    <tr>
      <td>Nome</td>
      <td>Argomento</td>
      <td>name</td>
    </tr>
    <tr>
      <td>Valore stimato</td>
      <td>Stim. Ricavi</td>
      <td>estimatedValue</td>
    </tr>
    <tr>
      <td>Descrizione</td>
      <td>Descrizione</td>
      <td>descrizione</td>
    </tr>
  </tbody>
</table>

I campi Account riportati di seguito sono sincronizzati per uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo MS Dynamics</th>
      <th>Nome API MS Dynamics</th>
    </tr>
    <tr>
      <td>Proprietario </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>Opportunità</td>
      <td>optionId</td>
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
      <td>Data di creazione Microsoft</td>
      <td>Data di creazione in MS Dynamics (può essere diversa da Creato in Marketo)</td>
    </tr>
    <tr>
      <td>Microsoft eliminato</td>
      <td>La persona era in Microsoft ma è stata eliminata e ora risiede solo in Marketo</td>
    </tr>
  </tbody>
</table>
