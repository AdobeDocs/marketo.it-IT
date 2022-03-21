---
description: Disinstallare il pacchetto di personalizzazione Salesforce Lightning - Marketo Docs - Documentazione del prodotto
title: Disinstallare il pacchetto di personalizzazione Salesforce Lightning
exl-id: 4af89222-22b1-4c08-8081-3dab89d1985b
source-git-commit: f2f81167066c2f170f81308b2deec52d19efafb3
workflow-type: tm+mt
source-wordcount: '1182'
ht-degree: 0%

---

# Disinstallare il pacchetto di personalizzazione Salesforce Lightning {#uninstall-salesforce-lightning-customization-package}

Disinstalla il pacchetto Marketo Sales Connect dal tuo account Salesforce dopo aver iniziato a utilizzare il pacchetto Azioni MSI.

## Rimuovi campi di vendita Connect dal layout di pagina {#remove-sales-connect-fields-from-page-layout}

1. In Salesforce Lightning, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Configurazione**.

   ![](assets/uninstall-salesforce-lightning-customization-package-1.png)

1. Fai clic su **Gestione oggetti**.

   ![](assets/uninstall-salesforce-lightning-customization-package-2.png)

1. Scorri verso il basso e seleziona **Lead**.

   ![](assets/uninstall-salesforce-lightning-customization-package-3.png)

1. Fai clic su **Layout di pagina**.

   ![](assets/uninstall-salesforce-lightning-customization-package-4.png)

1. Fai clic su **Layout lead**.

   ![](assets/uninstall-salesforce-lightning-customization-package-5.png)

   >[!NOTE]
   >
   >La visualizzazione Modifica layout pagina non è ancora stata aggiornata in Salesforce Lightning.

1. Nella console, seleziona **Campi**. In Ricerca rapida, cerca &quot;MSC&quot;. Tutti i campi disattivati sono stati aggiunti al layout di pagina. Dovrai eliminarle.

   ![](assets/uninstall-salesforce-lightning-customization-package-6.png)

   >[!NOTE]
   >
   >Se nessuno dei campi è disabilitato, significa che non li hai aggiunti al layout di pagina. Puoi saltare questa sezione.

1. Scorri fino alla sezione con i campi personalizzati di vendita Connect.

   ![](assets/uninstall-salesforce-lightning-customization-package-7.png)

1. Ci sono 10 tipi di campi MSC che possono essere aggiunti a questa sezione. Rimuovi tutti i campi aggiunti o elimina semplicemente l’intera sezione.

1. Fai clic su **Salvataggio rapido** al termine.

   ![](assets/uninstall-salesforce-lightning-customization-package-8.png)

## Rimuovere i pulsanti di connessione alle vendite dai layout di pagina {#remove-sales-connect-buttons-from-page-layouts}

1. Nella console (passaggio 4 precedente), seleziona **Pulsanti**. Cerca &quot;MSC&quot;. Tutti i pulsanti disattivati sono stati aggiunti alla sezione dei pulsanti personalizzati. Dovrai eliminarle.

   ![](assets/uninstall-salesforce-lightning-customization-package-9.png)

   >[!NOTE]
   >
   >Se nessuno dei pulsanti è disabilitato, significa che non li hai aggiunti. Puoi saltare questa sezione.

1. Trascina i pulsanti MSC dalla sezione Pulsanti personalizzati alla console.

   ![](assets/uninstall-salesforce-lightning-customization-package-10.png)

1. Fai clic su **Salvataggio rapido** al termine.

   ![](assets/uninstall-salesforce-lightning-customization-package-11.png)

## Rimuovi campi di connessione vendite dalla sezione Cronologia attività {#remove-sales-connect-fields-from-activity-history-section}

1. Scorri fino alla parte inferiore della pagina, fino alla sezione dell’elenco relativo alla cronologia delle attività e fai clic sull’icona a forma di chiave inglese .

   ![](assets/uninstall-salesforce-lightning-customization-package-12.png)

1. Selezionare Campi di connessione vendite dall&#39;area Campi selezionati e fare clic sulla freccia Rimuovi. Fai clic su **OK** al termine.

   ![](assets/uninstall-salesforce-lightning-customization-package-13.png)

   >[!NOTE]
   >
   >L&#39;abbreviazione MSE _è_ Sales Connect È solo il nome precedente, &quot;Marketo Sales Engage&quot;.

1. Fai clic su **Salva** quando hai finito con la pagina Lead.

## Rimuovere i pulsanti di azione in blocco di vendita Connect dalla visualizzazione elenco lead {#remove-sales-connect-bulk-action-buttons-from-lead-list-view}

1. In Salesforce Lightning, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Configurazione**.

   ![](assets/uninstall-salesforce-lightning-customization-package-14.png)

1. Fai clic su **Gestione oggetti**.

   ![](assets/uninstall-salesforce-lightning-customization-package-15.png)

1. Scorri verso il basso e seleziona **Lead**.

   ![](assets/uninstall-salesforce-lightning-customization-package-16.png)

1. Fai clic su **Layout di ricerca**.

   ![](assets/uninstall-salesforce-lightning-customization-package-17.png)

1. Fai clic sulla freccia accanto a Vista a elenco e seleziona **Modifica**.

   ![](assets/uninstall-salesforce-lightning-customization-package-18.png)

1. Seleziona **Aggiungi alla campagna MSC**, **Email con MSC** e **Spingi a MSC** e fare clic sulla freccia Rimuovi. Quindi fai clic su **Salva**.

   ![](assets/uninstall-salesforce-lightning-customization-package-19.png)

Non è più necessario visualizzare i pulsanti nella vista a elenco di lead.

## Rimuovi configurazione MSC per i contatti {#remove-msc-configuration-for-contacts}

1. In Salesforce Lightning, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Configurazione**.

1. Fai clic su **Gestione oggetti**.

1. Scorri verso il basso e seleziona **Contatto**.

1. Fai clic su **Layout di pagina**.

1. Fai clic su **Layout dei contatti**.

1. Ripetere i passaggi da tutte e tre le sezioni.

## Rimuovi configurazione MSC per opportunità {#remove-msc-configuration-for-opportunity}

1. In Salesforce Lightning, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Configurazione**.

1. Fai clic su **Gestione oggetti**.

1. Scorri verso il basso e seleziona **Opportunità**.

1. Fai clic su **Layout di pagina**.

1. Fai clic su **Layout opportunità**.

La visualizzazione Opportunità dispone di un solo pulsante: &quot;Invia e-mail MSE&quot; e i campi seguenti:

![](assets/uninstall-salesforce-lightning-customization-package-20.png)

## Rimuovi configurazione MSC per account {#remove-msc-configuration-for-account}

1. In Salesforce Lightning, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Configurazione**.

1. Fai clic su **Gestione oggetti**.

1. Scorri verso il basso e seleziona **Account**.

1. Fai clic su **Layout di pagina**.

1. Fai clic su **Layout account**.

La visualizzazione account ha un solo pulsante: &quot;Invia e-mail MSE&quot; e i campi seguenti:

![](assets/uninstall-salesforce-lightning-customization-package-21.png)

## Rimuovi casella in uscita vendite Marketo {#remove-marketo-sales-outbox}

1. In Salesforce, fai clic sul pulsante **+** nella parte superiore dello schermo.

1. Fai clic su **Personalizzare le schede**.

1. Seleziona l’opzione Marketo Sales Outbox da destra. Fare clic sulla freccia Rimuovi, quindi fare clic su **Salva**.

## Elimina pacchetto di vendita {#delete-sales-connect-package}

Dopo aver rimosso tutti gli oggetti dal tuo account Salesforce, segui i passaggi seguenti.

1. In Salesforce Lightning, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Configurazione**.

1. Nella casella Ricerca rapida immettere &quot;Classi Apex&quot;.

1. Fai clic su **Elimina** accanto a tutte le voci &quot;MarketoSalesConnectionCustomization&quot; o &quot;MarketoSalesEngageCustomization&quot; nell’elenco.

Sei pronto!

Elenco di tutti gli oggetti che devono essere rimossi dall’istanza Salesforce:

## Dettagli sulla personalizzazione di Sales Connect {#sales-connect-customization-details}

<table>
 <tr>
  <th>Campi attività personalizzati</th>
  <th>Descrizione</th>
  <th>Tipo</th>
  <th>Tipo di dati</th>
 </tr>
 <tr>
  <td>ID presenza locale chiamata MSC</td>
  <td>In qualità di utente, posso scegliere Presenza locale come opzione quando effettuo chiamate da MSC Phone. Le chiamate in arrivo mostrano un numero locale per il ricevitore</td>
  <td>Attività</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>URL registrazione chiamata MSC</td>
  <td>Le chiamate possono essere registrate e un link per la registrazione verrà registrato qui </td>
  <td>Attività</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>Campagna MSC</td>
  <td>Nome del registro della campagna MSC su cui si trova il contatto/lead</td>
  <td>Attività</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>URL della campagna MSC</td>
  <td>Registra l'URL della campagna creata in MSC. Fai clic su questo pulsante per aprire la campagna nell’app web MSC.</td>
  <td>Attività</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>Passaggio corrente campagna MSC</td>
  <td>Se un contatto/lead si trova in una campagna, questo campo registra il nome del passaggio su cui si trovano.</td>
  <td>Attività</td>
  <td>Casella di controllo</td>
 </tr>
 <tr>
  <td>Allegato e-mail MSC visualizzato</td>
  <td>Registra i dati quando un’e-mail viene inviata con un allegato visualizzato dal destinatario</td>
  <td>Attività</td>
  <td>Casella di controllo</td>
 </tr>
 <tr>
  <td>MSC E-mail selezionata</td>
  <td>Registra un segno di spunta quando il destinatario fa clic su un collegamento nell'e-mail</td>
  <td>Attività</td>
  <td>Casella di controllo</td>
 </tr>
 <tr>
  <td>Risposte e-mail MSC</td>
  <td>Registra un segno di spunta quando il destinatario risponde all'e-mail</td>
  <td>Attività</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>Stato e-mail MSC</td>
  <td>Mostra se un’e-mail viene inviata/in corso/rimbalzata (il tracciamento delle e-mail rimbalzate dipende dal canale di consegna utilizzato)</td>
  <td>Attività</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>Modello e-mail MSC</td>
  <td>Nome del registro del modello MSC utilizzato nell’e-mail inviata al lead/contatto</td>
  <td>Attività</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>URL modello e-mail MSC</td>
  <td>Registra l'URL del modello creato in MSC. Fai clic su questo pulsante per aprire il modello nell’app web MSC</td>
  <td>Attività</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>URL e-mail MSC</td>
  <td>Facendo clic su questo URL si aprirà il centro comandi in MSC e si aprirà la scheda Cronologia visualizzazione dettagli persone in cui l'utente può visualizzare l'e-mail inviata</td>
  <td>Attività</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>MSC E-mail visualizzata</td>
  <td>Registra un segno di spunta quando il destinatario visualizza un’e-mail</td>
  <td>Attività</td>
  <td>Casella di controllo</td>
 </tr>
</table>

<table>
 <tr>
  <th>Campo registrazione rollup MSC</th>
  <th>Descrizione</th>
  <th>Tipo</th>
  <th>Tipo di dati</th>
 </tr>
 <tr>
  <td>MSC - Ultimo impegno di marketing</td>
  <td>Ultimo coinvolgimento in arrivo da Marketing</td>
  <td>
  <p>Account
  <p>Contatto
  <p>Lead
  <p>Opportunità</td>
  <td>Dati e tempo</td>
 </tr>
 <tr>
  <td>MSC - Data ultimo coinvolgimento marketing</td>
  <td>Timestamp del coinvolgimento da Marketing</td>
  <td>
  <p>Account 
  <p>Contatto 
  <p>Lead 
  <p>Opportunità</td>
  <td>Dati e tempo</td>
 </tr>
 <tr>
  <td>MSC - Ultimo servizio di marketing</td>
  <td>Descrizione del coinvolgimento</td>
  <td>
  <p>Account 
  <p>Contatto 
  <p>Lead 
  <p>Opportunità</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>MSC - Ultima origine di coinvolgimento nel marketing</td>
  <td>Origine dell’impegno di marketing</td>
  <td>
  <p>Account 
  <p>Contatto 
  <p>Lead 
  <p>Opportunità</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>MSC - Ultimo tipo di coinvolgimento marketing</td>
  <td>Tipo di coinvolgimento (es: Attività web)</td>
  <td>
  <p>Account 
  <p>Contatto 
  <p>Lead 
  <p>Opportunità</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>MSC - Ultima attività per vendita</td>
  <td>Ultima attività in uscita eseguita dal team vendite</td>
  <td>
  <p>Account 
  <p>Contatto 
  <p>Lead 
  <p>Opportunità</td>
  <td>Dati e tempo</td>
 </tr>
 <tr>
  <td>MSC - Ultima risposta</td>
  <td>Ultima risposta e-mail alle vendite</td>
  <td>
  <p>Account 
  <p>Contatto 
  <p>Lead 
  <p>Opportunità</td>
  <td>Dati e tempo</td>
 </tr>
 <tr>
  <td>MSC - Campagna di vendita corrente</td>
  <td>Nome del registro della campagna MSC su cui si trova il contatto/lead</td>
  <td>
  <p>Account 
  <p>Contatto 
  <p>Lead 
  <p>Opportunità</td>
  <td>Testo</td>
 </tr>
 <tr>
  <td>MSC - Ultimo impegno di vendita</td>
  <td>Ultimo impegno in arrivo dalle vendite</td>
  <td>
  <p>Account
  <p>Contatto
  <p>Lead
  <p>Opportunità</td>
  <td>Dati e tempo</td>
 </tr>
 <tr>
  <td>MSC - Opt Out</td>
  <td>Campo Rinuncia</td>
  <td>
  <p>Account 
  <p>Contatto 
  <p>Lead 
  <p>Opportunità</td>
  <td>Casella di controllo</td>
 </tr>
</table>

<table>
 <tr>
  <th>Pulsanti MSC</th>
  <th>Descrizione</th>
  <th>Tipo</th>
 </tr>
 <tr>
  <td>Invia e-mail MSC</td>
  <td>Invia e-mail di vendita da Salesforce</td>
  <td>
  <p>Account 
  <p>Contatto 
  <p>Lead 
  <p>Opportunità</td>
 </tr>
 <tr>
  <td>Aggiungi alla campagna MSC</td>
  <td>Aggiungi a campagne MSC da Salesforce</td>
  <td>
  <p>Contatto
  <p>Lead</td>
 </tr>
 <tr>
  <td>Spingi a MSC</td>
  <td>Invia il contatto da Salesforce a MSC</td>
  <td>
  <p>Contatto
  <p>Lead</td>
 </tr>
 <tr>
  <td>Chiama con MSC</td>
  <td>Effettuare chiamate di vendita da Salesforce</td>
  <td>
  <p>Contatto
  <p>Lead</td>
 </tr>
</table>

<table>
 <tr>
  <th>Pulsanti di azione di massa MSC</th>
  <th>Descrizione</th>
  <th>Tipo</th>
 </tr>
 <tr>
  <td>Aggiungi alla campagna MSC</td>
  <td>Aggiungi a campagne MSC da Salesforce</td>
  <td>
  <p>Contatto
  <p>Lead</td>
 </tr>
 <tr>
  <td>Spingi a MSC</td>
  <td>Invia il contatto da Salesforce a MSC</td>
  <td>
  <p>Contatto
  <p>Lead</td>
 </tr>
 <tr>
  <td>Email con MSC</td>
  <td>Email con MSC da Salesforce</td>
  <td>
  <p>Contatto
  <p>Lead</td>
 </tr>
</table>
