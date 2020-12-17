---
unique-page-id: 3571797
description: Passaggio 2 di 3 - Crea un utente Salesforce per Marketo (Professional) - Marketo Docs - Documentazione del prodotto
title: Passaggio 2 di 3 - Crea un utente Salesforce per Marketo (Professional)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---


# Passaggio 2 di 3: Crea un utente Salesforce per Marketo (Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>Questi passaggi devono essere completati da un amministratore Salesforce

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: Aggiunta di campi Marketo a Salesforce (Professional)](step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

>



In questo articolo, personalizzerai le autorizzazioni per i campi con un layout di pagina Salesforce e creerai un utente per la sincronizzazione Marketo-Salesforce.

## Imposta layout pagina {#set-page-layouts}

Salesforce Professional imposta l&#39;accessibilità a livello di campo con i layout di pagina, invece dei profili di Salesforce Enterprise/Unlimited. Seguendo questa procedura, l&#39;utente di Marketo potrà sincronizzare l&#39;utente e aggiornare i campi personalizzati.

1. Digitare **layout di pagina** nella barra di ricerca Nav senza premere **Invio**, quindi fare clic su **Layout di pagina** in **Lead**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Fate clic su **Modifica** accanto a Layout lead.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Fare clic e trascinare un nuovo elemento **Section** nel layout della pagina.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Immettere &quot;Marketo&quot; per **Nome sezione** e fare clic su **OK**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Fare clic e trascinare il campo **Data acquisizione** nella sezione **Marketo**.

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Ripetere il passaggio precedente per i campi seguenti:

   * Programma di acquisizione
   * Id Programma Di Acquisizione
   * Rifiuto e-mail
   * Città di provenienza
   * Società destinataria
   * Paese di provenienza
   * Area metropolitana
   * Codice area telefono
   * Codice postale
   * Regione dello stato di provenienza
   * Punteggio lead
   * Referente originale
   * Motore di ricerca originale
   * Frase di ricerca originale
   * Informazioni origine originali
   * Tipo origine originale

   >[!NOTE]
   >
   >Questi campi devono trovarsi nel layout di pagina in modo che Marketo possa leggerli o scriverli.

   >[!TIP]
   >
   >Creare due colonne per i campi trascinando verso il basso a destra della pagina. È possibile spostare i campi da un lato all&#39;altro per bilanciare le lunghezze delle colonne.

1. Fare clic su **Save** al termine dell&#39;aggiunta dei campi.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Ripetete tutti i passaggi indicati sopra per il layout della pagina di contatto **Salesforce**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. Ricordare di fare clic su **Save** al termine della procedura **Contact Page Layout**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >**Promemoria**
   >
   >
   >Assicurarsi che il campo **All-Day Event** sia stato aggiunto al **Event Page Layout**.

## Crea sincronizzazione utente {#create-sync-user}

Marketo richiede le credenziali per accedere a Salesforce. Questa operazione è consigliabile con un utente dedicato creato con i passaggi indicati di seguito.

>[!NOTE]
>
>Se l&#39;organizzazione non dispone di licenze Salesforce aggiuntive, è possibile utilizzare un utente Marketing **Marketing** esistente con il profilo **Amministratore di sistema**.

1. Immettete &quot;users&quot; nella barra di ricerca della navigazione e fate clic su **Users** in **Gestisci utenti**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Fare clic su **Nuovo utente**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Compila i campi richiesti, seleziona la **Licenza utente: Salesforce**, imposta il **profilo: Amministratore di sistema**, controllare **Marketing User** e fare clic su **Salva**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Verificate che l&#39;indirizzo e-mail immesso sia valido. Per ripristinare la password dovrete effettuare l&#39;accesso come utente sincronizzato.

Eccellente! Ora hai un account che Marketo può usare per connettersi a Salesforce. Facciamolo.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Passaggio 3 di 3: Connect Marketo e Salesforce (Professional)](step-3-of-3-connect-marketo-and-salesforce-professional.md)

>



