---
unique-page-id: 2360364
description: Passaggio 2 di 3 - Crea un utente Salesforce per Marketo (Enterprise/Unlimited) - Marketo Docs - Documentazione prodotto
title: Passaggio 2 di 3 - Crea un utente Salesforce per Marketo (Enterprise/Unlimited)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# Passaggio 2 di 3: Crea un utente Salesforce per Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Questi passaggi devono essere completati da un amministratore Salesforce

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: Aggiungi campi Marketo a Salesforce (Enterprise/Unlimited)](step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

>



In questo articolo, configurerai le autorizzazioni utente nel profilo Salesforce e creerai un account di integrazione Marketing-Salesforce.

## Creazione di un profilo {#create-a-profile}

1. Fate clic su **Configurazione**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Digita &quot;profili&quot; nella barra di ricerca Nav e fai clic sul collegamento **Profili** .

   ![](assets/sfdc-profiles-hands.png)

1. Fate clic su **Nuovo**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Selezionate Utente **** standard, denominate il profilo &quot;Sincronizzazione Marketo-Salesforce&quot; e fate clic su **Salva**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Imposta autorizzazioni profilo {#set-profile-permissions}

1. Fate clic su **Modifica** per impostare le autorizzazioni di protezione.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Nella sezione Autorizzazioni **** amministrative, accertatevi che le caselle seguenti siano selezionate:

   * API abilitata
   * Modifica modelli HTML
   * Gestisci documenti pubblici
   * Gestisci modelli pubblici

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Accertatevi di selezionare la casella **Password never Expires** (Password non scadrà mai).

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

1. Al termine, fate clic su **Salva** nella parte inferiore della pagina.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Imposta autorizzazioni campo {#set-field-permissions}

1. Consulta i tuoi esperti di marketing per scoprire quali campi personalizzati sono necessari per la sincronizzazione.

   >[!NOTE]
   >
   >Questo passaggio impedisce la visualizzazione dei campi non necessari in Marketo, riducendo il disordine e velocizzando la sincronizzazione.

1. Nella pagina dei dettagli del profilo, andate alla sezione Protezione **a livello di** campo. Fare clic su **Visualizza** per modificare l&#39;accessibilità per gli oggetti:

   * `Lead`
   * `Contact`
   * `Account`
   * `Opportunity`

   >[!TIP]
   >
   >È possibile configurare altri oggetti in base alle esigenze aziendali.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Per ciascun oggetto, fare clic su **Modifica**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Individuare i campi non necessari, assicurarsi che **Accesso lettura **** e Accesso modifica **siano deselezionati. Al termine, fate clic su **Salva** .

   >[!NOTE]
   >
   >**Promemoria**
   >
   >
   >Modificate solo l&#39;accessibilità per i campi personalizzati.

   ![](assets/sfdc-sync-field-edit2.png)

1. Dopo aver disattivato tutti i campi non necessari, è necessario selezionare **Accesso lettura e Accesso modifica **per i campi oggetto seguenti. Al termine, fate clic su **Salva** .

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
>Crea un account Salesforce dedicato (ad es. [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#89e4e8fbe2ecfde6c9f0e6fcfbeae6e4f9e8e7f0a7eae6e4)) per distinguere le modifiche apportate da Marketo rispetto ad altri utenti Salesforce.

1. Digita &quot;Gestisci utenti&quot; nella barra di ricerca Nav, quindi fai clic su **Utenti**. Fate clic su **Nuovo utente**.

   ![](assets/sfdc-new-users.png)

1. Compilate i campi richiesti. Selezionate quindi Licenza **utente: Salesforce** e il profilo precedentemente creato. Al termine, fate clic su **Salva** .

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Il passaggio 2 di 2 è completato.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Passaggio 3 di 3: Connect Marketo e Salesforce (Enterprise/Unlimited)](step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)

>



