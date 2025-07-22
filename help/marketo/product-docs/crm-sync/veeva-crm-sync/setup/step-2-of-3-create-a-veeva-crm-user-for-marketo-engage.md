---
description: Passaggio 2 di 3 - Creazione di un utente CRM [!DNL Veeva] per Marketo Engage - Documenti Marketo - Documentazione del prodotto
title: Passaggio 2 di 3 - Creare un utente Veeva CRM per Marketo Engage
exl-id: 78945192-36b0-4e0b-830a-f37eb0b83484
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 6%

---

# Passaggio 2 di 3: creazione di un utente CRM [!DNL Veeva] per Marketo Engage {#step-2-of-3-create-a-veeva-crm-user-for-marketo-engage}

>[!NOTE]
>
>I passaggi in questo articolo devono essere completati da un amministratore di CRM [!DNL Veeva].

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: aggiunta di campi Marketo a [!DNL Salesforce] (Professional)](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}

In questo articolo personalizzerai le autorizzazioni del campo con un layout di pagina CRM [!DNL Veeva] e creerai un utente di sincronizzazione CRM [!DNL Marketo-Veeva].

## Imposta layout di pagina {#set-page-layouts}

La procedura seguente consente all&#39;utente di Marketo Sync di aggiornare i campi personalizzati.

1. Fare clic sui layout di pagina **[!UICONTROL Account]** (account persona) nella barra di ricerca di navigazione senza premere Invio, quindi fare clic su **[!UICONTROL Page Layout]** in [!UICONTROL Contacts].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. Fai clic su **[!UICONTROL Page Layouts]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. Fai clic su **[!UICONTROL HCP - Professional]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. Fare clic e trascinare un nuovo **[!UICONTROL Section]** nel layout di pagina.

1. Immettere &quot;Marketo&quot; per **[!UICONTROL Section Name]** e fare clic su **[!UICONTROL OK]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. Fai clic su e trascina il campo **[!UICONTROL Score]** nella sezione Marketo.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-5.png)

1. Ripeti il passaggio precedente per i campi seguenti:

   * Città dedotta
   * Azienda in oggetto
   * Paese in oggetto
   * Area metropolitana dedotta
   * Prefisso telefonico dedotto
   * Codice postale dedotto
   * Area geografica dello stato dedotta

   >[!NOTE]
   >
   >Questi campi devono trovarsi nel layout di pagina in modo che Marketo possa leggerli/scrivervi.

   >[!TIP]
   >
   >Per creare due colonne per i campi, trascinare verso il basso il lato destro della pagina. È possibile spostare i campi da un lato all&#39;altro per bilanciare la lunghezza delle colonne.

1. Al termine del layout [!UICONTROL HCP-Professional], fare clic su **[!UICONTROL Save]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

>[!NOTE]
>
>Ripetere questa operazione per gli altri [!UICONTROL Account] layout di pagina.

## Creare un profilo {#create-a-profile}

1. Fai clic su **[!UICONTROL Setup]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. Digitare &quot;profiles&quot; nella barra di ricerca di navigazione e fare clic sul collegamento **[!UICONTROL Profiles]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. Fai clic su **[!UICONTROL New]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. Selezionare **[!UICONTROL Standard User]**, denominare il profilo &quot;[!UICONTROL Marketo-Salesforce Sync]&quot; e fare clic su **[!UICONTROL Save]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## Imposta autorizzazioni profilo {#set-profile-permissions}

1. Fare clic su **[!UICONTROL Edit]** per impostare le autorizzazioni di protezione.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. Nella sezione [!UICONTROL Administrative Permissions], assicurati che [!UICONTROL API Enabled] sia selezionato.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >Assicurarsi di selezionare la casella [!UICONTROL Password Never Expires].

1. Nella sezione [!UICONTROL General User Permissions], assicurati che [!UICONTROL Edit Events] e [!UICONTROL Edit Tasks] siano selezionati.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. Nella sezione [!UICONTROL Standard Object Permissions] verificare che le autorizzazioni [!UICONTROL Read], [!UICONTROL Create], [!UICONTROL Edit] e [!UICONTROL Delete] siano verificate per [!UICONTROL Accounts] e [!UICONTROL Contacts].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. Nella sezione [!UICONTROL Custom Object Permissions], verificare che le autorizzazioni [!UICONTROL Read] siano verificate per [!UICONTROL Call], [!UICONTROL Call Key Message] e per qualsiasi altro oggetto personalizzato desiderato.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. Al termine, fare clic su **[!UICONTROL Save]** nella parte inferiore della pagina.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## Imposta autorizzazioni campo {#set-field-permissions}

1. Rivolgiti ai tuoi esperti di marketing per scoprire quali campi personalizzati sono necessari per la sincronizzazione.

   >[!NOTE]
   >
   >Questo passaggio impedisce la visualizzazione dei campi non necessari in Marketo, riducendo il disordine e velocizzando la sincronizzazione.

1. Nella pagina [!UICONTROL profile detail], vai alla sezione **[!UICONTROL Field-Level Security]**. Fare clic su **[!UICONTROL View]** per modificare l&#39;accessibilità per gli oggetti [!UICONTROL Contact] e [!UICONTROL Account].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

   >[!TIP]
   >
   >Puoi configurare altri oggetti in base alle esigenze della tua organizzazione.

1. Per ogni oggetto, fare clic su **[!UICONTROL Edit]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

Individuare i campi non necessari, verificare che [!UICONTROL Read Access] e [!UICONTROL Edit Access] siano **un** selezionati. Al termine, fai clic su **[!UICONTROL Save]**.

![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

>[!NOTE]
>
>Modifica solo l’accessibilità per i campi personalizzati.

1. Dopo aver disabilitato tutti i campi non necessari, selezionare [!UICONTROL Read Access] e [!UICONTROL Edit Access] per i campi oggetto seguenti. Al termine, fai clic su **[!UICONTROL Save]**.

<table>
 <tbody>
  <tr>
   <th>Oggetto
   <th>Campi
  </tr>
  <tr>
   <td>Account</td>
   <td>Campo tipo</td>
  </tr>
  <tr>
   <td>Evento</td>
   <td>Tutti i campi</td>
  </tr>
  <tr>
   <td>Attività</td>
   <td>Tutti i campi</td>
  </tr>
 </tbody>
</table>

## Crea utente di sincronizzazione {#create-sync-user}

Marketo richiede le credenziali per accedere a [!DNL Veeva] CRM. Questa operazione può essere eseguita con un utente dedicato creato con i passaggi seguenti.

>[!NOTE]
>
>Se la tua organizzazione non dispone di ulteriori [!DNL Veeva] licenze CRM, puoi utilizzare un utente Marketing esistente con il profilo Amministratore di sistema.

1. Immettere &quot;utenti&quot; nella barra di ricerca di navigazione e fare clic su **[!UICONTROL Users]** in [!UICONTROL Manage Users].

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. Fai clic su **[!UICONTROL New User]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. Compila i campi obbligatori, seleziona **[!UICONTROL User License]**: **[!UICONTROL Salesforce]**, imposta l&#39;utente **[!UICONTROL Profile]**: **[!UICONTROL Marketo Sync]** e fai clic su **[!UICONTROL Save]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>Verifica che l’indirizzo e-mail inserito sia valido. Per reimpostare la password è necessario accedere come utente di sincronizzazione.

Eccellente! Ora disponi di un account che Marketo Engage può utilizzare per connettersi a [!DNL Veeva] CRM. Facciamolo.

>[!MORELIKETHIS]
>
>[Passaggio 3 di 3: connettere Marketo e [!DNL Veeva] CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target="_blank"}
