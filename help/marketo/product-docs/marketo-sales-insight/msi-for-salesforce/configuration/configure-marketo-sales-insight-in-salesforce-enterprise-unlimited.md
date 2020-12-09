---
unique-page-id: 2360368
description: Configurare il marketing Sales Insight in Salesforce Enterprise/Unlimited - Marketo Docs - Documentazione prodotto
title: Configurare Marketing Sales Insight in Salesforce Enterprise/Unlimited
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---


# Configurare Marketing Sales Insight in Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Di seguito sono descritti i passaggi da effettuare per configurare Marketing Cloud Sales Insight in Salesforce Enterprise/Unlimited Edition. Cominciamo.

>[!PREREQUISITES]
>
>* [Configurare la sincronizzazione dei campi Marketo nella versione Salesforce Enterprise/Unlimited Edition](http://docs.marketo.com/pages/viewpage.action?pageid=2360372)
>* [Installazione del pacchetto marketing Sales Insight in Salesforce  AppExchange](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>



>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Configurare Sales Insight in Marketo {#configure-sales-insight-in-marketo}

1. Aprite una nuova finestra del browser per ottenere le credenziali di Marketing to Sales Insight dal vostro account Marketo.
1. Vai all&#39;area Admin e seleziona **Sales Insight**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Fate clic su **Modifica configurazione** API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Immettete una chiave segreta API di vostra scelta e fate clic su **Salva**. NON utilizzate una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >La chiave segreta API è come una password per l&#39;organizzazione e deve essere protetta.

1. Fate clic su **Visualizza** nel pannello Configurazione API rimanente per compilare le credenziali.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Verrà visualizzato un messaggio di conferma. Fate clic su **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

## Configurare l&#39;analisi delle vendite in Salesforce {#configure-sales-insight-in-salesforce}

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Cercate &quot;sito remoto&quot; e selezionate Impostazioni **sito** remoto.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Fate clic su **Nuovo sito** remoto.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Inserite il Nome del sito remoto (può essere simile a &quot;MarketoSoapAPI&quot;). Inserite l&#39;URL del sito remoto, che è l&#39;URL dell&#39;host Marketo dal pannello Configurazione API Soap in Marketo. Fate clic su **Salva**. Ora avete creato le impostazioni del sito remoto per l&#39;API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Fate di nuovo clic su **Nuovo sito** remoto.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Immettete il nome del sito remoto (può essere simile a &quot;MarketoRestAPI&quot;). Inserite URL sito remoto, che è l&#39;URL API dal pannello Configurazione API di ripristino in Marketo. Fate clic su **Salva**. Sono state create impostazioni del sito remoto per l&#39;API Rest.

## Imposta analisi vendite Marketo {#set-up-marketo-sales-insight}

1. Accedi all’istanza di Marketo e fai clic su **Admin**.

   ![](assets/login-admin.png)

1. Fare clic su** Insight vendite**.

   ![](assets/image2015-5-22-15-3a12-3a33.png)

1. Fate clic su **Modifica configurazione** API.

   ![](assets/image2015-5-22-15-3a15-3a0.png)

1. Immettete una chiave **segreta** API e fate clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzate una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2015-5-27-16-3a36-3a56.png)

   >[!TIP]
   >
   >Tieni questa finestra aperta. Queste informazioni saranno necessarie più tardi in Salesforce.

1. Torna a Salesforce, fai clic su **Configurazione**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Cercate &quot;sito remoto&quot; e fate clic su Impostazioni **sito** remoto in **Controlli** di sicurezza.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Fate clic su **Nuovo sito** remoto.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Immettete Nome **sito** remoto e URL **sito** remoto, quindi fate clic su **Salva**.

   ![](assets/remote-site.png)

   >[!NOTE]
   >
   >Scegliete il nome **del sito** remoto (qui viene utilizzata l’API Marketo). L&#39;URL **del sito** remoto si trova nel campo Host di Marketo della finestra di dialogo Modifica configurazione API dal Passaggio 4.

## Personalizzare i layout di pagina {#customize-page-layouts}

1. Fate clic su **Configurazione**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Cercate &quot;layout di pagina&quot; e selezionate il layout **di** pagina in **Lead**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Fare clic su **Visualforce Pages **a sinistra. Trascinate **Sezione** sul layout sotto la sezione Collegamenti personalizzati.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Immettete &quot;Visione vendite marketing&quot; come nome **** sezione. Selezionate **1 colonna** e fate clic su **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Trascina **lead** nella nuova sezione.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Il nome di questa casella viene modificato in base al tipo di oggetto. Ad esempio, se modificate il layout della pagina per Contatti, verrà visualizzato Contatto.

1. Fare doppio clic sul blocco **Lead** appena aggiunto.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Modificate l’altezza a **450** pixel e fate clic su **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >È consigliabile un&#39;altezza di 410 pixel per gli oggetti Account e Opportunità.

1. Fare clic su **Fields **a sinistra. Quindi, cercate e trascinate l&#39;etichetta **Partecipazione** nel layout **Visione** vendite di Marketing.

   ![](assets/image2015-5-22-16-3a32-3a46.png)

1. Ripetere il passaggio precedente anche per questi campi.

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">Coinvolgimento</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valore punteggio relativo</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valore di urgenza</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Data ultimo momento interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Ultimo interessante momento</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Ultima origine momento interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Ultimo tipo di momento interessante</p></td> 
  </tr> 
 </tbody> 
</table>

1. Al termine, fate clic su **Salva** .

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Ripetete questa procedura per aggiungere le sezioni delle pagine Visualforce e i campi Vendite Insight per **Contatto**, **Account** e **Opportunità**.
1. Ripetere i passaggi da 5 a 7 per aggiungere le sezioni delle pagine di Visualforce per Contatto, Account e Opportunità. Quindi, ripeti i passaggi da 8 a 10 per aggiungere i campi Informazioni sulle vendite per il **contatto**. Accertatevi di salvare dopo eventuali modifiche.

## Mappa campi persona personalizzati {#map-custom-person-fields}

I campi persona marketing devono essere mappati sui campi di contatto Salesforce per garantire il corretto funzionamento della conversione. Ecco come.

1. Fate clic su **Configurazione**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Cercate &quot;campi&quot; nella barra di ricerca e fate clic su **Campi** in **Lead**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Fate clic su **Mappa campi** lead.

   ** ![](assets/image2015-6-1-9-3a58-3a48.png)

   **

1. Fate clic sul menu a discesa a destra per **Partecipazione**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Selezionare **Contact.Engagement **nell&#39;elenco.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Ripetete e mappate anche questi campi.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1">Campo personalizzato Marketo Person</th> 
   <th colspan="1" rowspan="1">Campo personalizzato contatto Salesforce</th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Coinvolgimento</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valore punteggio relativo</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Relative Score Value</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valore di urgenza</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Urency Value</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Data ultimo momento interessante</p></td> 
   <td colspan="1" rowspan="1"><p>Contatto.Data ultimo momento interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Ultimo interessante momento</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interessante Momento Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Ultima origine momento interessante</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interesting Moment Source</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Ultimo tipo di momento interessante</p></td> 
   <td colspan="1" rowspan="1"><p>Contatto.Ultimo tipo di momento interessante</p></td> 
  </tr> 
 </tbody> 
</table>

1. Fare clic su **Save **al termine.

## Configurazione analisi vendite Marketo {#marketo-sales-insight-config}

1. Fare clic su **+ **e quindi selezionare Configurazione **analisi vendite** Marketo.

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. Selezionate **Abilita API** Marketo. Quindi compila le informazioni di configurazione [API in Amministratore](http://docs.marketo.com/display/DOCS/Configure+Marketo+Sales+Insight+in+Salesforce+Professional+Edition#ConfigureMarketoSalesInsightinSalesforceProfessionalEdition-SetupMarketoSalesInsight)Marketo. Fare clic su **Salva modifiche **al termine.

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >Se il test di diagnostica non riesce, potrebbe essere necessario [aggiungere altri campi al layout](http://nation.marketo.com/docs/DOC-1115)della pagina.

Ed è tutto! È necessario essere in grado di visualizzare i campi Visione marketing per lead, contatti, account e opportunità.

![](assets/twenty-six.png)

>[!NOTE]
>
>Per gli account, Sales Insight includerà tutte le e-mail, ma solo i momenti interessanti più recenti, l&#39;attività Web e le modifiche alla valutazione.

## Accesso al punto vendita di Marketo {#access-marketo-sales-insight}

1. In Salesforce, fai clic su **+** alla fine della barra delle schede, quindi fai clic su Configurazione **analisi vendite** Marketo.
1. Selezionate la casella di controllo **Abilita API** marketing.
1. Copiate le credenziali dal pannello API Soap nella pagina Admin di Marketing’s Sales Insight e incollatele nella sezione API Soap della pagina Configurazione di Salesforce Sales Insight.
1. Copiate le credenziali dal pannello Rest API nella pagina Admin di Marketing’s Sales Insight e incollatele nella sezione Rest API della pagina Configurazione Salesforce Sales Insight.

   ![](assets/access-msi.png)

>[!NOTE]
>
>**Articoli correlati**
>
>* [Priorità, Urgenza, Punteggio relativo e migliori risultati](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Aggiungi la scheda Marketing Sales Insight e i pulsanti a Salesforce](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)

>



