---
description: Pagina principale della pubblicità online OA-YYY-MM-Marketo - Documentazione Marketo - Documentazione del prodotto
title: Pagina di destinazione Marketo per la pubblicità online OA-YYY-MM
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 569f61f15a9bdeb31b3a60b237f0c19aad68800a
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 3%

---

# Pagina di destinazione Marketo per la pubblicità online OA-YYY-MM {#oa-yyyy-mm-online-advertising-marketo-landing-page}

Questo è un esempio di un programma di tracciamento della pubblicità online, che include una pagina di destinazione Marketo con modulo di registrazione e utilizza un programma predefinito Marketo. Il collegamento all’offerta può essere visualizzato nella pagina di ringraziamento, inviato tramite e-mail di ringraziamento o entrambi.

Per ulteriore assistenza sulla strategia o per personalizzare un programma, contatta il team dell’account Adobe o visita il [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} pagina.

## Riepilogo canale {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Canale</th> 
   <th>Stato iscrizione</th>
   <th>Comportamento di Analytics</th>
   <th>Tipo di programma</th>
  </tr> 
  <tr> 
   <td>Pubblicità online</td> 
   <td>01 - Membro 
<br/>02 - Coinvolto - Completato</td>
   <td>Inclusivo</td>
   <td>Predefinito</td>
  </tr>
 </tbody> 
</table>

## Il programma contiene le seguenti risorse {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo</th> 
   <th>Nome modello</th>
   <th>Nome risorsa</th>
  </tr> 
  <tr> 
   <td>Modulo</td> 
   <td> </td>
   <td>Registrazione di contenuti FM</td>
  </tr>
  <tr> 
   <td>E-mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modello e-mail di avvio rapido</a></td>
   <td>01-E-Mail-Grazie</td>
  </tr>
  <tr> 
   <td>Pagina di destinazione</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Modello di programma di apprendimento rapido</a></td>
   <td>01 - LP - Registrazione</td>
  </tr>
   <tr> 
   <td>Pagina di destinazione</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Modello di programma di apprendimento rapido</a></td>
   <td>02 - LP - Grazie</td>
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
   <td>00 - Acquisizione del programma</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>01 - Modulo compilato</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>02 - Coinvolto (successo del programma)</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Assets: contiene tutte le risorse creative 
<br/>(sottocartelle per e-mail e pagine di destinazione)  </td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Campagne: ospita tutte le campagne Smart</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Rapporti</td>
  </tr>
 </tbody> 
</table>

## I miei token inclusi {#my-tokens-included}

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
   <td><code>{{my.Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Testo</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL?senza http://</td>
  </tr>
 </tbody> 
</table>

SCHERMATA DEL PROGRAMMA

## Regole di conflitto {#conflict-rules}

* **Tag del programma**
   * Crea tag in questa sottoscrizione - _Consigliato_
   * Ignora

* **Modello per pagina di destinazione con lo stesso nome**
   * Copia modello originale
   * Usa modello di destinazione - _Consigliato_

* **Immagini con lo stesso nome**
   * Mantieni entrambi i file
   * Sostituisci elemento in questa sottoscrizione - _Consigliato_

* **Modelli e-mail con lo stesso nome**
   * Mantieni entrambi i modelli
   * Sostituisci modello esistente - _Consigliato_

SCHERMATA DELLE REGOLE DI CONFLITTO

## Best practice {#best-practices}

* Dopo aver importato il programma per contenuti, spostare il modulo da una risorsa locale a una risorsa globale disponibile in Design Studio.
   * La riduzione del numero di moduli e l’utilizzo di più risorse globali da Design Studio consentono una maggiore scalabilità nella progettazione dei programmi e nella governance amministrativa. Offre inoltre flessibilità per gli aggiornamenti regolari sulla conformità per campi, lingua di consenso, ecc.

* È consigliabile aggiornare i modelli nel programma importato per utilizzare i modelli attualmente contrassegnati con il marchio oppure aggiornare il modello appena importato in base al marchio aggiungendo uno snippet o le informazioni appropriate su logo/piè di pagina.

* Utilizza i tag del programma per filtrare i rapporti in base alle varie fonti di pubblicità online.

* Prendi in considerazione l’aggiornamento della convenzione di denominazione di questo esempio di programma per allinearla alla convenzione di denominazione.

>[!NOTE]
>
>Ricorda di aggiornare i Valori token personali nel modello di programma e ogni volta che utilizzi il programma, in base alle esigenze.

>[!TIP]
>
>Non dimenticare di attivare la campagna &quot;02 - Coinvolto (Programma riuscito)&quot; per tenere traccia del successo. Esegui questa operazione _prima di_ il modulo è attivo e le e-mail vengono inviate.

>[!IMPORTANT]
>
>I miei token che fanno riferimento a un URL non possono contenere http:// o https:// altrimenti il collegamento non funzionerà in modo appropriato all’interno della risorsa.
