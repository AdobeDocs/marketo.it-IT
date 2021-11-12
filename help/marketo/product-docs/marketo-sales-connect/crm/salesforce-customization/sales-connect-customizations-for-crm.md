---
unique-page-id: 14745793
description: Personalizzazioni di vendita Connect per CRM - Marketo Docs - Documentazione del prodotto
title: Personalizzazioni di vendita Connect per CRM
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
source-git-commit: 2712a21b7457ef51a9112074465c54e8f7954fa9
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# Personalizzazioni di vendita Connect per CRM {#sales-connect-customizations-for-crm}

I campi e i pulsanti riportati di seguito vengono creati dall’API metadati in CRM Salesforce. Una volta creati i campi, gli amministratori devono configurare i layout di pagina nel proprio sistema di gestione delle relazioni con i clienti per esporli. Le istruzioni sono disponibili [qui](https://docs.marketo.com/display/docs/assets/marketo-sales-engage-for-salesforce-installation-and-success-guide.pdf).

>[!NOTE]
>
>Questo ha un impatto sia sui clienti ToutApp che su Sales Connect.

## Come installare personalizzazioni in Salesforce {#how-to-install-customizations-in-salesforce}

1. In Sales Connect, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/one.png)

1. In Impostazioni amministratore, seleziona **Salesforce**.

   ![](assets/two.png)

1. Fai clic su **Personalizzazioni di Marketo Sales Connect**.

   ![](assets/three.png)

1. Fai clic su **Connessione a Salesforce**.

   ![](assets/four.png)

1. Accedi a Salesforce.

   ![](assets/five.png)

## Aggiorna personalizzazione Salesforce {#update-salesforce-customization}

Gli aggiornamenti al pacchetto di personalizzazione Salesforce includeranno miglioramenti e correzioni di bug. Per verificare se sono disponibili aggiornamenti o per eseguire un aggiornamento, effettua le seguenti operazioni.

>[!NOTE]
>
>**Autorizzazioni di amministrazione richieste.**

1. In [applicazione web](https://www.toutapp.com), fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. In Impostazioni amministratore, fai clic su **Salesforce**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. Se sono disponibili aggiornamenti, verrà visualizzata la scheda Personalizzazione di Sales Connect. Fai clic su **Aggiorna personalizzazioni**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. Fai clic su **Aggiornamento**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. Attendi gli aggiornamenti da installare. A seconda dei numeri di versione necessari, il tempo di installazione varia.

   ![](assets/sales-connect-customizations-for-crm-10.png)

Una volta completata, la scheda mostrerà &quot;Le personalizzazioni di Sales Connect sono aggiornate&quot;.

![](assets/sales-connect-customizations-for-crm-11.png)

## Campi attività personalizzati {#custom-activity-fields}

Marketo rileverà la creazione dei nuovi campi e quindi eseguirà una retrocompilazione unica dei dati, una ri-mappatura e una sincronizzazione continua dei valori nel **nuovo** solo campi. I campi precedenti non verranno aggiornati.

| **Nome campo** | **Descrizione** |
|---|---|
| ID presenza locale chiamata MSE | In qualità di utente puoi scegliere Presenza locale come opzione quando effettui chiamate dal telefono MSE. Le chiamate in arrivo mostrano un numero locale per il ricevitore. |
| URL di registrazione della chiamata MSE | Le chiamate possono essere registrate e un link per la registrazione verrà registrato qui. |
| Campagna MSE | Nome di registro della campagna MSE di cui è membro il contatto/lead. |
| URL della campagna MSE | Registra l&#39;URL della campagna creata in MSE. Fai clic su questo pulsante per aprire la campagna nell’app Web MSE. |
| Passaggio corrente campagna MSE | Se un contatto/lead fa parte di una campagna, questo campo registra il nome del passaggio attualmente in cui si trova il lead/contatto. |
| Allegato e-mail MSE visualizzato | Registra i dati quando un’e-mail viene inviata con un allegato e l’allegato viene visualizzato dal destinatario. |
| E-mail MSE selezionata | Registra un segno di spunta quando il destinatario fa clic su un collegamento in un messaggio e-mail. |
| MSE Risposta E-Mail | Registra un segno di spunta quando il destinatario risponde a un’e-mail. |
| Stato e-mail MSE | Mostra se un’e-mail viene inviata/in corso/rimbalzata (il tracciamento delle e-mail rimbalzate dipende dal canale di consegna utilizzato). |
| Modello e-mail MSE | Registra il nome del modello MSE utilizzato nell&#39;e-mail inviata al lead/contatto. |
| URL modello e-mail MSE | Registra l&#39;URL del modello creato in MSE. Fai clic su questo pulsante per aprire il modello nell’app Web MSE. |
| URL e-mail MSE | Facendo clic su questo URL si aprirà il centro comandi in MSE e si aprirà la scheda della cronologia della visualizzazione dettagli persone in cui potrai visualizzare l’e-mail inviata. |
| E-mail MSE visualizzata | Registra un segno di spunta quando il destinatario visualizza un’e-mail. |

## Campi Di Registrazione Roll-Up {#roll-up-logging-fields}

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
   <td>MSE - Ultimo impegno di marketing</td> 
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
   <td>MSE - Ultima origine di coinvolgimento marketing</td> 
   <td>Origine dell’impegno di marketing.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Ultimo tipo di coinvolgimento marketing</td> 
   <td colspan="1">Tipo di coinvolgimento.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Ultima attività per vendita<br></td> 
   <td colspan="1">Ultima attività in uscita eseguita dal team vendite.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Ultima risposta</td> 
   <td colspan="1">Ultima risposta e-mail alle vendite.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Campagna di vendita corrente</td> 
   <td colspan="1">Registra il nome della campagna MSE di cui è membro il lead/contatto.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Ultimo impegno di vendita</td> 
   <td colspan="1">Ultimo impegno in arrivo dalle vendite. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Rinuncia</td> 
   <td colspan="1">Campo Rinuncia.</td> 
  </tr> 
 </tbody> 
</table>

## Pulsanti {#buttons}

| **Nome pulsante** | **Descrizione** |
|---|---|
| Invia e-mail MSE | Invia e-mail di vendita da Salesforce. |
| Aggiungi a campagna MSE | Aggiungi a campagne MSE da Salesforce. |
| Invia a MSE | Invia il contatto da Salesforce a MSE. |
| Chiamata con MSE | Effettua chiamate di vendita da Salesforce. |

## Pulsanti di azione in blocco {#bulk-action-buttons}

| **Nome pulsante** | **Descrizione** |
|---|---|
| Aggiungi a campagna MSE | Aggiungi a campagne MSE da Salesforce. |
| Invia a MSE | Invia il contatto da Salesforce a MSE. |

## Guide utente {#user-guides}

[Report personalizzati MSE in Salesforce](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE per Salesforce](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE per fulmine salesforce](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
