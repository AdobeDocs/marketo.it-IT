---
unique-page-id: 11387674
description: Aggiornamenti alla terminologia di Marketo - Documentazione di Marketo - Documentazione del prodotto
title: Aggiornamenti alla terminologia di Marketo
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 1%

---

# Aggiornamenti alla terminologia di Marketo {#updates-to-marketo-terminology}

Stiamo apportando alcune modifiche alla nostra piattaforma, che influiranno su ciò che alcune cose vengono chiamate. Se disponi di una nuova istanza di Marketo a partire da marzo 2016 o se la tua azienda è stata rinnovata dopo luglio 2016, potresti visualizzare la nuova terminologia ora.

Anche se potresti trovare una terminologia diversa nella documentazione di Marketo, assicurati che tutti gli articoli verranno presto aggiornati per riflettere queste modifiche. Tutte le istruzioni sono le stesse.

Allora, cosa è cambiato?

## Il lead è ora una persona {#lead-is-now-person}

Il cambiamento più importante è la ridenominazione di Lead/Lead a persona/persone.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Antico</strong></td> 
   <td><strong>Nuovo</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img width="295" src="assets/leads.png" data-linked-resource-id="11387678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img width="295" src="assets/people.png" data-linked-resource-id="11387679" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

In alcuni casi, la parola &quot;lead&quot; viene semplicemente rimossa.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Antico</strong></td> 
   <td><strong>Nuovo</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-database.png" data-linked-resource-id="11387676" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <p><img src="assets/database.png" data-linked-resource-id="11387677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"></p> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Lead e persona **sono la stessa cosa**.

## Token {#tokens}

Token con la parola lead **non vengono modificati**. Ci scusiamo per ogni confusione; tuttavia, cambiare tutti i token in modo che corrispondano alla nuova terminologia interromperebbe molti token attualmente in uso. Quindi vedrai ancora token come &quot;`{{lead.First Name}}`.&quot; Non sono disponibili token specifici per una persona.

>[!NOTE]
>
>Là *è* un token chiamato &quot;Note personali&quot;, tuttavia quel token era sempre presente. In genere viene utilizzato per un campo di descrizione nel CRM, se del caso.

## Gestione dei campi {#field-management}

I campi contenenti il termine Lead sono stati sostituiti con Persona oppure la parola Lead è stata rilasciata. Un’eccezione rilevante è tuttavia il campo &quot;Proprietario lead&quot;. È ora noto come &quot;Proprietario vendite&quot;.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Antico</strong></td> 
   <td><strong>Nuovo</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-owner.png" data-linked-resource-id="11387757" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/sales-owner.png" data-linked-resource-id="11387758" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Per un elenco completo dei nomi di campo interessati, visita questo [Articolo di supporto](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target=&quot;_blank&quot;}.

## La personalizzazione in tempo reale (RTP, Real-Time Personalization) è ora la personalizzazione web {#real-time-personalization-rtp-is-now-web-personalization}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Antico</strong></td> 
   <td><strong>Nuovo</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/rtp.png" data-linked-resource-id="11387692" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/web.png" data-linked-resource-id="11387693" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Oltre alla modifica del nome, ora è costituito da quattro app separate:

| **[Personalizzazione web](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target=&quot;_blank&quot;}** | Ha un proprio riquadro sullo schermo home |
|---|---|
| **[Web Marketing basato su account](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target=&quot;_blank&quot;}** | Accessibile tramite il riquadro di personalizzazione web |
| **[Retargeting personalizzato](https://docs.marketo.com/display/DOCS/Website+Retargeting){target=&quot;_blank&quot;}** | Accessibile tramite il riquadro di personalizzazione web |
| **[Contenuto predittivo](https://docs.marketo.com/display/DOCS/Predictive+Content){target=&quot;_blank&quot;}** | Ha un proprio riquadro sullo schermo home |

>[!NOTE]
>
>I riquadri visibili nella schermata iniziale rifletteranno i moduli acquistati.

Grazie per la pazienza durante questo aggiornamento.
