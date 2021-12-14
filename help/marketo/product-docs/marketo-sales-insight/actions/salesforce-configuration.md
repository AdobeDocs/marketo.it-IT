---
description: Configurazione Salesforce - Documenti Marketo - Documentazione del prodotto
title: Configurazione Salesforce
hide: true
hidefromtoc: true
source-git-commit: 86b5fe66192490227c305e5d353454354496a274
workflow-type: tm+mt
source-wordcount: '1181'
ht-degree: 0%

---

# Configurazione Salesforce {#salesforce-configuration}

## Disinstallare il pacchetto di personalizzazione Salesforce (Classic) {#uninstall-salesforce-customization-package-classic}

Disinstalla il pacchetto Marketo Sales Connect dal tuo account Salesforce una volta che inizi a utilizzare il pacchetto MSI-Actions.

**Rimuovi campi di vendita Connect dal layout di pagina**

1. In Salesforce Classic, fai clic su **Configurazione**.

   ![](assets/salesforce-configuration-1.png)

1. Nella barra di navigazione a sinistra, nella sezione Genera, espandi (ma non fai clic su) Personalizza, quindi Lead. Quindi, seleziona **Layout di pagina**.

   ![](assets/salesforce-configuration-2.png)

1. Fai clic su **Modifica** accanto a Layout lead.

   ![](assets/salesforce-configuration-3.png)

1. Nella console, seleziona **Campi**. In Ricerca rapida, cerca &quot;MSC&quot;. Tutti i campi disattivati sono stati aggiunti al layout di pagina. Dovrai eliminarle.

   ![](assets/salesforce-configuration-4.png)

   >[!NOTE]
   >
   >Se nessuno dei campi è disabilitato, significa che non li hai aggiunti al layout di pagina. Puoi saltare questa sezione.

1. Scorri fino alla sezione con i campi personalizzati di vendita Connect.

   ![](assets/salesforce-configuration-5.png)

1. Ci sono 10 tipi di campi MSC che possono essere aggiunti a questa sezione. Rimuovi tutti i campi aggiunti o elimina semplicemente l’intera sezione.

1. Fai clic su **Salvataggio rapido** al termine.

   ![](assets/salesforce-configuration-6.png)

**Rimuovere i pulsanti di connessione alle vendite dai layout di pagina**

1. Nella console (passaggio 4 precedente), seleziona **Pulsanti**. Cerca &quot;MSC&quot;. Tutti i pulsanti disattivati sono stati aggiunti alla sezione dei pulsanti personalizzati. Dovrai eliminarle.

   ![](assets/salesforce-configuration-7.png)

   >[!NOTE]
   >
   >Se nessuno dei pulsanti è disabilitato, significa che non li hai aggiunti. Puoi saltare questa sezione.

1. Trascina i pulsanti MSC dalla sezione Pulsanti personalizzati alla console.

   ![](assets/salesforce-configuration-8.png)

1. Fai clic su **Salvataggio rapido** al termine.

   ![](assets/salesforce-configuration-9.png)

**Rimuovi campi di connessione vendite dalla sezione Cronologia attività**

1. Scorri fino alla parte inferiore della pagina, fino alla sezione dell’elenco relativo alla cronologia delle attività e fai clic sull’icona a forma di chiave inglese .

   ![](assets/salesforce-configuration-10.png)

1. Quindi, selezionare Campi di connessione vendite dall&#39;area Campi selezionati e fare clic sulla freccia Rimuovi. Fai clic su **OK** al termine.

   ![](assets/salesforce-configuration-11.png)

   >[!NOTE]
   >
   >L&#39;abbreviazione MSE _è_ Sales Connect È solo il nome precedente, &quot;Marketo Sales Engage&quot;.

1. Fai clic su **Salva** quando hai finito con la pagina Lead.

**Rimuovere i pulsanti di azione in blocco di vendita Connect dalla visualizzazione elenco lead**

1. Nella barra di navigazione a sinistra, nella sezione Genera, espandi (ma non fai clic su) Personalizza, quindi Lead. Quindi, seleziona **Layout di ricerca**.

   ![](assets/salesforce-configuration-12.png)

1. Accanto alla visualizzazione elenco Lead, fai clic su **Modifica**.

   ![](assets/salesforce-configuration-13.png)

1. Seleziona **Aggiungi alla campagna MSC (Classic)**, **E-mail con MSC (Classic)** e **Push to MSC (Classic)** e fare clic sulla freccia Rimuovi. Quindi fai clic su **Salva**.

   ![](assets/salesforce-configuration-14.png)

Non è più necessario visualizzare i pulsanti nella vista a elenco di lead.

**Rimuovi configurazione MSC per i contatti**

1. In Salesforce, fai clic su **Configurazione**.

1. Nella barra di navigazione a sinistra, in Genera, espandi (ma non fai clic su) Personalizza, quindi Contatti. Quindi, seleziona **Layout di pagina**.

1. Accanto a Layout contatto, fare clic su **Modifica**.

1. Ripetere i passaggi da tutte e tre le sezioni.

**Rimuovi configurazione MSC per opportunità**

1. In Salesforce, fai clic su **Configurazione**.

1. Nella barra di navigazione a sinistra, in Genera, espandi (ma non fai clic su) Personalizza, quindi Opportunità. Quindi, seleziona **Layout di pagina**.

1. Accanto a Layout opportunità, fare clic su **Modifica**.

1. Ripetere i passaggi da tutte e tre le sezioni.

La visualizzazione Opportunità dispone di un solo pulsante: &quot;Invia e-mail MSE&quot; e i campi seguenti:

![](assets/salesforce-configuration-15.png)

**Rimuovi configurazione MSC per account**

1. In Salesforce, fai clic su **Configurazione**.

1. Nella barra di navigazione a sinistra, in Genera, espandi (ma non fai clic su) Personalizza, quindi Account. Quindi, seleziona **Layout di pagina**.

1. Accanto al layout dell&#39;account, fai clic su **Modifica**.

1. Ripetere i passaggi da tutte e tre le sezioni.

La visualizzazione account ha un solo pulsante: &quot;Invia e-mail MSE&quot; e i campi seguenti:

![](assets/salesforce-configuration-16.png)

**Rimuovi casella in uscita vendite Marketo**

1. In Salesforce, fai clic sul pulsante **+** nella parte superiore dello schermo.

1. Fai clic su **Personalizzare le schede**.

1. Seleziona l’opzione Marketo Sales Outbox da destra. Fare clic sulla freccia Rimuovi, quindi fare clic su **Salva**.

**Elimina pacchetto di vendita**

Dopo aver rimosso tutti gli oggetti dal tuo account Salesforce, segui i passaggi seguenti.

1. In Salesforce, fai clic su **Configurazione**.

1. Nella casella Ricerca rapida immettere &quot;Classi Apex&quot;.

1. Fai clic su **Elimina** accanto a tutte le voci &quot;MarketoSalesConnectionCustomization&quot; o &quot;MarketoSalesEngageCustomization&quot; nell’elenco.

Sei pronto!

Elenco di tutti gli oggetti che devono essere rimossi dall’istanza Salesforce:

**Dettagli sulla personalizzazione di Sales Connect**

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
  <td>Aggiungi alla campagna MSC (Classic)</td>
  <td>Aggiungi a campagne MSC da Salesforce</td>
  <td>
  <p>Contatto
  <p>Lead</td>
 </tr>
 <tr>
  <td>Push to MSC (Classic)</td>
  <td>Invia il contatto da Salesforce a MSC</td>
  <td>
  <p>Contatto
  <p>Lead</td>
 </tr>
 <tr>
  <td>E-mail con MSC (Classic)</td>
  <td>Email con MSC da Salesforce</td>
  <td>
  <p>Contatto
  <p>Lead</td>
 </tr>
</table>
