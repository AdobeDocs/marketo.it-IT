---
description: Passaggio 2 di 3 - Creare un utente Salesforce per Marketo (Enterprise/Unlimited) - Documentazione Marketo - Documentazione del prodotto
title: Passaggio 2 di 3 - Creazione di un utente Salesforce per Marketo (Enterprise/Unlimited)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 4%

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

1. Fai clic su **[!UICONTROL Setup]**.

   SCHERMATA

1. Digita &quot;profiles&quot; nella barra di ricerca di navigazione e fai clic sul collegamento Profili.

   SCHERMATA

1. Fai clic su Nuovo profilo.

   SCHERMATA

1. Seleziona Utente Standard, denomina il profilo &quot;Marketo-Salesforce Sync&quot; e fai clic su Salva.

   SCHERMATA

## Imposta autorizzazioni profilo {#set-profile-permissions}

1. Fai clic su Modifica per impostare le autorizzazioni di protezione.

   SCHERMATA

1. Nella sezione Autorizzazioni amministrative verificare che siano selezionate le caselle seguenti:

   * API abilitata
   * Modifica modelli HTML
   * Gestisci documenti pubblici
   * Gestisci modelli pubblici

   >[!TIP]
   >
   >Seleziona la casella Password Never Expires (Password senza scadenza).

1. Nella sezione Autorizzazioni utente generali verificare che siano selezionate le caselle seguenti:

   * Converti lead
   * Modifica eventi
   * Modifica le Attività

1. Nella sezione Autorizzazioni oggetto standard verificare che le autorizzazioni di lettura, creazione, modifica ed eliminazione siano verificate per:

   * Account
   * Campagne
   * Contatti
   * Lead
   * Opportunità

   >[!NOTE]
   >
   >Concedi le autorizzazioni per le campagne, se intendi utilizzare Campaign Sync.

   SCHERMATA

1. Al termine, fai clic su Salva nella parte inferiore della pagina.

   SCHERMATA

## Imposta autorizzazioni campo {#set-field-permissions}

1. Rivolgiti ai tuoi esperti di marketing per scoprire quali campi personalizzati sono necessari per la sincronizzazione.

   >[!NOTE]
   >
   >Questo passaggio impedisce la visualizzazione dei campi non necessari in Marketo, riducendo il disordine e velocizzando la sincronizzazione.

1. Nella pagina dei dettagli del profilo, vai alla sezione Sicurezza a livello di campo. Fare clic su Visualizza per modificare l&#39;accessibilità per gli oggetti:

   * Lead
   * Contatto
   * Account
   * Opportunità

   >[!TIP]
   >
   >Puoi configurare altri oggetti in base alle esigenze della tua organizzazione.

1. Per ogni oggetto, fare clic su Modifica.

   SCHERMATA

1. Individuare i campi non necessari, verificare che le opzioni Accesso in lettura e Accesso in modifica siano deselezionate. Al termine, fai clic su Salva.

   >[!NOTE]
   >
   >Modifica solo l’accessibilità per i campi personalizzati.

   SCHERMATA

1. Dopo aver disattivato tutti i campi non necessari, è necessario controllare Accesso in lettura e Accesso in modifica per i seguenti campi oggetto. Al termine, fai clic su Salva.

   TABELLA

   SCHERMATA

## Crea account di sincronizzazione Marketo-Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Creare un account Salesforce dedicato (ad esempio, `marketo@yourcompany.com`) per distinguere le modifiche apportate da Marketo rispetto ad altri utenti di Salesforce.

1. Digita &quot;Gestisci utenti&quot; nella barra di ricerca di navigazione, quindi fai clic su Utenti. Fare clic su Nuovo utente.

   SCHERMATA

   SCHERMATA

1. Compila i campi obbligatori. Quindi, seleziona la Licenza utente: Salesforce e il profilo creato in precedenza. Al termine, fai clic su Salva.

   SCHERMATA

Viene completato il passaggio 2 di 3.
