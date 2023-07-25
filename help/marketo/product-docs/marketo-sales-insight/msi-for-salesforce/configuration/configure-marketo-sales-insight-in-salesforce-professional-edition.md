---
unique-page-id: 3571743
description: Configurare Marketo Sales Insight in Salesforce Professional Edition - Documentazione Marketo - Documentazione del prodotto
title: Configurare Marketo Sales Insight in Salesforce Professional Edition
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 0%

---

# Configurare Marketo Sales Insight in Salesforce Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Ecco i passaggi da seguire per configurare Marketo Sales Insight in Salesforce Professional Edition. Cominciamo.

>[!PREREQUISITES]
>
>* Installa Marketo nella tua Salesforce Professional Edition.
>
>* [Installare il pacchetto Marketo Sales Insight nell’AppExchange di Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Configurare Sales Insight in Marketo {#configure-sales-insight-in-marketo}

1. Apri una nuova finestra del browser per ottenere le credenziali di Marketo Sales Insight dal tuo account Marketo.
1. Vai all’area Amministratore e seleziona **Insight sulle vendite**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Clic **Modifica configurazione API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Inserisci una chiave segreta API a tua scelta e fai clic su **Salva**. NON utilizzare una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >La chiave segreta API è una password per la tua organizzazione e deve essere sicura.

1. Clic **Visualizza** nel pannello Configurazione API REST per compilare le credenziali.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Viene visualizzata una finestra a comparsa di conferma. Clic **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Configurare Sales Insight in Salesforce {#configure-sales-insight-in-salesforce}

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Cercare &quot;sito remoto&quot; e selezionare **Impostazioni sito remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Clic **Nuovo sito remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Immetti il nome del sito remoto (può essere ad esempio &quot;MarketoSoapAPI&quot;). Immetti l’URL del sito remoto, che è l’URL dell’host Marketo dal pannello Configurazione API Soap in Marketo. Clic **Salva**. Sono state create le impostazioni del sito remoto per l’API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Clic **Nuovo sito remoto** di nuovo.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Immetti il nome del sito remoto (può essere ad esempio &quot;MarketoRestAPI&quot;). Immetti l’URL del sito remoto, che è l’URL dell’API dal pannello Configurazione API REST in Marketo. Clic **Salva**. Sono state create le impostazioni del sito remoto per l’API REST.

## Configurare Marketo Sales Insight {#set-up-marketo-sales-insight}

1. Accedi all’istanza di Marketo e fai clic su **Amministratore**.

   ![](assets/login-admin-1.png)

1. Clic **Insight sulle vendite**.

   ![](assets/image2015-5-22-15-3a12-3a33-1.png)

1. Clic **Modifica configurazione API**.

   ![](assets/image2015-5-22-15-3a15-3a0-1.png)

1. Immetti un **Chiave segreta API** e fai clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzare una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2015-5-27-16-3a36-3a56-1.png)

   >[!TIP]
   >
   >Tieni aperta questa finestra. Queste informazioni saranno necessarie più avanti in Salesforce.

1. Torna a Salesforce, fai clic su **Configurazione**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Cercare &quot;sito remoto&quot; e fare clic su **Impostazione sito remoto** in **Controlli di sicurezza**.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Clic **Nuovo sito remoto**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Invio **Nome sito remoto** e **URL sito remoto**, quindi fai clic su **Salva**.

   ![](assets/remote-site-1.png)

   >[!NOTE]
   >
   >Scegli il tuo **Nome sito remoto** (MarketoAPI viene utilizzato qui). Il **URL sito remoto** sono disponibili nel campo Host Marketo della finestra di dialogo Modifica configurazione API dal passaggio 4.

## Personalizza layout di pagina {#customize-page-layouts}

1. Clic **Configurazione**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Cerca &quot;layout di pagina&quot; e seleziona la **Layout di pagina** in **Lead**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. Clic **Visualforce Pages** a sinistra. Trascina **Sezione** al layout sotto la sezione Collegamenti personalizzati.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Immetti &quot;Marketo Sales Insight&quot; come **Nome sezione**. Seleziona **1 colonna** e fai clic su **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Trascina **Lead** nella nuova sezione.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Il nome di questa casella verrà modificato in base al tipo di oggetto. Se ad esempio si modifica il layout di pagina per i contatti, verrà visualizzato Contatto.

1. Fai doppio clic sul pulsante **Lead** blocco appena aggiunto.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Modifica altezza in **450** pixel e fai clic su **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Verifica **Mostra barre di scorrimento** se hai bisogno di accedere alle attività di scorrimento.

   >[!TIP]
   >
   >È consigliabile un&#39;altezza di 410 pixel per gli oggetti Account e Opportunità.

1. Fai clic su **Campi** a sinistra. Quindi cerca e trascina il **Coinvolgimento** etichetta in **Insight sulla vendita di Marketo** layout.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. Ripeti il passaggio precedente anche per questi campi.

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">Coinvolgimento</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valore punteggio relativo</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valore Urgenza</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Data ultimo momento di interesse</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Descrizione ultimo momento di interesse</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Sorgente ultimo momento di interesse</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Tipo ultimo momento di interesse</p></td> 
  </tr> 
 </tbody> 
</table>

1. Clic **Salva** al termine.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Ripetete questa procedura per aggiungere sezioni di pagina e campi di approfondimento vendite di Visualforce per **Contatto**, **Account** e **opportunità**.
1. Ripeti i passaggi 5-7 per aggiungere sezioni di pagina Visualforce per Contatto, Account e Opportunità. Quindi, ripeti i passaggi 8-10 per aggiungere i campi Sales Insight per **Contatto**. Assicurati di salvare dopo eventuali modifiche.

## Mappa campi persona personalizzati {#map-custom-person-fields}

I campi persona di Marketo devono essere mappati sui campi contatto Salesforce per garantire il corretto funzionamento della conversione. Ecco come.

1. Clic **Configurazione**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Cerca i &quot;campi&quot; nella barra di ricerca e fai clic su **Campi** in **Lead**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Clic **Mappa campi lead**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Fai clic sul menu a discesa a destra per **Coinvolgimento**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Seleziona **Contact.Engagement** nell&#39;elenco.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

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
   <td colspan="1" rowspan="1"><p>Valore punteggio relativo Contact.Relative</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valore Urgenza</p></td> 
   <td colspan="1" rowspan="1"><p>Valore Contact.Urgency</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Data ultimo momento di interesse</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Date</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Descrizione ultimo momento di interesse</p></td> 
   <td colspan="1" rowspan="1"><p>Descrizione Momento Di Interesse Contact.Last</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Sorgente ultimo momento di interesse</p></td> 
   <td colspan="1" rowspan="1"><p>Origine momento di interesse Contact.Last</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Tipo ultimo momento di interesse</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Type</p></td> 
  </tr> 
 </tbody> 
</table>

1. Clic **Salva** quando hai finito.

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Scheda Configurazione di Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. In Salesforce, fai clic su **+** alla fine della barra delle schede e fare clic su **Configurazione approfondimento vendite Marketo**.

1. Copiare le credenziali dal pannello API Soap in [Pagina di amministrazione di Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} e incollali nella sezione API Soap della pagina Configurazione di Salesforce Sales Insight.

1. Copiare le credenziali dal pannello API Rest in [Pagina di amministrazione di Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} e incollali nella sezione API Rest della pagina Configurazione di Salesforce Sales Insight.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

Ed è tutto! Dovresti essere in grado di visualizzare i campi Insight vendite Marketo per lead, contatti, account e opportunità.

>[!NOTE]
>
>Se il test di diagnostica non è riuscito, potrebbe essere necessario [aggiungi altri campi al layout della pagina](https://nation.marketo.com/docs/DOC-1115){target="_blank"}.

>[!NOTE]
>
>Per gli account, Sales Insight includerà tutte le e-mail, ma solo i momenti di interesse più recenti, l’attività web e le modifiche dei punteggi.

>[!MORELIKETHIS]
>
>* [Priorità, urgenza, punteggio relativo e elementi di maggiore rilevanza](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [Aggiungi scheda Marketo a Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [Aggiungere l’accesso a Sales Insight ai profili](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
