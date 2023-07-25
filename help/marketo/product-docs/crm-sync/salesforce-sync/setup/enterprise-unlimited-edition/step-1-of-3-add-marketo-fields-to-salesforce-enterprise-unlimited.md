---
unique-page-id: 2360362
description: Passaggio 1 di 3 - Aggiungere campi Marketo a Salesforce (Enterprise/Unlimited) - Documentazione Marketo - Documentazione del prodotto
title: 'Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Enterprise/Unlimited)'
exl-id: bcfba281-0d4b-42c3-b52a-ce1c3da884ba
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 7%

---

# Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>Per eseguire la sincronizzazione tra Marketo e Salesforce, devi avere accesso alle API di Salesforce.

Marketo utilizza un set di campi per acquisire determinati tipi di informazioni di marketing. Se desideri questi dati in Salesforce, segui le istruzioni riportate di seguito.

1. Crea tre campi personalizzati in Salesforce sugli oggetti lead e contatto: Punteggio, Programma di acquisizione e Data di acquisizione.
1. Mappa questi campi personalizzati tra lead e contatti in modo che, al momento della conversione in Salesforce, i valori vengano riportati.
1. Se necessario, puoi creare altri campi aggiuntivi (vedi la tabella seguente).

Tutti questi campi personalizzati sono facoltativi e non sono necessari per sincronizzare Marketo e Salesforce. Come best practice, consigliamo di creare campi per Punteggio, Programma di acquisizione e Data di acquisizione.

## Aggiungere campi Marketo a Salesforce {#add-marketo-fields-to-salesforce}

Aggiungi tre campi personalizzati agli oggetti lead e contatto in Salesforce elencati sopra. Per aggiungerne altri, vedere la tabella dei campi disponibili alla fine di questa sezione.

Per aggiungerli, effettua le seguenti operazioni per ciascuno dei tre campi personalizzati. Inizia con Punteggio.

1. Accedi a Salesforce e fai clic su **Configurazione**.

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. Nel menu Genera a sinistra, fai clic su **Personalizza** e seleziona **Lead**. Clic **Campi**.

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. Clic **Nuovo** nella sezione Campi personalizzati e relazioni, nella parte inferiore della pagina.

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. Scegliere il tipo di campo appropriato (per Punteggio — Numero; Programma di acquisizione — Testo; Data di acquisizione — Data/ora).

   ![](assets/choose-field-type-2-hand.png)

1. Clic **Successivo**.

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. Immettere l&#39;Etichetta campo, la Lunghezza e il Nome campo per il campo, come illustrato nella tabella seguente.

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
   <td>Lunghezza 10<br>Cifre decimali 0 </td> 
  </tr> 
  <tr> 
   <td>Data di acquisizione</td> 
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
>Salesforce aggiunge __c ai nomi dei campi quando li utilizza per creare i nomi API.

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>I campi di testo e numerici richiedono una lunghezza, ma i campi di data e ora non la richiedono. Una descrizione è facoltativa.

1. Clic **Successivo**.

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. Specifica le impostazioni di accesso e fai clic su **Successivo**:

   * Imposta tutti i ruoli su **Visibile** e **Sola lettura**

   * Cancella **Sola lettura** casella di controllo per il profilo dell&#39;utente di sincronizzazione:

      * Se hai un utente con il profilo di un _Amministratore di sistema_ come utente di sincronizzazione, cancella **Sola lettura** casella di controllo per il profilo Amministratore di sistema (come mostrato di seguito)
      * Se hai creato un’ _profilo personalizzato_ per l&#39;utente di sincronizzazione, cancellare **Sola lettura** casella di controllo per il profilo personalizzato

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. Scegliere i layout di pagina da visualizzare nel campo.

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. Clic **Salva e nuovo** per tornare indietro e creare ciascuno degli altri due campi personalizzati. Clic **Salva** con voi avete finito tutti e tre.

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. Nel menu Genera a sinistra, fai clic su **Personalizza** e selezionare Contatti. Fare clic su Campi.
1. Eseguire i passaggi da 3 a 10 per i campi Punteggio, Data acquisizione e Programma di acquisizione sull&#39;oggetto contatto, come è stato fatto per l&#39;oggetto lead.
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
   <td>ID programma di acquisizione</td> 
   <td>mkto71_Acquisition_Program_Id</td> 
   <td>Numero</td> 
   <td>Lunghezza 18<br>Cifre decimali 0 </td> 
  </tr> 
  <tr> 
   <td>Destinatario che inoltra originale</td> 
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
   <td>Informazioni sorgente originali</td> 
   <td>mkto71_Original_Source_Info</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Tipo di sorgente originale</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Città dedotta</td> 
   <td>mkto71_Inferred_City</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Azienda dedotta</td> 
   <td>mkto71_Inferred_Company</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Paese dedotto</td> 
   <td>mkto71_Inferred_Country</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Area metropolitana dedotta</td> 
   <td>mkto71_Inferred_Metropolitan_Area</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Prefisso telefonico dedotto</td> 
   <td>mkto71_Inferred_Phone_Area_Code</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Codice postale dedotto</td> 
   <td>mkto71_Inferred_Postal_Code</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
  <tr> 
   <td>Area geografica dello stato dedotta</td> 
   <td>mkto71_Inferred_State_Region</td> 
   <td>Testo</td> 
   <td>Lunghezza 255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>I valori nei campi assegnati automaticamente da Marketo non saranno immediatamente disponibili in Salesforce al momento della creazione del nuovo campo. Marketo sincronizzerà i dati con Salesforce al prossimo aggiornamento del record su uno dei due sistemi (ovvero, un aggiornamento a uno qualsiasi dei campi sincronizzati tra Marketo e Salesforce).

## Mappa campi personalizzati per conversioni {#map-custom-fields-for-conversions}

Un campo personalizzato sull’oggetto lead in Salesforce deve essere mappato su un campo contatto nell’oggetto contatto in modo che i dati vengano trasferiti quando si verifica una conversione.

1. Nell’angolo in alto a destra, fai clic su **Configurazione**.

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. Digitare &quot;Fields&quot; nella ricerca di navigazione senza premere Invio. I campi vengono visualizzati sotto oggetti diversi; fare clic su **Campi** in Lead.

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. Vai alla sezione Campi personalizzati lead e relazioni e fai clic su **Mappa campi lead**.

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. Fai clic sul menu a discesa accanto al campo da mappare.

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. Selezionare il campo personalizzato del contatto corrispondente.

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. Ripeti i passaggi precedenti per tutti gli altri campi creati.

1. Clic **Salva** quando hai finito.

   Abbastanza facile, vero?

>[!MORELIKETHIS]
>
>[Passaggio 2 di 3: creare un utente Salesforce per Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
