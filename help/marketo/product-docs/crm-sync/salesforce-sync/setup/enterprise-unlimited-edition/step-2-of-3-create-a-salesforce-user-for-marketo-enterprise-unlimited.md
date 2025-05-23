---
unique-page-id: 2360364
description: Passaggio 2 di 3 -Creare un utente Salesforce per Marketo (Enterprise/Unlimited) - Documentazione Marketo - Documentazione del prodotto
title: 'Passaggio 2 di 3: creazione di un utente Salesforce per Marketo (Enterprise/Unlimited)'
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 3%

---

# Passaggio 2 di 3: creare un utente Salesforce per Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Questi passaggi devono essere completati da un amministratore Salesforce

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

In questo articolo, configurerai le autorizzazioni utente nel profilo Salesforce e creerai un account di integrazione Marketo-Salesforce.

## Creare un profilo {#create-a-profile}

1. Fare clic su **[!UICONTROL Configurazione]**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Digita &quot;profiles&quot; nella barra di ricerca di navigazione e fai clic sul collegamento **[!UICONTROL Profili]**.

   ![](assets/sfdc-profiles-hands.png)

1. Fai clic su **[!UICONTROL Nuovo]**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Seleziona **[!UICONTROL Utente standard]**, denomina il profilo &quot;Marketo-Salesforce Sync&quot; e fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Imposta autorizzazioni profilo {#set-profile-permissions}

1. Fai clic su **[!UICONTROL Modifica]** per impostare le autorizzazioni di protezione.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Nella sezione **[!UICONTROL Autorizzazioni amministrative]**, assicurati che siano selezionate le caselle seguenti:

   * API abilitata
   * Modifica modelli di HTML
   * Gestisci documenti pubblici
   * Gestisci modelli pubblici

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Assicurarsi di selezionare la casella **[!UICONTROL Password Never Expires]**.

1. Nella sezione Autorizzazioni utente generali verificare che siano selezionate le caselle seguenti:

   * Converti lead
   * Modifica eventi
   * Modifica le Attività

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Nella sezione Autorizzazioni oggetto standard verificare che le autorizzazioni di lettura, creazione, modifica ed eliminazione siano verificate per:

   * Account
   * Campagne
   * Contatti
   * Lead
   * Opportunità

   >[!NOTE]
   >
   >Concedi le autorizzazioni per le campagne, se intendi utilizzare Campaign Sync.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Al termine, fare clic su **[!UICONTROL Salva]** nella parte inferiore della pagina.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Imposta autorizzazioni campo {#set-field-permissions}

1. Rivolgiti ai tuoi esperti di marketing per scoprire quali campi personalizzati sono necessari per la sincronizzazione.

   >[!NOTE]
   >
   >Questo passaggio impedisce la visualizzazione dei campi non necessari in Marketo, riducendo il disordine e velocizzando la sincronizzazione.

1. Nella pagina dei dettagli del profilo, vai alla sezione **[!UICONTROL Sicurezza a livello di campo]**. Fare clic su **[!UICONTROL Visualizza]** per modificare l&#39;accessibilità per gli oggetti:

   * Lead
   * Contatto
   * Account
   * Opportunità

   >[!TIP]
   >
   >Puoi configurare altri oggetti in base alle esigenze della tua organizzazione.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Per ogni oggetto, fare clic su **[!UICONTROL Modifica]**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Individua i campi non necessari, assicurati che **[!UICONTROL Accesso in lettura]** e **[!UICONTROL Accesso in modifica]** siano deselezionati. Al termine, fai clic su **[!UICONTROL Salva]**.

   >[!NOTE]
   >
   >Modifica solo l’accessibilità per i campi personalizzati.

   ![](assets/sfdc-sync-field-edit2.png)

1. Dopo aver disabilitato tutti i campi non necessari, è necessario selezionare **[!UICONTROL Accesso in lettura e accesso in modifica]** per i campi oggetto seguenti. Al termine, fai clic su **[!UICONTROL Salva]**.

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
>Creare un account Salesforce dedicato (ad esempio, `marketo@yourcompany.com`) per distinguere le modifiche apportate da Marketo rispetto ad altri utenti di Salesforce.

1. Digita &quot;Gestisci utenti&quot; nella barra di ricerca di navigazione, quindi fai clic su **[!UICONTROL Utenti]**. Fare clic su **[!UICONTROL Nuovo utente]**.

   ![](assets/sfdc-new-users.png)

1. Compila i campi obbligatori. Quindi, selezionare la **[!UICONTROL licenza utente: Salesforce]** e il profilo creato in precedenza. Al termine, fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Viene completato il passaggio 2 di 3.

>[!NOTE]
>
>[Passaggio 3 di 3: connettere Marketo e Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}
