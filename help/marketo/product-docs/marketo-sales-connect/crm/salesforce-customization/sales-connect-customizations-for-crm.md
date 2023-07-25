---
unique-page-id: 14745793
description: Personalizzazioni di Sales Connect per CRM - Documenti Marketo - Documentazione del prodotto
title: Personalizzazioni di Sales Connect per CRM
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 1%

---

# Personalizzazioni di Sales Connect per CRM {#sales-connect-customizations-for-crm}

I campi e i pulsanti riportati di seguito sono creati dall’API dei metadati nel sistema CRM di Salesforce. Una volta creati i campi, gli amministratori devono configurare i layout di pagina nel CRM per esporli. Le istruzioni sono disponibili sul sito [qui](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Questo interessa sia i clienti ToutApp che Sales Connect.

## Installare le personalizzazioni in Salesforce {#how-to-install-customizations-in-salesforce}

1. In Sales Connect, fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/one.png)

1. In Impostazioni amministratore, seleziona **Salesforce**.

   ![](assets/two.png)

1. Clic **Personalizzazioni di Marketo Sales Connect**.

   ![](assets/three.png)

1. Clic **Connetti a Salesforce**.

   ![](assets/four.png)

1. Accedi a Salesforce.

   ![](assets/five.png)

## Aggiorna personalizzazione Salesforce {#update-salesforce-customization}

Gli aggiornamenti al pacchetto di personalizzazione di Salesforce includeranno miglioramenti e correzioni di bug. Per verificare se sono disponibili aggiornamenti o per eseguire un aggiornamento, attieniti alla procedura seguente.

>[!NOTE]
>
>**Autorizzazioni di amministrazione richieste.**

1. In [applicazione web](https://www.toutapp.com), fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. In Impostazioni amministrazione, fai clic su **Salesforce**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. Se sono disponibili aggiornamenti, verrà visualizzata la scheda Personalizzazione Sales Connect. Clic **Aggiorna personalizzazioni**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. Clic **Aggiorna**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. Attendere l&#39;installazione degli aggiornamenti. Il tempo di installazione varia in base al numero di versioni necessarie.

   ![](assets/sales-connect-customizations-for-crm-10.png)

Una volta completata, sulla scheda verrà visualizzato &quot;Le personalizzazioni di Sales Connect sono aggiornate&quot;.

![](assets/sales-connect-customizations-for-crm-11.png)

## Campi attività personalizzati {#custom-activity-fields}

Marketo rileverà la creazione dei nuovi campi, quindi eseguirà una compilazione unica dei dati, una nuova mappatura e una sincronizzazione continua dei valori in **nuovo** solo campi. I campi obsoleti non verranno aggiornati.

| **Nome campo** | **Descrizione** |
|---|---|
| ID presenza locale chiamata MSE | Come utente puoi scegliere Presenza locale come opzione quando effettui chiamate dal telefono MSE. Le chiamate in arrivo mostreranno un numero locale per il ricevente. |
| URL di registrazione chiamate MSE | È possibile registrare le chiamate e qui verrà registrato un collegamento per la registrazione. |
| Campagna MSE | Nome dei registri della campagna MSE di cui il contatto/lead è membro. |
| URL campagna MSE | Registra l’URL della campagna creata in MSE. Facendo clic su questo pulsante, la campagna verrà aperta nell’app web MSE. |
| Passaggio corrente della campagna MSE | Se un contatto/lead fa parte di una campagna, questo campo registra il nome del passaggio in cui si trova il lead/contatto. |
| Allegato e-mail MSE visualizzato | Registra i dati quando un’e-mail viene inviata con un allegato e l’allegato viene visualizzato dal destinatario. |
| E-mail MSE selezionata | Registra un segno di spunta quando il destinatario fa clic su un collegamento in un messaggio e-mail. |
| E-mail MSE risposto | Registra un segno di spunta quando il destinatario risponde a un messaggio e-mail. |
| Stato e-mail MSE | Mostra se un’e-mail è inviata/in corso/non recapitata (il tracciamento delle e-mail non recapitate dipende dal canale di consegna utilizzato). |
| Modello e-mail MSE | Nome del registro del modello MSE utilizzato nell’e-mail inviata al lead/contatto. |
| URL modello e-mail MSE | Registra l’URL del modello creato in MSE. Facendo clic su questa icona si aprirà il modello nell’app Web MSE. |
| URL e-mail MSE | Facendo clic su questo URL verrà aperto il Centro comandi in MSE e verrà visualizzata la scheda Cronologia di Visualizzazione dettagli persone, in cui è possibile visualizzare l&#39;e-mail inviata. |
| E-mail MSE visualizzata | Registra un segno di spunta quando il destinatario visualizza un messaggio e-mail. |

## Campi di registrazione rollup {#roll-up-logging-fields}

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
   <td>Ultimo coinvolgimento in ingresso da Marketing. </td> 
  </tr> 
  <tr> 
   <td>MSE - Data ultimo accordo di marketing</td> 
   <td>Timestamp del coinvolgimento da Marketing.</td> 
  </tr> 
  <tr> 
   <td>MSE - Descrizione ultimo coinvolgimento marketing</td> 
   <td>Descrizione del coinvolgimento.</td> 
  </tr> 
  <tr> 
   <td>MSE - Ultima origine del coinvolgimento marketing</td> 
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
   <td colspan="1">Ultima risposta e-mail all’e-mail di vendita.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Campagna di vendita corrente</td> 
   <td colspan="1">Nome del registro della campagna MSE di cui il lead/contatto è membro.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Ultimo accordo di vendita</td> 
   <td colspan="1">Ultimo impegno in entrata dalle vendite. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Rinuncia</td> 
   <td colspan="1">Campo di rinuncia.</td> 
  </tr> 
 </tbody> 
</table>

## Pulsanti {#buttons}

| **Nome pulsante** | **Descrizione** |
|---|---|
| Invia e-mail MSE | Invia e-mail di vendita da Salesforce. |
| Aggiungi a campagna MSE | Campagne Add to MSE da Salesforce. |
| Invia a MSE | Invia il contatto da Salesforce a MSE. |
| Chiamata con MSE | Effettuare chiamate di vendita da Salesforce. |

## Pulsanti di azione in blocco {#bulk-action-buttons}

| **Nome pulsante** | **Descrizione** |
|---|---|
| Aggiungi a campagna MSE | Campagne Add to MSE da Salesforce. |
| Invia a MSE | Invia il contatto da Salesforce a MSE. |

## Guide utente {#user-guides}

[Rapporti personalizzati MSE in Salesforce](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE per Salesforce](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE per Salesforce Lightning](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
