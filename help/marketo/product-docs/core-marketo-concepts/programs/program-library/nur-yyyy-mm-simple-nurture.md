---
description: NUR-YYYY-MM-Simple Nurture - Documentazione di Marketo - Documentazione del prodotto
title: NUR-YYYY-MM-Statura semplice
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 5aa0c2e3be16219613f0c72235428a962f8d58b3
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 4%

---

# NUR-YYYY-MM-Statura semplice {#nur-yyyy-mm-simple-nurture}

Questo è un esempio di semplici programmi di sviluppo, che utilizzano il programma di coinvolgimento del Marketo Engage, con contenuto cadenziato da versare nel tempo nel database utilizzando i flussi per guidare i record attraverso i percorsi in base al comportamento.

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
   <td>Allevamento</td> 
   <td>01 - Membro 
<br/>02 - Coinvolto - Completato</td>
   <td>Inclusivo</td>
   <td>Coinvolgimento</td>
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
   <td>E-mail</td> 
   <td>Modello e-mail di avvio rapido</td>
   <td>01 - E-mail</td>
  </tr>
   <tr> 
   <td>E-mail</td> 
   <td>Modello e-mail di avvio rapido</td>
   <td>02 - E-mail</td>
  </tr>
   <tr> 
   <td>E-mail</td> 
   <td>Modello e-mail di avvio rapido</td>
   <td>03 - E-mail</td>
  </tr>
  <tr> 
   <td>Rapporto locale</td> 
   <td> </td>
   <td>Prestazioni e-mail</td>
  </tr>
  <tr> 
   <td>Rapporto locale</td> 
   <td> </td>
   <td>Prestazioni del flusso di coinvolgimento</td>
  </tr>
  <tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>01 - Aggiungere allo sviluppo</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>02 - Pausa sviluppo</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>03 - Riprendere l’allattamento</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>04 - Coinvolto (successo del programma)</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Assets: ospita tutte le risorse creative
   <br/>(sottocartelle per e-mail)</td>
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

## I miei token inclusi {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo di token</th> 
   <th>Nome token</th>
   <th>Valore</th>
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

* È consigliabile aggiornare i modelli nel programma importato per utilizzare i modelli attualmente contrassegnati con il marchio oppure aggiornare il modello appena importato in base al marchio aggiungendo uno snippet o le informazioni appropriate su logo/piè di pagina.

* Prendi in considerazione l’aggiornamento della convenzione di denominazione di questo esempio di programma per allinearla alla convenzione di denominazione.

* Assicurati di disporre di regole per mettere in pausa e riprendere la cadenza dell’allattamento. Queste campagne intelligenti devono essere attivate o pianificate prima dell’attivazione del programma di coinvolgimento.

>[!NOTE]
>
>Ricorda di aggiornare i Valori token personali nel modello di programma e ogni volta che utilizzi il programma, in base alle esigenze.

>[!TIP]
>
>Non dimenticare di attivare la campagna &quot;04 - Coinvolto (Programma riuscito)&quot; per tenere traccia del successo. Esegui questa operazione _prima di_ le e-mail vengono inviate.
