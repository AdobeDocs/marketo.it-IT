---
description: NUR-YYYY-MM-Advanced Nurture - Documentazione Marketo - Documentazione del prodotto
title: Nurturing avanzato NUR-MM-AAAA
feature: Programs
exl-id: bd9c6605-a13f-4c73-aaa8-eca43cfcc950
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 10%

---

# Nurturing avanzato NUR-MM-AAAA {#nur-yyyy-mm-advanced-nurture}

Questo è un esempio di programmi di sviluppo avanzati che utilizzano il programma Marketo Engage Engagement. I programmi e-mail nidificati impediscono agli utenti di ricevere contenuti già utilizzati o controllano il tipo di contenuto da utilizzare in ciascun flusso. È possibile eseguire rapporti di attribuzione per ogni singolo programma e-mail nidificato. Canali: &quot;Nurture&quot; e un canale dedicato &quot;Nurture Email&quot; per i Programmi e-mail nidificati invia un’e-mail alla newsletter utilizzando un Programma e-mail di Marketo Engage. L’e-mail può includere o meno un test A/B.

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
   <td>Attività di nurturing</td>
   <td>01 - Membro
<br/>02 - Coinvolto - Completato</td>
   <td>Inclusivo</td>
   <td>Coinvolgimento</td>
  </tr>
  <tr>
   <td>E-mail per lo sviluppo</td>
   <td>01 - Salta
<br/>02 - Inviato
<br/>03 - Coinvolto - Completato</td>
   <td>Inclusivo</td>
   <td>Predefinito</td>
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
   <td>Programma nidificato</td>
   <td> </td>
   <td>01 - Argomento X</td>
  </tr>
  <tr>
   <td>Programma nidificato</td>
   <td> </td>
   <td>02 - Argomento Y</td>
  </tr>
  <tr>
   <td>Programma nidificato</td>
   <td> </td>
   <td>03 - Argomento Z</td>
  </tr>
  <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modello di e-mail per avvio rapido</a></td>
   <td>01 - E-mail (dal vivo nei programmi nidificati)</td>
  </tr>
   <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modello di e-mail per avvio rapido</a></td>
   <td>02 - E-mail (dal vivo nei programmi nidificati)</td>
  </tr>
   <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modello di e-mail per avvio rapido</a></td>
   <td>03 - E-mail (dal vivo nei programmi nidificati)</td>
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
   <td>Campagna avanzata</td>
   <td> </td>
   <td>00 - Salta e-mail (in ogni programma nidificato)</td>
  </tr>
  <tr>
   <td>Campagna avanzata</td>
   <td> </td>
   <td>01 - Invia e-mail (disponibile in ciascun programma nidificato)</td>
  </tr>
  <tr>
   <td>Campagna avanzata</td>
   <td> </td>
   <td>02 - Coinvolto-Successo (in ogni programma nidificato)</td>
  </tr>
  <tr>
   <td>Cartella</td>
   <td> </td>
   <td>Assets (contiene programmi nidificati e cartelle di risorse anche in Programmi nidificati per contenere le e-mail)</td>
  </tr>
  <tr>
   <td>Cartella</td>
   <td> </td>
   <td>Programmi nidificati (risiede nella cartella Assets)</td>
  </tr>
  <tr>
   <td>Cartella</td>
   <td> </td>
   <td>Campagne: ospita tutte le campagne intelligenti nel programma di sviluppo principale e le cartelle delle campagne sono anch’esse posizionate in ciascun programma nidificato</td>
  </tr>
  <tr>
   <td>Cartella</td>
   <td> </td>
   <td>Rapporti</td>
  </tr>
 </tbody>
</table>

![](assets/nur-yyyy-mm-advanced-nurture-1.png)

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

* Assicurati di disporre di regole per mettere in pausa e riprendere la cadenza dell’allattamento. Queste campagne intelligenti devono essere attivate o pianificate prima dell’attivazione del programma di coinvolgimento.

>[!NOTE]
>
>Ricorda di aggiornare i Valori token personali nel modello di programma e ogni volta che utilizzi il programma, in base alle esigenze.

>[!TIP]
>
>Non dimenticare di attivare la campagna &quot;04 - Coinvolto (Programma riuscito)&quot; per tenere traccia del successo. Esegui questa operazione _prima_ che le e-mail vengano inviate.
