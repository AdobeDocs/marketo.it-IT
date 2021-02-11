---
unique-page-id: 14745793
description: Personalizzazioni di vendita Connect per CRM - Documenti Marketo - Documentazione prodotto
title: Personalizzazioni di Connect per CRM
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---


# Personalizzazioni di vendita Connect per CRM {#sales-connect-customizations-for-crm}

I campi e i pulsanti di seguito vengono creati dall&#39;API dei metadati in Salesforce CRM. Una volta creati i campi, gli amministratori devono configurare i layout di pagina nel CRM per esporli. Le istruzioni sono disponibili [qui](https://docs.marketo.com/display/docs/assets/marketo-sales-engage-for-salesforce-installation-and-success-guide.pdf).

>[!NOTE]
>
>Questo interessa sia i clienti ToutApp che i clienti di Sales Connect.

## Come installare le personalizzazioni in Salesforce {#how-to-install-customizations-in-salesforce}

1. In Sales Connect, fate clic sull&#39;icona a forma di ingranaggio e selezionate **Settings**.

   ![](assets/one.png)

1. In Impostazioni amministratore, seleziona **Salesforce**.

   ![](assets/two.png)

1. Fate clic su **Personalizzazioni di Marketing Connect per le vendite**.

   ![](assets/three.png)

1. Fare clic su **Connetti a Salesforce**.

   ![](assets/four.png)

1. Accedi a Salesforce.

   ![](assets/five.png)

## Campi attività personalizzati {#custom-activity-fields}

Marketo rileverà la creazione dei nuovi campi, quindi eseguirà una backfill una tantum di dati, una nuova mappatura e una sincronizzazione continua dei valori solo nei campi **new**. I vecchi campi non verranno aggiornati.

| **Nome campo** | **Descrizione** |
|---|---|
| ID presenza locale chiamata MSE | In qualità di utente potete scegliere Presenza locale come opzione quando effettuate chiamate dal telefono MSE. Le chiamate in arrivo visualizzeranno un numero locale per il ricevitore. |
| URL registrazione chiamata MSE | Le chiamate possono essere registrate e un collegamento per la registrazione verrà registrato qui. |
| Campagna MSE | Nome registro della campagna MSE di cui è membro il contatto/lead. |
| URL campagna MSE | URL registro per la campagna creata in MSE. Facendo clic su questo pulsante si aprirà la campagna nell&#39;app Web MSE. |
| Passaggio corrente campagna MSE | Se un contatto o un lead fa parte di una campagna, questo campo registra il nome del passaggio su cui il lead o il contatto è attualmente attivo. |
| Allegato e-mail MSE visualizzato | Registra i dati quando un&#39;e-mail viene inviata con un allegato e l&#39;allegato viene visualizzato dal destinatario. |
| Messaggio e-mail MSE selezionato | Registra un segno di spunta quando il destinatario fa clic su un collegamento in un messaggio e-mail. |
| Risposta e-mail MSE | Registra un segno di spunta quando il destinatario risponde a un&#39;e-mail. |
| Stato e-mail MSE | Indica se un messaggio e-mail è inviato/è in corso/rimbalzato (il tracciamento dei messaggi e-mail rimbalzati dipende dal canale di consegna utilizzato). |
| Modello e-mail MSE | Nome registro del modello MSE utilizzato nell’e-mail inviata al lead/contatto. |
| URL modello e-mail MSE | Registra l’URL del modello creato in MSE. Facendo clic su questo pulsante si aprirà il modello nell&#39;app Web MSE. |
| URL e-mail MSE | Facendo clic su questo URL si aprirà il centro comandi in MSE e si passerà alla scheda Cronologia visualizzazione dettagli persone, dove potrete vedere il messaggio e-mail inviato. |
| E-mail MSE visualizzata | Registra un segno di spunta quando il destinatario visualizza un messaggio e-mail. |

## Rollup dei campi di registrazione {#roll-up-logging-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Nome campo</strong></td> 
   <td><strong>Descrizione</strong></td> 
  </tr> 
  <tr> 
   <td>MSE - Ultimo coinvolgimento nel marketing</td> 
   <td>Ultimo coinvolgimento in arrivo da Marketing. </td> 
  </tr> 
  <tr> 
   <td>MSE - Data ultimo coinvolgimento marketing</td> 
   <td>Timestamp del coinvolgimento da Marketing.</td> 
  </tr> 
  <tr> 
   <td>MSE - Ultimo servizio di marketing</td> 
   <td>Descrizione del coinvolgimento.</td> 
  </tr> 
  <tr> 
   <td>MSE - Ultima origine di coinvolgimento nel marketing</td> 
   <td>Origine del coinvolgimento marketing.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Ultimo tipo di coinvolgimento marketing</td> 
   <td colspan="1">Tipo di coinvolgimento.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Ultima attività per vendite<br></td> 
   <td colspan="1">Ultima attività in uscita eseguita dal team vendite.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Ultima risposta</td> 
   <td colspan="1">Ultima risposta via e-mail al messaggio e-mail di vendita.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Campagna di vendita corrente</td> 
   <td colspan="1">Nome registro della campagna MSE di cui il lead/contatto è membro.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Ultimo impegno di vendita</td> 
   <td colspan="1">Ultimo coinvolgimento in arrivo dalle vendite. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Rifiuto</td> 
   <td colspan="1">Campo di rifiuto.</td> 
  </tr> 
 </tbody> 
</table>

## Pulsanti {#buttons}

| **Nome pulsante** | **Descrizione** |
|---|---|
| Invia e-mail MSE | Invia e-mail di vendita da Salesforce. |
| Aggiungi a campagna MSE | Aggiungi a campagne MSE da Salesforce. |
| Invia a MSE | Invia il contatto da Salesforce a MSE. |
| Chiama con MSE | Effettuare chiamate di vendita da Salesforce. |

## Pulsanti di azione di massa {#bulk-action-buttons}

| **Nome pulsante** | **Descrizione** |
|---|---|
| Aggiungi a campagna MSE | Aggiungi a campagne MSE da Salesforce. |
| Invia a MSE | Invia il contatto da Salesforce a MSE. |

## Guide utente {#user-guides}

[Report personalizzati MSE in Salesforce](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE per Salesforce](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE per fulmine Salesforce](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
