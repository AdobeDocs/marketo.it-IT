---
unique-page-id: 11372975
description: Passaggio 1 di 3 - Aggiungere campi Marketo a Salesforce (Professional) - Documentazione Marketo - Documentazione del prodotto
title: 'Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Professional)'
exl-id: 1b52825e-201d-4b55-8edf-444b1653d591
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 8%

---

# Passaggio 1 di 3: aggiunta di campi Marketo a [!DNL Salesforce] (Professional) {#step-of-add-marketo-fields-to-salesforce-professional}

>[!PREREQUISITES]
>
>Per sincronizzare i dati tra Marketo Engage e Salesforce, l’istanza di Salesforce deve avere accesso alle API di Salesforce.

Marketo utilizza un set di campi per acquisire determinati tipi di informazioni di marketing. Se desideri questi dati in [!DNL Salesforce], segui le istruzioni riportate di seguito.

1. Creare tre campi personalizzati in [!DNL Salesforce] sugli oggetti lead e contatto: Punteggio, Programma di acquisizione e Data di acquisizione.
1. Mappare questi campi personalizzati tra lead e contatti in modo che alla conversione in [!DNL Salesforce] i valori vengano riportati.
1. Se necessario, puoi creare altri campi aggiuntivi (vedi la tabella seguente).

Tutti questi campi personalizzati sono facoltativi e non sono necessari per sincronizzare Marketo e [!DNL Salesforce]. Come best practice, consigliamo di creare campi per Punteggio, Programma di acquisizione e Data di acquisizione.

## Aggiungi campi Marketo a [!DNL Salesforce] {#add-marketo-fields-to-salesforce}

Aggiungere tre campi personalizzati sugli oggetti lead e contatto in [!DNL Salesforce] elencati sopra. Per aggiungerne altri, vedere la tabella dei campi disponibili alla fine di questa sezione.

Per aggiungerli, effettua le seguenti operazioni per ciascuno dei tre campi personalizzati. Inizia con **[!UICONTROL Score]**.

1. Accedere a Salesforce e fare clic su **[!UICONTROL Setup]**.

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. Nel menu Build a sinistra, fare clic su **[!UICONTROL Customize]** e selezionare **[!UICONTROL Leads]**. Fai clic su **[!UICONTROL Fields]**.

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. Fare clic su **[!UICONTROL New]** nella sezione Campi personalizzati e relazioni nella parte inferiore della pagina.

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. Scegli il tipo di campo appropriato (per Punteggio - **[!UICONTROL number]**; Programma di acquisizione - **[!UICONTROL text]**; Data di acquisizione - **Data/Ora**).

   ![](assets/choose-field-type-2-hand.png)

1. Fai clic su **[!UICONTROL Next]**.

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. Immettere [!UICONTROL Field Label], [!UICONTROL Length] e [!UICONTROL Field Name] per il campo, come illustrato nella tabella seguente.

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
>[!DNL Salesforce] aggiunge __c ai nomi di campo quando li utilizza per creare i nomi API.

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>I campi di testo e numerici richiedono una lunghezza, ma i campi di data e ora non la richiedono. Una descrizione è facoltativa.

1. Fai clic su **[!UICONTROL Next]**.

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. Specificare le impostazioni di accesso e fare clic su **[!UICONTROL Next]**:

   * Imposta tutti i ruoli su **[!UICONTROL Visible]** e **[!UICONTROL Read-Only]**

   * Deselezionare la casella di controllo **[!UICONTROL Read-Only]** per il profilo dell&#39;utente di sincronizzazione:

      * Se come utente di sincronizzazione è presente un utente con il profilo di _Amministratore di sistema_, deselezionare la casella di controllo **[!UICONTROL Read-Only]** per il profilo Amministratore di sistema (come illustrato di seguito)

      * Se hai creato un _profilo personalizzato_ per l&#39;utente di sincronizzazione, deseleziona la casella di controllo **[!UICONTROL Read-Only]** per tale profilo personalizzato

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. Scegliere i layout di pagina da visualizzare nel campo.

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. Fare clic su **[!UICONTROL Save & New]** per tornare indietro e creare ciascuno degli altri due campi personalizzati. Fai clic su **[!UICONTROL Save]** e termina con tutti e tre.

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. Nel menu Build a sinistra, fare clic su **[!UICONTROL Customize]** e selezionare **[!UICONTROL Contacts]**. Fai clic su **[!UICONTROL Fields]**.
1. Eseguire i passaggi da 3 a 10 per i campi Punteggio, Data acquisizione e Programma di acquisizione sull&#39;oggetto contatto, come è stato fatto per l&#39;oggetto lead.
1. Facoltativamente, utilizza la procedura precedente per tutti i campi personalizzati aggiuntivi di questa tabella.

<table> 
 <tbody> 
  <tr> 
   <th>Etichetta campo</th> 
   <th>Nome campo</th> 
   <th>Tipo di dati</th> 
   <th>Attributi del campo</th> 
  </tr> 
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
>I valori nei campi assegnati automaticamente da Marketo non saranno immediatamente disponibili in [!DNL Salesforce] al momento della creazione del nuovo campo. Marketo sincronizzerà i dati con [!DNL Salesforce] al prossimo aggiornamento del record in uno dei due sistemi (ovvero, un aggiornamento di uno qualsiasi dei campi sincronizzati tra Marketo e [!DNL Salesforce]).

## Mappa campi personalizzati per conversioni  {#map-custom-fields-for-conversions}

È necessario mappare un campo personalizzato sull&#39;oggetto lead in [!DNL Salesforce] a un campo contatto nell&#39;oggetto contatto in modo che i dati vengano trasferiti quando si verifica una conversione.

1. Nell&#39;angolo superiore destro fare clic su **[!UICONTROL Setup]**.

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. Digitare &quot;[!UICONTROL fields]&quot; nella ricerca di navigazione senza premere Invio. I campi vengono visualizzati in oggetti diversi. Fare clic su **[!UICONTROL Fields]** in Lead.

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. Andare alla sezione Campi personalizzati lead e relazioni e fare clic su **[!UICONTROL Map Lead Fields]**.

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. Fai clic sul menu a discesa accanto al campo da mappare.

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. Selezionare il campo personalizzato del contatto corrispondente.

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. Ripeti i passaggi precedenti per tutti gli altri campi creati.
1. Al termine, fai clic su **[!UICONTROL Save]**.

Abbastanza facile, vero?

>[!MORELIKETHIS]
>
>[Passaggio 2 di 3: creazione di un utente Salesforce per Marketo (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"}
