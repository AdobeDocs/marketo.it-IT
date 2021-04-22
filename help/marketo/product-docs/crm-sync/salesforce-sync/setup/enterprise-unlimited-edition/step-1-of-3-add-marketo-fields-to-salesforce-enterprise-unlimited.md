---
unique-page-id: 2360362
description: Passaggio 1 di 3 - Aggiungere campi Marketo a Salesforce (Enterprise/Unlimited) - Marketo Docs - Documentazione del prodotto
title: Passaggio 1 di 3 - Aggiungere campi Marketo a Salesforce (Enterprise/Senza limiti)
exl-id: bcfba281-0d4b-42c3-b52a-ce1c3da884ba
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 0%

---

# Passaggio 1 di 3: Aggiungi campi Marketo a Salesforce (Enterprise/Senza limiti) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>Devi disporre dell’accesso alle API Salesforce per la sincronizzazione tra Marketo e Salesforce.

Marketo utilizza un set di campi per acquisire alcuni tipi di informazioni relative al marketing. Se desideri questi dati in Salesforce, segui le istruzioni riportate di seguito.

1. Crea tre campi personalizzati in Salesforce sugli oggetti lead e contact : Punteggio, programma di acquisizione e data di acquisizione.
1. Mappa questi campi personalizzati tra lead e contatti in modo che, al momento della conversione in Salesforce, i valori vengano riportati.
1. Se necessario, puoi creare altri campi aggiuntivi (vedi la tabella seguente).

Tutti questi campi personalizzati sono facoltativi e non sono necessari per sincronizzare Marketo e Salesforce. È consigliabile creare campi per Punteggio, Programma di acquisizione e Data di acquisizione.

## Aggiungi campi Marketo a Salesforce {#add-marketo-fields-to-salesforce}

Aggiungi tre campi personalizzati sugli oggetti lead e contact in Salesforce elencati sopra. Per ulteriori informazioni, consulta la tabella dei campi disponibili alla fine di questa sezione.

Esegui i seguenti passaggi per ciascuno dei tre campi personalizzati per aggiungerli. Inizia con Punteggio.

1. Accedi a Salesforce e fai clic su **Configurazione**.

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. Nel menu Genera a sinistra, fai clic su **Personalizza** e seleziona **Lead**. Fare clic su **Campi**.

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. Fai clic su **Nuovo** nella sezione Campi personalizzati e correlazioni nella parte inferiore della pagina.

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. Scegliere il tipo di campo appropriato (per Punteggio — numero; Programma di acquisizione — testo; Data acquisizione — Data/Ora).

   ![](assets/choose-field-type-2-hand.png)

1. Fare clic su **Avanti**.

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. Immetti Etichetta campo, Lunghezza e Nome campo per il campo, come illustrato nella tabella seguente.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Etichetta campo 
    </div></th> 
   <th> 
    <div>
      Nome campo 
    </div></th> 
   <th> 
    <div>
      Tipo di dati 
    </div></th> 
   <th> 
    <div>
      Attributi del campo 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Punteggio</td> 
   <td>mkto71_Lead_Score</td> 
   <td>Numero</td> 
   <td>Lunghezza 10<br>Posizioni decimali 0 </td> 
  </tr> 
  <tr> 
   <td>Data acquisizione</td> 
   <td>mkto71_Acquisition_Date</td> 
   <td>Data/ora</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programma di acquisizione</td> 
   <td>mkto71_Acquisition_Program</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Salesforce aggiunge __c ai nomi dei campi quando li utilizza per creare nomi API.

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>I campi di testo e numerici richiedono una lunghezza, ma non i campi data/ora. Una descrizione è facoltativa.

1. Fare clic su **Avanti**.

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. Specifica le impostazioni di accesso e fai clic su **Avanti**:

   * Imposta tutti i ruoli su **Visibile** e **Solo lettura**

   * Deseleziona la casella di controllo **Sola lettura** per il profilo dell&#39;utente di sincronizzazione:

      * Se si dispone di un utente con il profilo di un _amministratore di sistema_ come utente di sincronizzazione, deselezionare la casella di controllo **Sola lettura** per il profilo Amministratore di sistema (come mostrato di seguito)
      * Se hai creato un _profilo personalizzato_ per l&#39;utente di sincronizzazione, deseleziona la casella di controllo **Sola lettura** per tale profilo personalizzato

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. Scegliere i layout di pagina da visualizzare nel campo.

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. Fai clic su **Salva e nuovo** per tornare indietro e creare ciascuno degli altri due campi personalizzati. Fai clic su **Salva** per completare l&#39;operazione con tutte e tre le opzioni.

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. Nel menu Genera a sinistra, fai clic su **Personalizza** e seleziona Contatti. Fare clic su Campi.
1. Esegui i passaggi da 3 a 10 per i campi Punteggio, Data acquisizione e Programma di acquisizione sull’oggetto contatto, proprio come per l’oggetto lead.
1. Facoltativamente, utilizza la procedura precedente per tutti i campi personalizzati aggiuntivi di questa tabella.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Etichetta campo 
    </div></th> 
   <th> 
    <div>
      Nome campo 
    </div></th> 
   <th> 
    <div>
      Tipo di dati 
    </div></th> 
   <th> 
    <div>
      Attributi del campo 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID del programma di acquisizione</td> 
   <td>mkto71_Acquisition_Program_Id</td> 
   <td>Numero</td> 
   <td>Lunghezza 18<br>Posizioni decimali 0 </td> 
  </tr> 
  <tr> 
   <td>Referrer originale</td> 
   <td>mkto71_Original_Referrer</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Motore di ricerca originale</td> 
   <td>mkto71_Original_Search_Engine</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Frase di ricerca originale</td> 
   <td>mkto71_Original_Search_Phrase</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Informazioni origine originali</td> 
   <td>mkto71_Original_Source_Info</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Tipo di origine originale</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Città di riferimento</td> 
   <td>mkto71_Inferred_City</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Azienda in oggetto</td> 
   <td>mkto71_Inferred_Company</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Paese in oggetto</td> 
   <td>mkto71_Inferred_Country</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Area metropolitana</td> 
   <td>mkto71_Inferred_Metropolitan_Area</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Codice di area del telefono</td> 
   <td>mkto71_Inferred_Phone_Area_Code</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Codice postale trasferito</td> 
   <td>mkto71_Inferred_Postal_Code</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Regione dello Stato di provenienza</td> 
   <td>mkto71_Inferred_State_Region</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
 </tbody> 
</table>

## Mappa campi personalizzati per le conversioni {#map-custom-fields-for-conversions}

Un campo personalizzato sull’oggetto lead di Salesforce deve essere mappato su un campo contatto dell’oggetto contatto in modo che i dati vengano trasferiti quando si verifica una conversione.

1. Nell&#39;angolo in alto a destra, fai clic su **Configurazione**.

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. Digitare &quot;Fields&quot; nella ricerca di navigazione senza premere Invio. I campi sono visualizzati sotto oggetti diversi; Fai clic su **Campi** in Lead.

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. Vai alla sezione Campi personalizzati lead e correlazioni e fai clic su **Mappa campi lead**.

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. Fai clic sull’elenco a discesa accanto al campo da mappare.

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. Seleziona il campo personalizzato del contatto corrispondente.

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. Ripeti i passaggi precedenti per tutti gli altri campi creati.

1. Al termine, fai clic su **Salva**.

   Abbastanza facile, vero?

>[!MORELIKETHIS]
>
>[Passaggio 2 di 3: Creare un utente Salesforce per Marketo (Enterprise/Senza limiti)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
