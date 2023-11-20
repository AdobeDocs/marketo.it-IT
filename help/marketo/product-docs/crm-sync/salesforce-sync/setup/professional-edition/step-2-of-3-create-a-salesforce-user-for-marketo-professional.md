---
unique-page-id: 3571797
description: Passaggio 2 di 3 -Creazione di un utente Salesforce per Marketo (Professional) - Documentazione Marketo - Documentazione del prodotto
title: 'Passaggio 2 di 3: creare un utente Salesforce per Marketo (Professional)'
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 8%

---

# Passaggio 2 di 3: creare un utente Salesforce per Marketo (Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>Questi passaggi devono essere completati da un amministratore Salesforce.

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}

In questo articolo personalizzerai le autorizzazioni per i campi con un layout di pagina Salesforce e creerai un utente di sincronizzazione Marketo-Salesforce.

## Imposta layout di pagina {#set-page-layouts}

Salesforce Professional imposta l&#39;accessibilità a livello di campo con Layout di pagina, anziché con i Profili di Salesforce Enterprise/Unlimited. La procedura seguente consente all&#39;utente di Marketo Sync di aggiornare i campi personalizzati.

1. Digita &quot;[!UICONTROL layout di pagina]&quot; nella barra di ricerca di navigazione senza premere **[!UICONTROL Invio]** e fai clic su **[!UICONTROL Layout di pagina]** in **[!UICONTROL Lead]**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Clic **[!UICONTROL Modifica]** accanto a Layout lead.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Fai clic e trascina un nuovo **[!UICONTROL Sezione]** nel layout di pagina.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Immetti &quot;Marketo&quot; per **[!UICONTROL Nome sezione]** e fai clic su **[!UICONTROL OK]**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Fai clic e trascina il campo **[!UICONTROL Data di acquisizione]** in **Marketo** sezione.

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Ripeti il passaggio precedente per i campi seguenti:

   * Programma di acquisizione
   * ID programma di acquisizione
   * Rinuncia e-mail
   * Città dedotta
   * Azienda in oggetto
   * Paese in oggetto
   * Area metropolitana dedotta
   * Prefisso telefonico dedotto
   * Codice postale dedotto
   * Area geografica dello stato dedotta
   * Punteggio lead
   * Destinatario che inoltra originale
   * Motore di ricerca originale
   * Frase di ricerca originale
   * Informazioni sorgente originali
   * Tipo di sorgente originale

   >[!NOTE]
   >
   >Questi campi devono trovarsi nel layout di pagina in modo che Marketo possa leggerli/scrivervi.

   >[!TIP]
   >
   >Per creare due colonne per i campi, trascinare verso il basso il lato destro della pagina. È possibile spostare i campi da un lato all&#39;altro per bilanciare la lunghezza delle colonne.

1. Clic **[!UICONTROL Salva]** al termine dell’aggiunta dei campi.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Ripeti tutti i passaggi precedenti per Salesforce **[!UICONTROL Layout pagina contatto]**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. Ricordati di fare clic su **[!UICONTROL Salva]** quando hai terminato con **[!UICONTROL Layout pagina contatto]**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >Assicurati che il **[!UICONTROL Evento giornata intera]** è stato aggiunto al **[!UICONTROL Layout pagina evento]**.

## Crea utente di sincronizzazione {#create-sync-user}

Marketo richiede le credenziali per accedere a Salesforce. Questa operazione può essere eseguita con un utente dedicato creato con i passaggi seguenti.

>[!NOTE]
>
>Se la tua organizzazione non dispone di licenze Salesforce aggiuntive, puoi utilizzare un utente Marketing esistente con il profilo Amministratore di sistema.

1. Immetti &quot;users&quot; (Utenti) nella barra di ricerca di navigazione e fai clic su **[!UICONTROL Utenti]** in **[!UICONTROL Gestisci utenti]**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Clic **[!UICONTROL Nuovo utente]**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Compila i campi obbligatori, seleziona la **[!UICONTROL Licenza utente: Salesforce]**, imposta **[!UICONTROL Profilo: Amministratore di sistema]**, spunta **[!UICONTROL Utente marketing]** e fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Verifica che l’indirizzo e-mail inserito sia valido. Per reimpostare la password è necessario accedere come utente di sincronizzazione.

Eccellente! Ora disponi di un account che Marketo può utilizzare per connettersi a Salesforce. Facciamolo.

>[!MORELIKETHIS]
>
>[Passaggio 3 di 3: collegare Marketo e Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md){target="_blank"}
