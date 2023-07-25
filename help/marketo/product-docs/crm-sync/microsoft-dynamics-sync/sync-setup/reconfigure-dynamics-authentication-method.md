---
description: Riconfigura metodo di autenticazione Dynamics - Documentazione di Marketo - Documentazione del prodotto
title: Riconfigura metodo di autenticazione Dynamics
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Riconfigura metodo di autenticazione Dynamics {#reconfigure-dynamics-authentication-method}

Per aggiornare il metodo di autenticazione Dynamics, segui la procedura riportata di seguito.

>[!PREREQUISITES]
>
>Configurare l&#39;applicazione in Microsoft Dynamics e Active Directory (Azure AD/ADFS) utilizzando il metodo di autenticazione desiderato da uno degli articoli seguenti:
>
>* [Passaggio 2 di 3: configurare una soluzione Marketo con connessione server-server](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)
>* [Passaggio 2 di 4: configurare la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)

1. In Marketo fai clic su **Amministratore**.

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. Clic **Microsoft Dynamics**, quindi **Disattiva sincronizzazione**.

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >Per aggiornare il metodo di autenticazione, è necessario disattivare temporaneamente la sincronizzazione globale.

1. Fai clic su **Riconfigura nuovo metodo di autenticazione** scheda.

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. Seleziona il nuovo metodo di autenticazione desiderato (in questo esempio stiamo scegliendo API web).

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. Immettere le credenziali richieste per il nuovo metodo di autenticazione e fare clic su **Convalida**.

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* I campi specifici variano a seconda del metodo di autenticazione scelto e il modulo viene aggiornato automaticamente a seconda del metodo di autenticazione precedente.
   >* Se hai sincronizzato in precedenza, i dati nel modulo di cui sopra possono essere precompilati. Immetti nuovamente tutte le credenziali per garantire i valori corretti.

1. Se tutto funziona correttamente, la funzione Convalida sincronizzazione genererà tutti i segni di spunta verdi ![](assets/green-check.png). Rivedi il messaggio e fai clic su **Switch** per aggiornare il metodo di autenticazione.

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >Se viene visualizzata una ![](assets/red-x.png), questo passaggio presenta un problema. Consulta [Correggi i problemi di sincronizzazione della convalida Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) per identificare e risolvere i problemi. Quindi esegui nuovamente i passaggi di convalida della sincronizzazione fino a quando il risultato non si presenta come nell’immagine precedente.

1. Clic **Conferma** per procedere.

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. Clic **Conferma** di nuovo.

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. Clic **OK**.

   >[!IMPORTANT]
   >
   >Il sistema impiega 15 minuti per accettare la nuova modalità di autenticazione. Attendere 15 minuti dall&#39;ora dello switch prima di riattivare la sincronizzazione.
