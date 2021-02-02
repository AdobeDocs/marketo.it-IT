---
unique-page-id: 2360364
description: Passaggio 2 di 3 - Crea un utente Salesforce per Marketo (Enterprise/Unlimited) - Marketo Docs - Documentazione prodotto
title: Passaggio 2 di 3 - Crea un utente Salesforce per Marketo (Enterprise/Unlimited)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---


# Passaggio 2 di 3: Crea un utente Salesforce per Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Questi passaggi devono essere completati da un amministratore Salesforce

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: Aggiungi campi Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

In questo articolo, configurerai le autorizzazioni utente nel profilo Salesforce e creerai un account di integrazione Marketing-Salesforce.

## Creare un profilo {#create-a-profile}

1. Fare clic su **Setup**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Digitare &quot;profili&quot; nella barra di ricerca di Nav e fare clic sul collegamento **Profili**.

   ![](assets/sfdc-profiles-hands.png)

1. Fare clic su **Nuovo**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Selezionare **Utente standard**, assegnare un nome al profilo &quot;Marketing-Salesforce Sync&quot; e fare clic su **Salva**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Imposta autorizzazioni profilo {#set-profile-permissions}

1. Fare clic su **Modifica** per impostare le autorizzazioni di protezione.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Nella sezione **Autorizzazioni amministrative**, verificare che le caselle seguenti siano selezionate:

   * API abilitata
   * Modifica modelli HTML
   * Gestisci documenti pubblici
   * Gestisci modelli pubblici

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Controllare la casella **Password never Expires**.

1. Nella sezione Autorizzazioni utente generali, accertatevi che le caselle seguenti siano selezionate:

   * Converti lead
   * Modifica eventi
   * Modifica attività

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Nella sezione Autorizzazioni oggetto standard, accertatevi che le autorizzazioni Lettura, Crea, Modifica ed Elimina siano verificate per:

   * Account
   * Campagne
   * Contatti
   * Lead
   * Opportunità

   >[!NOTE]
   >
   >Se intendete utilizzare la sincronizzazione delle campagne, assegnate le autorizzazioni per le campagne.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Al termine, fare clic su **Salva** nella parte inferiore della pagina.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Imposta autorizzazioni campo {#set-field-permissions}

1. Consulta i tuoi esperti di marketing per scoprire quali campi personalizzati sono necessari per la sincronizzazione.

   >[!NOTE]
   >
   >Questo passaggio impedisce la visualizzazione dei campi non necessari in Marketo, riducendo il disordine e velocizzando la sincronizzazione.

1. Nella pagina dei dettagli del profilo, andate alla sezione **Sicurezza a livello di campo**. Fare clic su **Visualizza** per modificare l&#39;accessibilità per gli oggetti:

   * Lead
   * Contatto
   * Account
   * Opportunità

   >[!TIP]
   >
   >È possibile configurare altri oggetti in base alle esigenze aziendali.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Per ciascun oggetto, fare clic su **Modifica**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Individuare i campi non necessari, assicurarsi che **Accesso in lettura** e **Accesso in modifica** siano deselezionati. Al termine, fate clic su **Salva**.

   >[!NOTE]
   >
   >Modificate solo l&#39;accessibilità per i campi personalizzati.

   ![](assets/sfdc-sync-field-edit2.png)

1. Dopo aver disattivato tutti i campi non necessari, è necessario controllare **Accesso in lettura e Accesso in modifica** per i seguenti campi oggetto. Al termine, fate clic su **Salva**.

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

## Crea account di sincronizzazione Marketing-Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Crea un account Salesforce dedicato (ad esempio, marketo@yourcompany.com) per distinguere le modifiche apportate da Marketo rispetto ad altri utenti di Salesforce.

1. Digita &quot;Gestisci utenti&quot; nella barra di ricerca Nav, quindi fai clic su **Utenti**. Fare clic su **Nuovo utente**.

   ![](assets/sfdc-new-users.png)

1. Compilate i campi richiesti. Selezionate quindi la **Licenza utente: Salesforce** e il profilo creato in precedenza. Al termine, fate clic su **Salva**.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Il passaggio 2 di 2 è completato.

>[!NOTE]
>
>[Passaggio 3 di 3: Connect Marketo e Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
