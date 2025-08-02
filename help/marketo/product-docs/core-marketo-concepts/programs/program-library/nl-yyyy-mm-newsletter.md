---
description: NL-YYYY-MM-Newsletter - Documentazione Marketo - Documentazione del prodotto
title: Newsletter NL-YYYY-MM
feature: Programs
exl-id: bce05e0f-e288-4614-9d05-c14844615454
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 5%

---

# Newsletter NL-YYYY-MM {#nl-yyyy-mm-newsletter}

In questo esempio viene inviata un’e-mail alla newsletter utilizzando un programma e-mail di Marketo Engage. L’e-mail può includere o meno un test A/B.

Per ulteriore assistenza sulla strategia o per personalizzare un programma, contatta il team dell&#39;account Adobe o visita la pagina [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}.

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
   <td>Newsletter</td>
   <td>01 membro
<br/>02-Coinvolto-Riuscito</td>
   <td>Inclusivo</td>
   <td>E-mail</td>
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
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modello e-mail di avvio rapido</a></td>
   <td>01 - E-mail</td>
  </tr>
  <tr>
   <td>Rapporto locale</td>
   <td> </td>
   <td>Prestazioni e-mail</td>
  </tr>
  <tr>
   <td>Rapporto locale</td>
   <td> </td>
   <td>Prestazioni collegamento e-mail</td>
  </tr>
  <tr>
  <tr>
   <td>Campagna avanzata</td>
   <td> </td>
   <td>01 - Coinvolto (successo del programma)</td>
  </tr>
  <tr>
   <td>Cartella</td>
   <td> </td>
   <td>Assets - Raccoglie tutte le risorse creative
<br/>(sottocartelle per e-mail)  </td>
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

![](assets/nl-yyyy-mm-newsletter-1.png)

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

* È consigliabile aggiornare i modelli nel programma importato per utilizzare i modelli attualmente contrassegnati con il marchio oppure aggiornare il modello appena importato in base al marchio aggiungendo uno snippet o le informazioni appropriate su logo/piè di pagina.

* Prendi in considerazione l’aggiornamento della convenzione di denominazione di questo esempio di programma per allinearla alla convenzione di denominazione.

>[!NOTE]
>
>Ricorda di aggiornare i Valori token personali nel modello di programma e ogni volta che utilizzi il programma, in base alle esigenze.

>[!TIP]
>
>Non dimenticare di attivare la campagna &quot;01-Engaged&quot; per il successo del tracciamento. Esegui questa operazione _prima_ che il modulo sia attivo e che le e-mail vengano inviate.
