---
description: Contenuto su Marketo LP - Documentazione Marketo - Documentazione del prodotto
title: Contenuto su Marketo LP
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 661a41eb0c5c43541a63a36c31837b35f516d827
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 2%

---

# Contenuto su Marketo LP {#content-on-marketo-lp}

Nome del programma: CT-YYYY-MM-Content su Marketo LP

Questo esempio di riferimento è progettato per essere un programma di contenuti che sfrutta una pagina di destinazione Marketo con un modulo Marketo utilizzando un programma predefinito Marketo. Il modulo deve accedere al contenuto/offerta. Il collegamento all’offerta può essere visualizzato nella pagina di ringraziamento, inviato tramite e-mail di ringraziamento o entrambi. Per ulteriore assistenza sulla strategia o per personalizzare un programma, contatta il team dell’account Adobe o visita il [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) pagina.

**Riepilogo canale**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Canale</th> 
   <th>Stato iscrizione</th>
   <th>Comportamento di Analytics</th>
   <th>Tipo di programma</th>
  </tr> 
  <tr> 
   <td>Contenuto web</td> 
   <td>01 membro 
<br/>02-Coinvolto-Successo</td>
   <td>Inclusivo</td>
   <td>Predefinito</td>
  </tr>
 </tbody> 
</table>

**Il programma contiene le seguenti risorse:**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo</th> 
   <th>Nome modello</th>
   <th>Nome risorsa</th>
  </tr> 
  <tr> 
   <td>E-mail</td> 
   <td>Modello e-mail di avvio rapido</td>
   <td>01-E-Mail-Grazie</td>
  </tr>
  <tr> 
   <td>Pagina di destinazione</td> 
   <td>Modello di programma di apprendimento rapido</td>
   <td>01 - LP - Registrazione</td>
  </tr>
  <tr> 
   <td>Pagina di destinazione</td> 
   <td>Modello di programma di apprendimento rapido</td>
   <td>02 - LP - Grazie</td>
  </tr>
  <tr> 
   <td>Modulo</td> 
   <td> </td>
   <td>Modulo di registrazione contenuto</td>
  </tr>
  <tr> 
   <td>Rapporto locale</td> 
   <td> </td>
   <td>Prestazioni e-mail</td>
  </tr>
  <tr> 
   <td>Rapporto locale</td> 
   <td> </td>
   <td>Prestazioni della pagina di destinazione</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Modulo compilato da 01</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>02-Coinvolto (programma di successo)</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Assets: ospita tutte le risorse creative 
<br/>(sottocartelle per e-mail e pagine di destinazione)  </td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Campagne: ospita tutte le campagne intelligenti</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Rapporti</td>
  </tr>
 </tbody> 
</table>

SCHERMATA - Immagine del programma

**I miei token includono:**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo di token</th> 
   <th>Nome token</th>
   <th>Valore</th>
  </tr> 
  <tr> 
   <td>Rich Text</td> 
   <td><code>{{my.Content-Description}}</code></td>
   <td>Doppio clic per dettagli  
<br/><code><--My Content Description Here--></code> 
<br/>Modifica questa descrizione del contenuto a livello di programma, nella scheda I miei token. 
<br/>Imparerai: 
<li>Punto elenco 1</li>
<li>Punto elenco 2</li>
<li>Punto elenco 3</li></td>
  </tr>
  <tr> 
   <td>Testo</td> 
   <td><code>{{my.Content-Title}}</code></td>
   <td><code><--My Content Title Here--></code></td>
  </tr>
  <tr> 
   <td>Testo</td> 
   <td><code>{{my.Content-Type}}</code></td>
   <td><code><--My Content Type Here--></code></td>
  </tr>
  <tr> 
   <td>Testo</td> 
   <td><code>{{my.Content-URL}}</code></td>
   <td>my.ContentURL?without=http://</td>
  </tr>
  <tr> 
   <td>Testo</td> 
   <td><code>{{my.Email-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Testo</td> 
   <td><code>{{my.Email-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>Testo</td> 
   <td><code>{{my. Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Testo</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL?senza http://</td>
  </tr>
 </tbody> 
</table>

>[!CAUTION]
>
>Consulta Istruzioni di importazione del programma per le regole di conflitto predefinite.

**Regole di conflitto predefinite consigliate per l&#39;importazione:**

* Tag del programma
   * Crea tag in questa sottoscrizione (predefinito) - Consigliato
   * Ignora

* Modello per pagina di destinazione con lo stesso nome
   * Copia modello originale (impostazione predefinita)
   * Usa modello di destinazione - Consigliato

* Immagini con lo stesso nome
   * Mantieni entrambi i file (impostazione predefinita)
   * Sostituisci elemento in questa sottoscrizione - Consigliato

* Modelli e-mail con lo stesso nome
   * Mantieni entrambi i modelli (impostazione predefinita)
   * Sostituisci modello esistente - Consigliato

SCHERMATA - Immagine delle regole di conflitto predefinite

**Best practice consigliate:**

* Le best practice di Marketo Consulting consigliano di spostare il modulo da una risorsa locale a una risorsa globale che si trova in Design Studio of Marketi Engage dopo l’importazione del programma di contenuti.
   * La riduzione del numero di moduli e l’utilizzo di più risorse globali da Design Studio consentono una maggiore scalabilità nella progettazione dei programmi e nella governance amministrativa. Offre inoltre flessibilità per gli aggiornamenti regolari sulla conformità per campi, lingua di consenso, ecc.

* È consigliabile aggiornare i modelli nel programma importato per utilizzare i modelli attualmente contrassegnati con il marchio oppure aggiornare il modello appena importato in base al marchio aggiungendo uno snippet o le informazioni appropriate su logo e piè di pagina.

* Se necessario, è consigliabile aggiornare la convenzione di denominazione di questo modello di programma per allinearla alla convenzione di denominazione.

* Non dimenticare di aggiornare i Valori token personali nel modello di programma e ogni volta che utilizzi il programma, in base alle esigenze.

* Per ulteriore assistenza sulla strategia o per personalizzare un programma, contatta il team del tuo account di Adobe o visita [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) pagina.

>[!TIP]
>
>Non dimenticare di attivare la campagna &quot;02-Engaged&quot; per tenere traccia del successo. Esegui questa operazione PRIMA che il modulo sia attivo e che le e-mail vengano inviate.

>[!NOTE]
>
>I miei token che fanno riferimento a un URL non possono contenere http:// o https:// altrimenti il collegamento non funzionerà in modo appropriato all’interno della risorsa.
