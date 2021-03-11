---
description: Mappatura predefinita dei campi di Dynamics - Documenti Marketo - Documentazione del prodotto
title: Mappatura predefinita dei campi di Dynamics
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 1%

---


# Mappatura predefinita dei campi Dynamics {#default-dynamics-field-mapping}

Quando si sincronizza inizialmente l’account Marketo con Microsoft, Marketo crea automaticamente queste associazioni tra i campi incorporati Dynamics e Marketo.  Marketo sincronizzerà anche i campi personalizzati sui lead, account, opportunità e contatti.

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
   <td>Saluto</td> 
   <td>Saluto</td> 
   <td>saluto</td> 
  </tr> 
  <tr> 
   <td>Primo</td> 
   <td>Nome</td> 
   <td>nome</td> 
  </tr> 
  <tr> 
   <td>Medio</td> 
   <td>Nome centrale</td> 
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
   <td>Titolo processo</td> 
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
   <td>Origine lead</td> 
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
   <td>Non chiamare</td> 
   <td>Non consentire chiamate telefoniche</td> 
   <td>telefonino</td> 
  </tr> 
  <tr> 
   <td>Annulla sottoscrizione</td> 
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
   <td>Telefono principale Microsoft</td> 
   <td>Telefono abitazione</td> 
   <td>telefono2</td> 
  </tr> 
  <tr> 
   <td>Metodo Di Contatto Preferito Microsoft</td> 
   <td>Metodo di contatto preferito</td> 
   <td>preferredcontactmetodcode</td> 
  </tr> 
  <tr> 
   <td>Argomento Microsoft</td> 
   <td>Argomento</td> 
   <td>soggetto</td> 
  </tr> 
 </tbody> 
</table>

## Campi di contatto {#contact-fields}

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
   <td>Saluto</td> 
   <td>Saluto</td> 
   <td>saluto</td> 
  </tr> 
  <tr> 
   <td>Primo</td> 
   <td>Nome</td> 
   <td>nome</td> 
  </tr> 
  <tr> 
   <td>Medio</td> 
   <td>Nome centrale</td> 
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
   <td>Titolo processo</td> 
   <td>Titolo processo</td> 
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
   <td>Non chiamare</td> 
   <td>Non consentire chiamate telefoniche</td> 
   <td>telefonino</td> 
  </tr> 
  <tr> 
   <td>Annulla sottoscrizione</td> 
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
   <td>Telefono principale Microsoft</td> 
   <td>Telefono abitazione</td> 
   <td>telefono2</td> 
  </tr> 
  <tr> 
   <td>Metodo Di Contatto Preferito Microsoft</td> 
   <td>Metodo Di Contatto Preferito</td> 
   <td>preferredcontactmetodcode</td> 
  </tr> 
 </tbody> 
</table>

## Campi account {#account-fields}

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
   <td>Telefono principale</td> 
   <td>Telefono principale</td> 
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
   <td>Stato della società Microsoft</td> 
   <td>Stato</td> 
   <td>codice di stato</td> 
  </tr> 
  <tr> 
   <td>Entrate annuali</td> 
   <td>Entrate annuali</td> 
   <td>entrate</td> 
  </tr> 
  <tr> 
   <td>Note aziendali</td> 
   <td>Descrizione</td> 
   <td>descrizione</td> 
  </tr> 
  <tr> 
   <td>Industria</td> 
   <td>Industria</td> 
   <td>industrycode</td> 
  </tr> 
  <tr> 
   <td>Codice SIC</td> 
   <td>Codice SIC</td> 
   <td>sic</td> 
  </tr> 
  <tr> 
   <td>Sito Web</td> 
   <td>Sito Web</td> 
   <td>sito web</td> 
  </tr> 
 </tbody> 
</table>

## Campi di sistema correlati a Microsoft in Marketo (sola lettura) {#microsoft-related-system-fields-in-marketo}

Questi campi vengono creati in Marketo ma non possono essere regolati dai clienti.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Campo Marketo</th> 
   <th>Descrizione</th> 
  </tr> 
  <tr> 
   <td>Microsoft Type</td> 
   <td>Lead o contatto. Se vuoto, il lead esiste solo come persona in Marketo</td> 
  </tr> 
  <tr> 
   <td>Data creazione Microsoft</td> 
   <td>Data di creazione in MS Dynamics (può essere diversa da quella creata in Marketo)</td> 
  </tr> 
  <tr> 
   <td>Microsoft eliminato</td> 
   <td>Una persona era in Microsoft ma è stato eliminato e ora vive solo in Marketo</td> 
  </tr> 
 </tbody> 
</table>
