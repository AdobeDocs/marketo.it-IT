---
unique-page-id: 2360364
description: Passaggio 2 di 3 - Creare un utente Salesforce per Marketo (Enterprise/Unlimited) - Marketo Docs - Documentazione del prodotto
title: Passaggio 2 di 3 - Creare un utente Salesforce per Marketo (Enterprise/Unlimited)
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Passaggio 2 di 3: Creare un utente Salesforce per Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Questi passaggi devono essere completati da un amministratore Salesforce

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: Aggiungi campi Marketo a Salesforce (Enterprise/Senza limiti)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

In questo articolo, configurerai le autorizzazioni utente nel profilo Salesforce e creerai un account di integrazione Marketo-Salesforce.

## Creare un profilo {#create-a-profile}

1. Fare clic su **Configurazione**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Digita &quot;profiles&quot; nella barra di ricerca della barra di navigazione e fai clic sul collegamento **Profiles** .

   ![](assets/sfdc-profiles-hands.png)

1. Fai clic su **Nuovo**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Seleziona **Utente standard**, denomina il profilo &quot;Marketo-Salesforce Sync&quot; e fai clic su **Salva**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Imposta autorizzazioni profilo {#set-profile-permissions}

1. Fare clic su **Modifica** per impostare le autorizzazioni di protezione.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Nella sezione **Autorizzazioni amministrative** , accertati che siano selezionate le seguenti caselle:

   * API abilitata
   * Modifica modelli HTML
   * Gestisci documenti pubblici
   * Gestisci modelli pubblici

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Controlla la casella **Password Never Expires** .

1. Nella sezione Autorizzazioni generali utente , accertati che siano selezionate le seguenti caselle:

   * Converti lead
   * Modifica eventi
   * Modifica attività

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Nella sezione Autorizzazioni oggetto standard , assicurati che le autorizzazioni Lettura, Crea, Modifica ed Elimina siano verificate per:

   * Account
   * Campagne
   * Contatti
   * Lead
   * Opportunità

   >[!NOTE]
   >
   >Concedi le autorizzazioni per le campagne, se intendi utilizzare la sincronizzazione delle campagne.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Al termine, fai clic su **Salva** nella parte inferiore della pagina.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Imposta autorizzazioni campo {#set-field-permissions}

1. Parla con i tuoi esperti di marketing per scoprire quali campi personalizzati sono necessari per la sincronizzazione.

   >[!NOTE]
   >
   >Questo passaggio impedisce la visualizzazione dei campi non necessari in Marketo, riducendo il disordine e velocizzando la sincronizzazione.

1. Nella pagina dei dettagli del profilo, vai alla sezione **Sicurezza a livello di campo** . Fai clic su **Visualizza** per modificare l&#39;accessibilità degli oggetti:

   * Lead
   * Contatto
   * Account
   * Opportunità

   >[!TIP]
   >
   >Puoi configurare altri oggetti in base alle esigenze della tua organizzazione.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Per ciascun oggetto, fare clic su **Modifica**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Individua i campi non necessari e assicurati che **Accesso in lettura** e **Accesso in modifica** siano deselezionati. Al termine fai clic su **Salva** .

   >[!NOTE]
   >
   >Modifica l’accessibilità solo per i campi personalizzati.

   ![](assets/sfdc-sync-field-edit2.png)

1. Dopo aver disabilitato tutti i campi non necessari, è necessario controllare **Accesso in lettura e Modifica accesso** per i seguenti campi oggetto. Al termine fai clic su **Salva** .

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1"><p>Oggetto</p></th> 
   <th colspan="1" rowspan="1"><p>Campi</p></th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Account</p></td> 
   <td colspan="1" rowspan="1"><p>Campo Tipo</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Evento</p></td> 
   <td colspan="1" rowspan="1"><p>Tutti i campi</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Attività</p></td> 
   <td colspan="1" rowspan="1"><p>Tutti i campi</p></td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## Crea account di sincronizzazione Marketo-Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Crea un account Salesforce dedicato (ad esempio, marketo@yourcompany.com) per distinguere le modifiche apportate da Marketo rispetto ad altri utenti Salesforce.

1. Digita &quot;Gestisci utenti&quot; nella barra di ricerca della barra di navigazione, quindi fai clic su **Utenti**. Fai clic su **Nuovo utente**.

   ![](assets/sfdc-new-users.png)

1. Compila i campi richiesti. Quindi, seleziona la **Licenza utente: Salesforce** e il profilo creato in precedenza. Al termine fai clic su **Salva** .

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Il passaggio 2 di 2 è completato.

>[!NOTE]
>
>[Passaggio 3 di 3: Connettere Marketo e Salesforce (Enterprise/Senza limiti)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
