---
unique-page-id: 14745793
description: Personalizzazioni di [!DNL Sales Connect] per CRM - Documentazione di Marketo - Documentazione del prodotto
title: Personalizzazioni di [!DNL Sales Connect] per CRM
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 2%

---

# Personalizzazioni di [!DNL Sales Connect] per CRM {#sales-connect-customizations-for-crm}

I campi e i pulsanti riportati di seguito vengono creati dall&#39;API metadati in Salesforce CRM. Una volta creati i campi, gli amministratori devono configurare i layout di pagina nel CRM per esporli. Le istruzioni [sono disponibili qui](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf).

## Come installare le personalizzazioni in [!DNL Salesforce] {#how-to-install-customizations-in-salesforce}

1. In [!DNL Sales Connect], fare clic sull&#39;icona a forma di ingranaggio e selezionare **[!UICONTROL Settings]**.

   ![](assets/one.png)

1. In [!UICONTROL Admin Settings], selezionare **[!UICONTROL Salesforce]**.

   ![](assets/two.png)

1. Fai clic su **[!UICONTROL Marketo Sales Engage Customizations]**.

   ![](assets/three.png)

1. Fai clic su **[!UICONTROL Connect to Salesforce]**.

   ![](assets/four.png)

1. Accedere a [!DNL Salesforce].

   ![](assets/five.png)

## Aggiorna personalizzazione [!DNL Salesforce] {#update-salesforce-customization}

Gli aggiornamenti al pacchetto di personalizzazione [!DNL Salesforce] includeranno miglioramenti e correzioni di bug. Per verificare se sono disponibili aggiornamenti o per eseguire un aggiornamento, attieniti alla procedura seguente.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste.**

1. Nell&#39;[applicazione Web](https://www.toutapp.com), fare clic sull&#39;icona ingranaggio e selezionare **[!UICONTROL Settings]**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. In [!UICONTROL Admin Settings], fare clic su **[!UICONTROL Salesforce]**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. La scheda Personalizzazione [!DNL Sales Connect] mostrerà se sono disponibili aggiornamenti. Fai clic su **[!UICONTROL Update Customizations]**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. Fai clic su **[!UICONTROL Upgrade]**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. Attendere l&#39;installazione degli aggiornamenti. Il tempo di installazione varia in base al numero di versioni necessarie.

   ![](assets/sales-connect-customizations-for-crm-10.png)

Una volta completata, sulla scheda verrà visualizzato &quot;Le personalizzazioni di Sales Connect sono aggiornate&quot;.

![](assets/sales-connect-customizations-for-crm-11.png)

## Campi attività personalizzati {#custom-activity-fields}

Marketo rileverà la creazione dei nuovi campi, quindi eseguirà una retrocompilazione unica dei dati, una nuova mappatura e una sincronizzazione continua dei valori solo nei campi **new**. I campi obsoleti non verranno aggiornati.

<table><thead>
  <tr>
    <th>Nome campo</th>
    <th>Descrizione</th>
  </tr></thead>
<tbody>
  <tr>
    <td>ID presenza locale chiamata MSE</td>
    <td>Come utente puoi scegliere Presenza locale come opzione quando effettui chiamate dal telefono MSE. Le chiamate in arrivo mostreranno un numero locale per il ricevente.</td>
  </tr>
  <tr>
    <td>URL di registrazione chiamate MSE</td>
    <td>È possibile registrare le chiamate e qui verrà registrato un collegamento per la registrazione.</td>
  </tr>
  <tr>
    <td>Campagna MSE</td>
    <td>Nome dei registri della campagna MSE di cui il contatto/lead è membro.</td>
  </tr>
  <tr>
    <td>URL campagna MSE</td>
    <td>Registra l’URL della campagna creata in MSE. Facendo clic su questo pulsante, la campagna verrà aperta nell’app web MSE.</td>
  </tr>
  <tr>
    <td>Passaggio corrente della campagna MSE</td>
    <td>Se un contatto/lead fa parte di una campagna, questo campo registra il nome del passaggio in cui si trova il lead/contatto.</td>
  </tr>
  <tr>
    <td>Allegato e-mail MSE visualizzato</td>
    <td>Registra i dati quando un’e-mail viene inviata con un allegato e l’allegato viene visualizzato dal destinatario.</td>
  </tr>
  <tr>
    <td>E-mail MSE selezionata</td>
    <td>Registra un segno di spunta quando il destinatario fa clic su un collegamento in un messaggio e-mail.</td>
  </tr>
  <tr>
    <td>E-mail MSE risposto</td>
    <td>Registra un segno di spunta quando il destinatario risponde a un messaggio e-mail.</td>
  </tr>
  <tr>
    <td>Stato e-mail MSE</td>
    <td>Mostra se un’e-mail è inviata/in corso/non recapitata (il tracciamento delle e-mail non recapitate dipende dal canale di consegna utilizzato).</td>
  </tr>
  <tr>
    <td>Modello e-mail MSE</td>
    <td>Nome del registro del modello MSE utilizzato nell’e-mail inviata al lead/contatto.</td>
  </tr>
  <tr>
    <td>URL modello e-mail MSE</td>
    <td>Registra l’URL del modello creato in MSE. Facendo clic su questa icona si aprirà il modello nell’app Web MSE.</td>
  </tr>
  <tr>
    <td>URL e-mail MSE</td>
    <td>Facendo clic su questo URL verrà aperto il Centro comandi in MSE e verrà visualizzata la scheda Cronologia di Visualizzazione dettagli persone, in cui è possibile visualizzare l'e-mail inviata.</td>
  </tr>
  <tr>
    <td>E-mail MSE visualizzata</td>
    <td>Registra un segno di spunta quando il destinatario visualizza un messaggio e-mail.</td>
  </tr>
</tbody></table>

## Campi di registrazione rollup {#roll-up-logging-fields}

<table><thead>
  <tr>
    <th>Nome campo</th>
    <th>Descrizione</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE - Ultimo impegno di marketing</td>
    <td>Ultimo coinvolgimento in ingresso da Marketing.</td>
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
    <td>MSE - Ultimo Source di coinvolgimento marketing</td>
    <td>Source del coinvolgimento nel marketing.</td>
  </tr>
  <tr>
    <td>MSE - Ultimo tipo di coinvolgimento marketing</td>
    <td>Tipo di coinvolgimento.</td>
  </tr>
  <tr>
    <td>MSE - Ultima attività per vendite</td>
    <td>Ultima attività in uscita eseguita dal team vendite.</td>
  </tr>
  <tr>
    <td>MSE - Ultima risposta</td>
    <td>Ultima risposta e-mail all’e-mail di vendita.</td>
  </tr>
  <tr>
    <td>MSE - Campagna di vendita corrente</td>
    <td>Nome del registro della campagna MSE di cui il lead/contatto è membro.</td>
  </tr>
  <tr>
    <td>MSE - Ultimo accordo di vendita</td>
    <td>Ultimo impegno in entrata dalle vendite.</td>
  </tr>
  <tr>
    <td>MSE - Rinuncia</td>
    <td>Campo di rinuncia.</td>
  </tr>
</tbody></table>

## Pulsanti {#buttons}

<table><thead>
  <tr>
    <th>Nome pulsante</th>
    <th>Descrizione</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Invia e-mail MSE</td>
    <td>Invia e-mail vendite da Salesforce.</td>
  </tr>
  <tr>
    <td>Aggiungi a campagna MSE</td>
    <td>Aggiungi a campagne MSE da Salesforce.</td>
  </tr>
  <tr>
    <td>Invia a MSE</td>
    <td>Invia il contatto da Salesforce a MSE.</td>
  </tr>
  <tr>
    <td>Chiamata con MSE</td>
    <td>Effettuare chiamate di vendita da Salesforce.</td>
  </tr>
</tbody>
</table>

## Pulsanti di azione in blocco {#bulk-action-buttons}

<table><thead>
  <tr>
    <th>Nome pulsante</th>
    <th>Descrizione</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Aggiungi a campagna MSE</td>
    <td>Aggiungi a campagne MSE da Salesforce.</td>
  </tr>
  <tr>
    <td>Invia a MSE</td>
    <td>Invia il contatto da Salesforce a MSE.</td>
  </tr>
</tbody>
</table>

## Guide utente {#user-guides}

[Rapporti personalizzati MSE in Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/reports-and-dashboards.pdf)

[MSE per Salesforce Classic](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf)

[MSE per Salesforce Lightning](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/sfdc-guide-lightning.pdf)
