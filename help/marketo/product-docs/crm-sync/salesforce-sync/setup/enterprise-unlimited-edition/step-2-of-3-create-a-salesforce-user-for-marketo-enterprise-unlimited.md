---
unique-page-id: 2360364
description: Passaggio 2 di 3 -Creazione di un utente Salesforce per Marketo (Enterprise/Unlimited) - Documentazione Marketo - Documentazione del prodotto
title: 'Passaggio 2 di 3: creazione di un utente Salesforce per Marketo (Enterprise/Unlimited)'
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 3%

---

# Passaggio 2 di 3: creare un utente Salesforce per Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Questi passaggi devono essere completati da un amministratore Salesforce

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

In questo articolo, configurerai le autorizzazioni utente nel profilo Salesforce e creerai un account di integrazione Marketo-Salesforce.

## Creare un profilo {#create-a-profile}

1. Clic **Configurazione**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Digita &quot;profiles&quot; nella barra di ricerca di navigazione e fai clic sul pulsante **Profili** collegamento.

   ![](assets/sfdc-profiles-hands.png)

1. Fai clic su **Nuovo**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Seleziona **Utente standard**, assegna al profilo il nome &quot;Marketo-Salesforce Sync&quot; e fai clic su **Salva**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Imposta autorizzazioni profilo {#set-profile-permissions}

1. Clic **Modifica** per impostare le autorizzazioni di protezione.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Sotto **Autorizzazioni amministrative** sezione, assicurarsi che siano selezionate le caselle seguenti:

   * API abilitata
   * Modifica modelli di HTML
   * Gestisci documenti pubblici
   * Gestisci modelli pubblici

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Verificare che il **La password non scade** casella.

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

1. Al termine, fai clic su **Salva** nella parte inferiore della pagina.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Imposta autorizzazioni campo {#set-field-permissions}

1. Rivolgiti ai tuoi esperti di marketing per scoprire quali campi personalizzati sono necessari per la sincronizzazione.

   >[!NOTE]
   >
   >Questo passaggio impedisce la visualizzazione dei campi non necessari in Marketo, riducendo il disordine e velocizzando la sincronizzazione.

1. Nella pagina dei dettagli del profilo, vai a **Sicurezza a livello di campo** sezione. Clic **Visualizza** per modificare l&#39;accessibilità per gli oggetti:

   * Lead
   * Contatto
   * Account
   * Opportunità

   >[!TIP]
   >
   >Puoi configurare altri oggetti in base alle esigenze della tua organizzazione.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Per ogni oggetto, fai clic su **Modifica**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Individua i campi non necessari, assicurati che **Accesso in lettura** e **Modifica accesso** sono deselezionate. Clic **Salva** quando hai finito.

   >[!NOTE]
   >
   >Modifica solo l’accessibilità per i campi personalizzati.

   ![](assets/sfdc-sync-field-edit2.png)

1. Dopo aver disabilitato tutti i campi non necessari, è necessario selezionare **Accesso in lettura e accesso in modifica** per i seguenti campi oggetto. Clic **Salva** quando hai finito.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1"><p>Oggetto</p></th> 
   <th colspan="1" rowspan="1"><p>Campi</p></th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Account</p></td> 
   <td colspan="1" rowspan="1"><p>Campo tipo</p></td> 
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

1. Digita &quot;Gestisci utenti&quot; nella barra di ricerca di navigazione, quindi fai clic su **Utenti**. Fai clic su **Nuovo utente**.

   ![](assets/sfdc-new-users.png)

1. Compila i campi obbligatori. Quindi, seleziona la **Licenza utente: Salesforce** e il profilo creato in precedenza. Clic **Salva** quando hai finito.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Viene completato il passaggio 2 di 2.

>[!NOTE]
>
>[Passaggio 3 di 3: Connessione di Marketo e Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
