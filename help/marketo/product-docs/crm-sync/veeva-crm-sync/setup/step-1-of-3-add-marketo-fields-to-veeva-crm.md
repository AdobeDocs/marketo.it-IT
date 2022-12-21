---
description: Passaggio 1 di 3 - Aggiungere campi Marketo a Veeva CRM - Marketo Docs - Documentazione del prodotto
title: Passaggio 1 di 3 - Aggiungere campi Marketo a Veeva CRM
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
source-git-commit: bb020cba0bb0cb65761e15cba05147b6e9fffe50
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 6%

---

# Passaggio 1 di 3: Aggiungere campi Marketo a Veeva CRM {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>La tua istanza di Veeva CRM deve avere accesso alle API Salesforce per sincronizzare i dati tra Marketi Engage e Veeva CRM.

Il Marketo Engage utilizza un set di campi per acquisire alcuni tipi di informazioni relative al marketing. Se desideri questi dati in Veeva CRM, segui le istruzioni riportate di seguito.

`1.` Crea un campo personalizzato in Veeva CRM sugli oggetti di contatto: Punteggio

`2.` Se necessario, puoi creare altri campi (vedi la tabella seguente).

Tutti questi campi personalizzati sono facoltativi e non sono necessari per sincronizzare il Marketo Engage e Veeva CRM.

## Aggiungere campi Marketo a Veeva CRM {#add-marketo-fields-to-veeva-crm}

Aggiungi un campo personalizzato sugli oggetti lead e contact in Veeva CRM elencati sopra. Per ulteriori informazioni, consulta la tabella dei campi disponibili alla fine di questa sezione.

Esegui i seguenti passaggi per aggiungere il campo Punteggio .

1. Accedi a Veeva CRM e fai clic su **Configurazione**.

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. Fare clic su Oggetti e campi e selezionare Gestione oggetti.

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. Nella barra di ricerca, cerca Contatto.

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. Fare clic sull&#39;oggetto Contact.

1. Selezionare Campi e relazioni.

1. Fai clic su **Nuovo**.

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. Scegli il tipo di campo appropriato (per Punteggio — numero).

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. Fai clic su **Successivo**.

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. Immetti Etichetta campo, Lunghezza e Nome campo per il campo, come illustrato nella tabella seguente.

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
Posizioni decimali 0</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Veeva CRM aggiunge __c ai nomi dei campi quando li utilizza per creare nomi API.

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>I campi di testo e numerici richiedono una lunghezza, ma non i campi data/ora. Una descrizione è facoltativa.

1. Fai clic su **Successivo**.

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. Specifica le impostazioni di accesso e fai clic su **Successivo**.

1. Imposta tutti i ruoli su Visibile e di sola lettura.

1. Deseleziona la casella di controllo Sola lettura per il profilo dell&#39;utente di sincronizzazione:

* Se si dispone di un utente con il profilo di un amministratore di sistema come utente di sincronizzazione, deselezionare la casella di controllo Sola lettura del profilo Amministratore di sistema (come mostrato di seguito).
* Se hai creato un profilo personalizzato per l’utente di sincronizzazione, deseleziona la casella di controllo Sola lettura per tale profilo personalizzato.

   ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. Scegliere i layout di pagina da visualizzare nel campo.

1. Fai clic su **Salva e nuovo** per tornare indietro e creare ciascuno degli altri due campi personalizzati.

1. Fai clic su **Salva** quando hai finito con tutti e tre.

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>Aggiungendo il campo all&#39;oggetto Contact, vengono aggiunti anche all&#39;oggetto Account persona.

FACOLTATIVO: Utilizza la procedura precedente per tutti i campi personalizzati aggiuntivi della tabella seguente.

<table>
 <tbody>
  <tr>
   <th>Etichetta campo
   <th>Nome campo
   <th>Tipo di dati
   <th>Attributi del campo
  </tr>
  <tr>
   <td>Città in oggetto</td>
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
   <td>oArea metropolitana in oggetto</td>
   <td>mkto71_Inferred_Metropolitan_Area</td>
   <td>Testo</td>
   <td>Lunghezza 255</td>
  </tr>
  <tr>
   <td>Prefisso telefonico in oggetto</td>
   <td>mkto71_Inferred_Phone_Area_Code</td>
   <td>Testo</td>
   <td>Lunghezza 255</td>
  </tr>
  <tr>
   <td>Codice postale in oggetto</td>
   <td>mkto71_Inferred_Postal_Code</td>
   <td>Testo</td>
   <td>Lunghezza 255</td>
  </tr>
  <tr>
   <td>Stato in oggetto</td>
   <td>mkto71_Inferred_State_Region</td>
   <td>Testo</td>
   <td>Lunghezza 255</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>I valori nei campi assegnati automaticamente da Marketo non saranno immediatamente disponibili in Veeva CRM quando il nuovo campo è stato creato. Marketo sincronizzerà i dati con Veeva CRM al successivo aggiornamento del record su entrambi i sistemi (ovvero, un aggiornamento a uno qualsiasi dei campi in sincronia tra Marketo e Veeva CRM).
