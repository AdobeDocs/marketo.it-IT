---
unique-page-id: 2360364
description: Passaggio 2 di 3 -Creare un utente Salesforce per Marketo (Enterprise/Unlimited) - Documentazione Marketo - Documentazione del prodotto
title: 'Passaggio 2 di 3: creazione di un utente Salesforce per Marketo (Enterprise/Unlimited)'
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 2%

---

# Passaggio 2 di 3: creazione di un utente [!DNL Salesforce] per Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Questi passaggi devono essere completati da un amministratore [!DNL Salesforce]

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: aggiunta di campi Marketo a [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

In questo articolo verranno impostate le autorizzazioni utente nel profilo [!DNL Salesforce] e verrà creato un account di integrazione Marketo-[!DNL Salesforce].

## Creare un profilo {#create-a-profile}

1. Fai clic su **[!UICONTROL Setup]**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Digitare &quot;profiles&quot; nella barra di ricerca di navigazione e fare clic sul collegamento **[!UICONTROL Profiles]**.

   ![](assets/sfdc-profiles-hands.png)

1. Fai clic su **[!UICONTROL New]**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Selezionare **[!UICONTROL Standard User]**, denominare il profilo &quot;Marketo-Salesforce Sync&quot; e fare clic su **[!UICONTROL Save]**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Imposta autorizzazioni profilo {#set-profile-permissions}

1. Fare clic su **[!UICONTROL Edit]** per impostare le autorizzazioni di protezione.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Nella sezione **[!UICONTROL Administrative Permissions]** verificare che siano selezionate le caselle seguenti:

   * [!UICONTROL API Enabled]
   * [!UICONTROL Edit HTML Templates]
   * [!UICONTROL Manage Public Documents]
   * [!UICONTROL Manage Public Templates]

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Assicurarsi di selezionare la casella **[!UICONTROL Password Never Expires]**.

1. Nella sezione [!UICONTROL General User Permissions] verificare che siano selezionate le caselle seguenti:

   * [!UICONTROL Convert Leads]
   * [!UICONTROL Edit Events]
   * [!UICONTROL Edit Tasks]

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Nella sezione [!UICONTROL Standard Object Permissions], assicurati che siano verificate le autorizzazioni [!UICONTROL Read, Create, Edit, and Delete] per:

   * [!UICONTROL Accounts]
   * [!UICONTROL Campaigns]
   * [!UICONTROL Contacts]
   * [!UICONTROL Leads]
   * [!UICONTROL Opportunities]

   >[!NOTE]
   >
   >Concedere le autorizzazioni a [!UICONTROL Campaigns], se si intende utilizzare Campaign Sync.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Al termine, fare clic su **[!UICONTROL Save]** nella parte inferiore della pagina.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Imposta autorizzazioni campo {#set-field-permissions}

1. Rivolgiti ai tuoi esperti di marketing per scoprire quali campi personalizzati sono necessari per la sincronizzazione.

   >[!NOTE]
   >
   >Questo passaggio impedisce la visualizzazione dei campi non necessari in Marketo, riducendo il disordine e velocizzando la sincronizzazione.

1. Nella pagina dei dettagli del profilo, vai alla sezione **[!UICONTROL Field-Level Security]**. Fare clic su **[!UICONTROL View]** per modificare l&#39;accessibilità per gli oggetti:

   * [!UICONTROL Lead]
   * [!UICONTROL Contact]
   * [!UICONTROL Account]
   * [!UICONTROL Opportunity]

   >[!TIP]
   >
   >Puoi configurare altri oggetti in base alle esigenze della tua organizzazione.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Per ogni oggetto, fare clic su **[!UICONTROL Edit]**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Individuare i campi non necessari, verificare che **[!UICONTROL Read Access]** e **[!UICONTROL Edit Access]** siano deselezionati. Al termine, fai clic su **[!UICONTROL Save]**.

   >[!NOTE]
   >
   >Modifica solo l’accessibilità per i campi personalizzati.

   ![](assets/sfdc-sync-field-edit2.png)

1. Dopo aver disabilitato tutti i campi non necessari, è necessario controllare **[!UICONTROL Read Access and Edit Access]** per i seguenti campi oggetto. Al termine, fai clic su **[!UICONTROL Save]**.

<table>
 <tbody>
  <tr>
   <th>Oggetto</th>
   <th>Campi</th>
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

![](assets/sfdc-check-the-boxes.png)

## Crea account di sincronizzazione Marketo-Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Creare un account [!DNL Salesforce] dedicato (ad esempio, <marketo@yourcompany.com>) per distinguere le modifiche apportate da Marketo rispetto ad altri utenti [!DNL Salesforce].

1. Digitare &quot;Gestisci utenti&quot; nella barra di ricerca di navigazione, quindi fare clic su **[!UICONTROL Users]**. Fai clic su **[!UICONTROL New User]**.

   ![](assets/sfdc-new-users.png)

1. Compila i campi obbligatori. Quindi, seleziona **[!UICONTROL User License: Salesforce]** e il profilo creato in precedenza. Al termine, fai clic su **[!UICONTROL Save]**.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Viene completato il passaggio 2 di 3.

>[!NOTE]
>
>[Passaggio 3 di 3: connettere Marketo e [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
