---
unique-page-id: 2360368
description: Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited - Marketo Docs - Documentazione del prodotto
title: Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
source-git-commit: 854bbc3642d52e670e0e55e6660ea85661edf904
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 0%

---

# Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Di seguito sono riportati i passaggi da effettuare per configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited Edition. Cominciamo.

>[!PREREQUISITES]
>
>[Installa il pacchetto Marketo Sales Insight in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Configurare la funzione Approfondimenti vendite in Marketo {#configure-sales-insight-in-marketo}

1. Ottieni le tue credenziali MSI in Marketo. Vai all’area Amministratore e seleziona **Approfondimenti vendite**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Fai clic su **Modifica configurazione API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Immetti una chiave segreto API a tua scelta e fai clic su **Salva**. NON utilizzare una e commerciale (&amp;) nella chiave segreto API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >La chiave di segreto API è una password per la tua organizzazione e deve essere protetta.

1. Fai clic su **Visualizza** nel pannello Configurazione API REST per popolare le credenziali.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Verrà visualizzato un pop-up di conferma. Fai clic su **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Tieni aperta questa finestra. Queste informazioni saranno necessarie più avanti a Salesforce.

## Configurazione di Sales Insight in Salesforce {#configure-sales-insight-in-salesforce}

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Cerca &quot;sito remoto&quot; e seleziona **Impostazioni del sito remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Fai clic su **Nuovo sito remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Inserisci il Nome del sito remoto (può essere simile a &quot;MarketoSoapAPI&quot;). Inserisci URL del sito remoto, che è l’URL host Marketo dal pannello Configurazione API Soap in Marketo. Fai clic su **Salva**. Ora hai creato le impostazioni del sito remoto per l’API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Fai clic su **Nuovo sito remoto** di nuovo.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Inserisci il Nome del sito remoto (può essere simile a &quot;MarketoAPI&quot;). Inserisci URL del sito remoto, che è l’URL API dal pannello Configurazione API di ripristino in Marketo. Fai clic su **Salva**. Sono state create le impostazioni del sito remoto per l’API di ripristino.

   >[!NOTE]
   >
   >_You_ scegli la tua **Nome del sito remoto** (MarketoAPI viene utilizzato qui). La **URL sito remoto** Si trova nel campo Host Marketo della finestra di dialogo Modifica configurazione API dal passaggio 3 nella sezione &quot;Configura informazioni sulle vendite in Marketo&quot;.

## Personalizzare i layout di pagina {#customize-page-layouts}

1. Fai clic su **Configurazione**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Cerca &quot;layout pagina&quot; e seleziona il **Layout pagina** sotto **Lead**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Fai clic su **Pagine della visualizzazione** a sinistra. Trascina **Sezione** al layout nella sezione Collegamenti personalizzati .

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Inserisci &quot;Marketo Sales Insight&quot; come **Nome sezione**. Seleziona **1 colonna** e fai clic su **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Trascinamento della selezione **Lead** nella nuova sezione.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Il nome di questa casella verrà modificato in base al tipo di oggetto. Ad esempio, se si modifica il layout di pagina per Contatti, verrà visualizzato Contatto.

1. Fai doppio clic sul pulsante **Lead** blocco appena aggiunto.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Modifica altezza in **450** pixel e fai clic su **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Controlla **Mostra barre di scorrimento** se hai bisogno di accedere alle attività di scorrimento.

   >[!TIP]
   >
   >È consigliabile un&#39;altezza di 410 pixel per gli oggetti Account e Opportunità.

1. Fai clic su **Campi** a sinistra. Quindi cerca e trascina il **Urgenza** nella **Informazioni sulle vendite Marketo** layout.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. Ripetere il passaggio precedente anche per questi campi.

   <table> 
    <tbody> 
     <tr> 
      <td>Ultimo momento interessante</td> 
     </tr> 
     <tr> 
      <td>Data ultimo momento interessante</td> 
     </tr> 
     <tr> 
      <td>Desc dell'ultimo momento interessante</td> 
     </tr> 
     <tr> 
      <td>Ultima origine momento interessante</td> 
     </tr> 
     <tr> 
      <td>Ultimo tipo di momento interessante</td> 
     </tr> 
     <tr> 
      <td>Ultima attività Marketo per vendite</td> 
     </tr> 
     <tr> 
      <td>Ultimo coinvolgimento Marketo per vendite</td> 
     </tr> 
     <tr> 
      <td>ID contatto MSI</td> 
     </tr> 
     <tr> 
      <td>Punteggio relativo</td> 
     </tr> 
     <tr> 
      <td>Valore punteggio relativo</td> 
     </tr> 
     <tr> 
      <td>Urgenza</td> 
     </tr> 
     <tr> 
      <td>Valore di urgenza</td> 
     </tr> 
     <tr> 
      <td>Visualizza in Marketo</td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva** una volta finito.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Ripetere i passaggi da 5 a 7 per aggiungere sezioni della pagina Visualforce e campi Approfondimenti vendite per **Contatto**, **Account** e **Opportunità**.

1. Ripetere i passaggi 8-10 per aggiungere campi Approfondimenti vendite dall&#39;elenco sottostante per **Contatto**. Assicurati di salvare eventuali modifiche.

<table> 
    <tbody> 
     <tr> 
      <td>Ultimo momento interessante</td> 
     </tr> 
     <tr> 
      <td>Data ultimo momento interessante</td> 
     </tr> 
     <tr> 
      <td>Desc dell'ultimo momento interessante</td> 
     </tr> 
     <tr> 
      <td>Ultima origine momento interessante</td> 
     </tr> 
     <tr> 
      <td>Ultimo tipo di momento interessante</td> 
     </tr> 
     <tr> 
      <td>Ultima attività Marketo per vendite</td> 
     </tr> 
     <tr> 
      <td>Ultimo coinvolgimento Marketo per vendite</td> 
     </tr> 
     <tr> 
      <td>Punteggio lead MKTO</td> 
     </tr> 
     <tr> 
      <td>Punteggio relativo</td> 
     </tr> 
     <tr> 
      <td>Valore punteggio relativo</td> 
     </tr> 
     <tr> 
      <td>Insight vendite: apre la pagina completa dell'elenco dei contatti</td> 
     </tr> 
     <tr> 
      <td>Urgenza</td> 
     </tr> 
     <tr> 
      <td>Valore di urgenza</td> 
     </tr> 
    </tbody> 
   </table>

## Mappa campi persona personalizzati {#map-custom-person-fields}

I campi persona di Marketo devono essere mappati sui campi contatto di Salesforce per garantire il corretto funzionamento della conversione. Ecco come.

1. Fai clic su **Configurazione**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Cerca &quot;campi&quot; nella barra di ricerca e fai clic su **Campi** sotto **Lead**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Fai clic su **Mappa campi lead**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Fai clic sul menu a discesa a destra di **Coinvolgimento**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Seleziona **Contact.Engagement** nell&#39;elenco.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Ripeti e mappa anche questi campi.

   <table> 
    <tbody> 
     <tr> 
      <th colspan="1" rowspan="1">Campo personalizzato persona Marketo</th> 
      <th colspan="1" rowspan="1">Campo personalizzato contatto Salesforce</th> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Coinvolgimento</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Valore punteggio relativo</p></td> 
      <td colspan="1" rowspan="1"><p>Valore punteggio relativo di Contact.Relative</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Valore di urgenza</p></td> 
      <td colspan="1" rowspan="1"><p>Valore Contact.Urency</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Data ultimo momento interessante</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interessante Momento Data</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Desc dell'ultimo momento interessante</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interessante Momento Desc</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Ultima origine momento interessante</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interessante Momento Origine</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Ultimo tipo di momento interessante</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interessante Moment Type</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva** quando hai finito.

## Scheda Configurazione di Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. In Salesforce, fai clic sul pulsante **+** alla fine della barra delle schede e fai clic su **Configurazione di Marketo Sales Insight**.

1. Copia le credenziali dal pannello API Soap in [Pagina Marketo Sales Insight Admin](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target=&quot;_blank&quot;} e incollali nella sezione API Soap della pagina Configurazione approfondimenti vendite Salesforce.

1. Copia le credenziali dal pannello Rest API in [Pagina Marketo Sales Insight Admin](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target=&quot;_blank&quot;} e incollali nella sezione Rest API della pagina Salesforce Sales Insight Configuration.

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

Ed è tutto! È necessario essere in grado di visualizzare i campi Marketo Sales Insight per Lead, Contatti, Account e Opportunità.

>[!NOTE]
>
>Se il test di diagnostica non è riuscito, potrebbe essere necessario [aggiungere altri campi al layout della pagina](https://nation.marketo.com/docs/DOC-1115){target=&quot;_blank&quot;}.

>[!NOTE]
>
>Per gli account, Insight vendite includerà tutte le e-mail, ma solo i momenti interessanti più recenti, l’attività web e i cambiamenti di punteggio.

>[!MORELIKETHIS]
>
>* [Priorità, Urgenza, Punteggio relativo e Migliori offerte](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Aggiungi scheda Marketo a Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Aggiungi accesso a informazioni sulle vendite nei profili](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;}

