---
unique-page-id: 11372975
description: Passaggio 1 di 3 - Aggiungi i campi Marketo a Salesforce (Professional) - Marketo Docs - Documentazione prodotto
title: Passaggio 1 di 3 - Aggiungi i campi Marketo a Salesforce (Professional)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---


# Passaggio 1 di 3: Aggiungi campi Marketo a Salesforce (Professional) {#step-of-add-marketo-fields-to-salesforce-professional}

>[!PREREQUISITES]
>
>L’istanza Salesforce deve avere accesso alle API Salesforce per sincronizzare i dati tra Marketo e Salesforce.

Marketo utilizza un set di campi per acquisire alcuni tipi di informazioni relative al marketing. Se desideri che questi dati siano disponibili in Salesforce, segui le istruzioni riportate di seguito.

1. Crea tre campi personalizzati in Salesforce sugli oggetti lead e di contatto: Punteggio, programma di acquisizione e data di acquisizione.
1. Mappa questi campi personalizzati tra lead e contatti in modo che alla conversione in Salesforce, i valori vengano riportati.
1. Se necessario, potete creare altri campi (vedere la tabella di seguito).

Tutti questi campi personalizzati sono facoltativi e non sono necessari per sincronizzare Marketo e Salesforce. Come procedura ottimale, ti consigliamo di creare campi per Valutazione, Programma di acquisizione e Data di acquisizione.

## Aggiungi campi Marketo a Salesforce {#add-marketo-fields-to-salesforce}

Aggiungi tre campi personalizzati al lead e agli oggetti di contatto in Salesforce elencati sopra. Per aggiungere di più, vedere la tabella dei campi disponibili alla fine di questa sezione.

Effettuare le seguenti operazioni per ciascuno dei tre campi personalizzati per aggiungerli. Iniziate con **Punteggio**.

1. Accedete a Salesforce e fate clic su **Configurazione.**

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. Nel menu Genera a sinistra, fate clic su **Personalizza** e selezionate **Lead**. Fare clic su **Campi**.

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. Fare clic su **Nuovo** nella sezione Campi e relazioni personalizzati nella parte inferiore della pagina.

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. Scegliete il tipo di campo appropriato (per Punteggio — **number**; Programma di acquisizione — **text**; Data acquisizione — **Data/Ora**).

   ![](assets/choose-field-type-2-hand.png)

1. Fare clic su **Next**.

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. Immettere l&#39;etichetta del campo, la lunghezza e il nome del campo, come illustrato nella tabella seguente.

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
      Attributi campo 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Punteggio</td> 
   <td>mkto71_Lead_Score</td> 
   <td>Numero</td> 
   <td>Lunghezza 10<br>Posti decimali 0 </td> 
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

1. Fare clic su **Next**.

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. Specificate le impostazioni di accesso e fate clic su **Next**:

   * Impostate tutti i ruoli su **Visible** e **Read Only**

   * Deselezionare la casella di controllo **Solo lettura** per il profilo dell&#39;utente di sincronizzazione:

      * Se si dispone di un utente con il profilo di _Amministratore di sistema_ come utente di sincronizzazione, deselezionare la casella di controllo **Solo lettura** per il profilo Amministratore di sistema (come mostrato di seguito)

      * Se avete creato un profilo _personalizzato_ per l&#39;utente della sincronizzazione, deselezionate la casella di controllo **Solo lettura** per tale profilo personalizzato

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. Scegliete i layout di pagina in cui visualizzare il campo.

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. Fare clic su **Salva e nuovo** per tornare indietro e creare ciascuno degli altri due campi personalizzati. Fare clic su **Salva** per terminare con tutte e tre le operazioni.

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. Nel menu Genera a sinistra, fare clic su **Personalizza** e selezionare **Contatti**. Fare clic su **Campi**.
1. Effettuate i passaggi da 3 a 10 per i campi Valutazione, Data acquisizione e Programma di acquisizione sull’oggetto di contatto, come per l’oggetto lead.
1. Facoltativamente, utilizzare la procedura descritta sopra per tutti i campi personalizzati aggiuntivi di questa tabella.

<table> 
 <tbody> 
  <tr> 
   <th>Etichetta campo</th> 
   <th>Nome campo</th> 
   <th>Tipo di dati</th> 
   <th>Attributi campo</th> 
  </tr> 
  <tr> 
   <td>Id Programma Di Acquisizione</td> 
   <td>mkto71_Acquisition_Program_Id</td> 
   <td>Numero</td> 
   <td>Lunghezza 18<br>Posti decimali 0 </td> 
  </tr> 
  <tr> 
   <td>Referente originale</td> 
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
   <td>Tipo origine originale</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Città di provenienza</td> 
   <td>mkto71_Inferred_City</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Società destinataria</td> 
   <td>mkto71_Inferred_Company</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Paese di provenienza</td> 
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
   <td>Codice area telefono</td> 
   <td>mkto71_Inferred_Phone_Area_Code</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Codice postale</td> 
   <td>mkto71_Inferred_Postal_Code</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Regione dello stato di provenienza</td> 
   <td>mkto71_Inferred_State_Region</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
 </tbody> 
</table>

## Mappa campi personalizzati per le conversioni {#map-custom-fields-for-conversions}

Un campo personalizzato sull&#39;oggetto lead in Salesforce deve essere mappato su un campo contatto sull&#39;oggetto contatto in modo che i dati vengano trasferiti quando si verifica una conversione.

1. Nell’angolo in alto a destra, fate clic su Configurazione.

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. Digitare &quot;fields&quot; nella Ricerca nav senza premere Invio. I campi sono visualizzati sotto diversi oggetti; Fate clic su Campi in Lead.

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. Andate alla sezione Campi personalizzati lead e relazioni e fate clic su Mappa campi lead.

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. Fai clic sul menu a discesa accanto al campo da mappare.

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. Selezionare il campo personalizzato di contatto corrispondente.

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. Ripetete i passaggi indicati sopra per tutti gli altri campi creati.
1. Al termine, fate clic su Salva.

Abbastanza facile, giusto?

>[!NOTE]
>
>Ecco un [video dell&#39;intero processo](https://nation.marketo.com/videos/1475) che dovrebbe renderlo chiaro!

>[!MORELIKETHIS]
>
>[Passaggio 2 di 3: Creare un utente Salesforce per Marketo (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)
