---
unique-page-id: 3571797
description: Passaggio 2 di 3 -Creare un utente Salesforce per Marketo (Professional) - Documentazione Marketo - Documentazione del prodotto
title: 'Passaggio 2 di 3: creazione di un utente Salesforce per Marketo (Professional)'
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Passaggio 2 di 3: creazione di un utente [!DNL Salesforce] per Marketo (Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>Questi passaggi devono essere completati da un amministratore Salesforce.

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}

In questo articolo personalizzerai le autorizzazioni del campo con un layout di pagina [!DNL Salesforce] e creerai un utente di sincronizzazione Marketo-[!DNL Salesforce].

## Imposta layout di pagina {#set-page-layouts}

[!DNL Salesforce] Professional imposta l&#39;accessibilità a livello di campo con Layout di pagina, anziché con i profili di [!DNL Salesforce] Enterprise/Unlimited. La procedura seguente consente all&#39;utente di Marketo Sync di aggiornare i campi personalizzati.

1. Digitare &quot;[!UICONTROL page layouts]&quot; nella barra di ricerca di spostamento senza premere **[!UICONTROL Enter]** e fare clic su **[!UICONTROL Page Layout]** in **[!UICONTROL Leads]**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Fare clic su **[!UICONTROL Edit]** accanto a Layout lead.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Fare clic e trascinare un nuovo **[!UICONTROL Section]** nel layout di pagina.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Immettere &quot;Marketo&quot; per **[!UICONTROL Section Name]** e fare clic su **[!UICONTROL OK]**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Fare clic e trascinare il campo **[!UICONTROL Acquisition Date]** nella sezione **Marketo**.

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Ripeti il passaggio precedente per i campi seguenti:

   * [!UICONTROL Acquisition Program]
   * [!UICONTROL Acquisition Program Id]
   * [!UICONTROL Email Opt Out]
   * [!UICONTROL Inferred City]
   * [!UICONTROL Inferred Company]
   * [!UICONTROL Inferred Country]
   * [!UICONTROL Inferred Metropolitan Area]
   * [!UICONTROL Inferred Phone Area Code]
   * [!UICONTROL Inferred Postal Code]
   * [!UICONTROL Inferred State Region]
   * [!UICONTROL Lead Score]
   * [!UICONTROL Original Referrer]
   * [!UICONTROL Original Search Engine]
   * [!UICONTROL Original Search Phrase]
   * [!UICONTROL Original Source Info]
   * [!UICONTROL Original Source Type]

   >[!NOTE]
   >
   >Questi campi devono trovarsi nel layout di pagina in modo che Marketo possa leggerli/scrivervi.

   >[!TIP]
   >
   >Per creare due colonne per i campi, trascinare verso il basso il lato destro della pagina. È possibile spostare i campi da un lato all&#39;altro per bilanciare la lunghezza delle colonne.

1. Fare clic su **[!UICONTROL Save]** al termine dell&#39;aggiunta dei campi.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Ripetere tutti i passaggi precedenti per Salesforce **[!UICONTROL Contact Page Layout]**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. Ricordarsi di fare clic su **[!UICONTROL Save]** al termine dell&#39;operazione con **[!UICONTROL Contact Page Layout]**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >Verificare che il campo **[!UICONTROL All-Day Event]** sia stato aggiunto a **[!UICONTROL Event Page Layout]**.

## Crea utente di sincronizzazione {#create-sync-user}

Marketo richiede le credenziali per accedere a [!DNL Salesforce]. Questa operazione può essere eseguita con un utente dedicato creato con i passaggi seguenti.

>[!NOTE]
>
>Se la tua organizzazione non dispone di licenze Salesforce aggiuntive, puoi utilizzare un utente Marketing esistente con il profilo Amministratore di sistema.

1. Immettere &quot;utenti&quot; nella barra di ricerca di navigazione e fare clic su **[!UICONTROL Users]** in **[!UICONTROL Manage Users]**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Fai clic su **[!UICONTROL New User]**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Compila i campi obbligatori, seleziona **[!UICONTROL User License: Salesforce]**, imposta **[!UICONTROL Profile: System Administrator]**, seleziona **[!UICONTROL Marketing User]** e fai clic su **[!UICONTROL Save]**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Verifica che l’indirizzo e-mail inserito sia valido. Per reimpostare la password è necessario accedere come utente di sincronizzazione.

Eccellente! Ora disponi di un account che Marketo può utilizzare per connettersi a [!DNL Salesforce]. Facciamolo.

>[!MORELIKETHIS]
>
>[Passaggio 3 di 3: connessione di Marketo e Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md){target="_blank"}
