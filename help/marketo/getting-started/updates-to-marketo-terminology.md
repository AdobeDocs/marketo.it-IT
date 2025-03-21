---
unique-page-id: 11387674
description: Aggiornamenti alla terminologia di Marketo - Documenti Marketo - Documentazione del prodotto
hide: true
hidefromtoc: true
title: Aggiornamenti alla terminologia di Marketo
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 1%

---

# Aggiornamenti alla terminologia di Marketo {#updates-to-marketo-terminology}

Stiamo apportando alcune modifiche alla nostra piattaforma, che influenzeranno ciò che alcuni elementi vengono chiamati. Se disponi di una nuova istanza di Marketo a partire da marzo 2016, o se la tua azienda è stata rinnovata dopo luglio 2016, ora potresti vedere la nuova terminologia.

Anche se nella documentazione di Marketo potresti notare una terminologia diversa, presto ogni articolo verrà aggiornato per riflettere queste modifiche. Tutte le istruzioni sono uguali.

Allora, cosa è cambiato?

## Il lead è ora la persona {#lead-is-now-person}

Il cambiamento più importante è la ridenominazione di lead/lead in persona/persone.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Vecchio</strong></td> 
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
   <td><strong>Vecchio</strong></td> 
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

I token con la parola lead in essi **non cambiano**. Ci scusiamo per qualsiasi confusione; tuttavia, cambiare tutti i token in modo che corrispondano alla nuova terminologia causerebbe la rottura di un sacco di token attualmente in uso. Verranno comunque visualizzati token come &quot;`{{lead.First Name}}`&quot;. Non sono presenti token specifici per le persone.

>[!NOTE]
>
>*è* un token denominato &quot;Note persona&quot;, tuttavia tale token era sempre presente. In genere viene utilizzato per un campo di descrizione nel CRM, se del caso.

## Gestione dei campi {#field-management}

I campi contenenti il termine Lead sono stati sostituiti con Person oppure la parola Lead è stata eliminata. Tuttavia, un’eccezione degna di nota è il campo &quot;Proprietario lead&quot;. Ora è noto come &quot;Proprietario vendite&quot;.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Vecchio</strong></td> 
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
>Per un elenco completo dei nomi di campo interessati, visita questo [articolo di supporto](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target="_blank"}.

## Real-Time Personalization (RTP) è ora Web Personalization {#real-time-personalization-rtp-is-now-web-personalization}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Vecchio</strong></td> 
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

| **[Web Personalization](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target="_blank"}** | Ha un riquadro proprio nella schermata iniziale |
|---|---|
| **[Marketing Web basato su account](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target="_blank"}** | Accessibile tramite riquadro Personalization Web |
| **[Retargeting personalizzato](https://docs.marketo.com/display/DOCS/Website+Retargeting){target="_blank"}** | Accessibile tramite riquadro Personalization Web |
| **[Contenuto predittivo](https://docs.marketo.com/display/DOCS/Predictive+Content){target="_blank"}** | Ha un riquadro proprio nella schermata iniziale |

>[!NOTE]
>
>Le tessere visibili nella schermata iniziale rifletteranno i moduli acquistati.

Grazie per la pazienza dimostrata durante l&#39;aggiornamento.
