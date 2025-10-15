---
description: Programma di fiere TS-YYY-MM-DD - Documentazione di Marketo - Documentazione del prodotto
title: Programma fiera TS-GG-MM-AAAA
feature: Programs
exl-id: 39ef8d6e-392b-456e-a925-b1f6c2cb81d8
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 10%

---

# Programma fiera TS-GG-MM-AAAA {#ts-yyyy-mm-dd-tradeshow-program}

Questo è un esempio di programma di fiere con inviti e e-mail di follow-up tramite un programma Marketo Engage Event.

Per ulteriore assistenza sulla strategia o per personalizzare un programma, contatta il team dell&#39;account Adobe o visita la pagina [Adobe Professional Services](https://business.adobe.com/it/customers/consulting-services/main.html){target="_blank"}.

## Riepilogo canale {#channel-summary}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Channel</th>
   <th>Stato iscrizione</th>
   <th>Comportamento di Analytics</th>
   <th>Tipo di programma</th>
  </tr>
  <tr>
   <td>Evento</td>
   <td>01 - Invitato
   <br/>02-In lista d'attesa
   <br/>03-Registrato
   Stand visitato da <br/>04
   <br/>05-Coinvolti allo spettacolo - Completato
   <br/>06-Coinvolto al post-show - operazione riuscita</td>
   <td>Inclusivo</td>
   <td>Evento</td>
  </tr>
 </tbody>
</table>

## Il programma contiene i seguenti Assets {#program-contains-the-following-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Tipo</th>
   <th>Nome modello</th>
   <th>Nome risorsa</th>
  </tr>
  <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modello di e-mail per avvio rapido</a></td>
   <td>01-E-Mail-Grazie</td>
  </tr>
   <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modello di e-mail per avvio rapido</a></td>
   <td>02a- E-mail - invito</td>
  </tr>
  <tr>
  <tr>
   <td>Rapporto locale</td>
   <td> </td>
   <td>Prestazioni e-mail</td>
  </tr>
  <tr>
   <td>Rapporto locale</td>
   <td> </td>
   <td>Prestazioni del programma</td>
  </tr>
  <tr>
   <td>Campagna avanzata</td>
   <td> </td>
   <td>00 - Acquisizione del programma</td>
  </tr>
  <tr>
   <td>Campagna avanzata</td>
   <td> </td>
   <td>01 - Invia invito</td>
  </tr>
   <tr>
   <td>Campagna avanzata</td>
   <td> </td>
   <td>02 - Inviare e-mail di follow-up</td>
  </tr>
   <tr>
   <td>Campagna avanzata</td>
   <td> </td>
   <td>03 - Coinvolto tramite e-mail di follow-up (operazione riuscita)</td>
  </tr>
  <tr>
   <td>Cartella</td>
   <td> </td>
   <td>Assets - Raccoglie tutte le risorse creative
<br/>(sottocartelle per e-mail e pagine di destinazione)</td>
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

![](assets/ts-yyyy-mm-dd-tradeshow-program-1.png)

## I miei token inclusi {#my-tokens-included}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Tipo di token</th>
   <th>Nome token</th>
   <th>Valore</th>
  </tr>
  <tr>
   <td>File di calendario</td>
   <td><code>{{my.AddToCalendar}}</code></td>
   <td>Doppio clic per dettagli</td>
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
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
  </tr>
   <tr>
   <td>Rich Text</td>
   <td><code>{{my.Event-Booth#}}</code></td>
   <td><code><--My Booth Number--></code></td>
  </tr>
   <tr>
   <td>Testo</td>
   <td><code>{{my.Event-City}}</code></td>
   <td><code><--My Event City Here--></code></td>
  </tr>
  <tr>
   <td>Testo</td>
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
  </tr>
  <tr>
   <td>Testo</td>
   <td><code>{{my.Event-Time}}</code></td>
   <td><code><--My Event Time + TimeZone--></code></td>
  </tr>
  <tr>
   <td>Testo</td>
   <td><code>{{my.Event-Title}}</code></td>
   <td><code><--My Event Title Here--></code></td>
  </tr>
  <tr>
   <td>Testo</td>
   <td><code>{{my.Event-Type}}</code></td>
   <td>Tradeshow</td>
  </tr>
 </tbody>
</table>

## Regole di conflitto {#conflict-rules}

* **Tag programma**
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

## Best practice {#best-practices}

* Dopo aver importato il programma del webinar, spostare il modulo da una risorsa locale a una risorsa globale disponibile in Design Studio.
   * La riduzione del numero di moduli e l’utilizzo di più risorse globali da Design Studio consentono una maggiore scalabilità nella progettazione dei programmi e nella governance amministrativa. Offre inoltre flessibilità per gli aggiornamenti regolari sulla conformità per campi, lingua di consenso, ecc.

* È consigliabile aggiornare i modelli nel programma importato per utilizzare i modelli attualmente contrassegnati con il marchio oppure aggiornare il modello appena importato in base al marchio aggiungendo uno snippet o le informazioni appropriate su logo/piè di pagina.

* Prendi in considerazione l’aggiornamento della convenzione di denominazione di questo esempio di programma per allinearla alla convenzione di denominazione.

>[!NOTE]
>
>Ricorda di aggiornare i Valori token personali nel modello di programma e ogni volta che utilizzi il programma, in base alle esigenze.

>[!TIP]
>
>Non dimenticare di attivare la campagna &quot;03 - Coinvolto tramite e-mail di follow-up (Programma riuscito)&quot; per tenere traccia del successo. Esegui questa operazione _prima_ che le e-mail vengano inviate.

>[!IMPORTANT]
>
>I miei token che fanno riferimento a un URL non possono contenere http:// o https:// altrimenti il collegamento non funzionerà in modo appropriato all’interno della risorsa.
