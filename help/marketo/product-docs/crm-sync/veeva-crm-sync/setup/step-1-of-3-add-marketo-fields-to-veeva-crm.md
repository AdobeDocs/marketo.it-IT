---
description: Passaggio 1 di 3 - Aggiungere campi Marketo a Veeva CRM - Documentazione Marketo - Documentazione del prodotto
title: Passaggio 1 di 3 - Aggiungere campi Marketo a Veeva CRM
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
feature: Veeva CRM
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 6%

---

# Passaggio 1 di 3: aggiungere campi Marketo a Veeva CRM {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>L’istanza di CRM Veeva deve avere accesso alle API Salesforce per sincronizzare i dati tra Marketo Engage e CRM Veeva.

Il Marketo Engage utilizza un set di campi per acquisire determinati tipi di informazioni di marketing. Se desideri questi dati in Veeva CRM, segui le istruzioni di seguito.

`1.` Crea un campo personalizzato in Veeva CRM sugli oggetti contatto: Punteggio

`2.` Se necessario, puoi creare campi aggiuntivi (vedi la tabella seguente).

Tutti questi campi personalizzati sono facoltativi e non sono necessari per sincronizzare Marketo Engage e Veeva CRM.

## Aggiungere campi Marketo a Veeva CRM {#add-marketo-fields-to-veeva-crm}

Aggiungi un campo personalizzato sugli oggetti lead e contatto in Veeva CRM elencati sopra. Per aggiungerne altri, vedere la tabella dei campi disponibili alla fine di questa sezione.

Per aggiungerlo, effettua le seguenti operazioni per il campo Punteggio.

1. Accedi a Veeva CRM e fai clic su **[!UICONTROL Configurazione]**.

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. Fare clic su **[!UICONTROL Oggetti e campi]** e selezionare **[!UICONTROL Gestione oggetti]**.

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. Nella barra di ricerca, cerca &quot;Contatto&quot;.

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. Fare clic sull&#39;oggetto **[!UICONTROL Contact]**.

1. Selezionare **[!UICONTROL Campi e relazioni]**.

1. Fare clic su **[!UICONTROL Nuovo]**.

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. Scegliere il tipo di campo appropriato (per Punteggio - Numero).

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. Fai clic su **[!UICONTROL Avanti]**.

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. Immetti **[!UICONTROL Etichetta campo]**, **[!UICONTROL Lunghezza]** e **[!UICONTROL Nome campo]** per il campo, come illustrato nella tabella seguente.

<table>
 <tbody>
  <tr>
   <th>Etichetta campo
   <th>Nome campo
   <th>Tipo di dati
   <th>Attributi del campo
  </tr>
  <tr>
   <td>Punteggio</td>
   <td>mkto71_Lead_Score</td>
   <td>Numero</td>
   <td>Lunghezza 10<br/>
Cifre decimali 0</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Veeva CRM aggiunge __c ai nomi dei campi quando li utilizza per creare i nomi API.

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>I campi di testo e numerici richiedono una lunghezza, ma i campi di data e ora non la richiedono. Una descrizione è facoltativa.

1. Fai clic su **[!UICONTROL Avanti]**.

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. Specificare le impostazioni di accesso e fare clic su **[!UICONTROL Avanti]**.

1. Imposta tutti i ruoli su Visibile e Sola lettura.

1. Deselezionare la casella di controllo Sola lettura per il profilo dell&#39;utente di sincronizzazione:

* Se come utente di sincronizzazione è presente un utente con il profilo Amministratore di sistema, deselezionare la casella di controllo Sola lettura per il profilo Amministratore di sistema (come illustrato di seguito).
* Se è stato creato un profilo personalizzato per l&#39;utente di sincronizzazione, deselezionare la casella di controllo Sola lettura per il profilo personalizzato.

  ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. Scegliere i layout di pagina da visualizzare nel campo.

1. Fai clic su **[!UICONTROL Salva e nuovo]** per tornare indietro e creare ciascuno degli altri due campi personalizzati.

1. Al termine, fai clic su **[!UICONTROL Salva]**.

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>Aggiungendo il campo all&#39;oggetto Contact, vengono aggiunte anche all&#39;oggetto Person Account.

FACOLTATIVO: utilizzare la procedura descritta sopra per i campi personalizzati aggiuntivi della tabella seguente.

<table>
 <tbody>
  <tr>
   <th>Etichetta campo
   <th>Nome campo
   <th>Tipo di dati
   <th>Attributi del campo
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
>I valori nei campi assegnati automaticamente da Marketo non saranno immediatamente disponibili in Veeva CRM al momento della creazione del nuovo campo. Marketo sincronizzerà i dati con Veeva CRM al prossimo aggiornamento del record su entrambi i sistemi (ovvero, un aggiornamento a qualsiasi campo sincronizzato tra Marketo e Veeva CRM).
