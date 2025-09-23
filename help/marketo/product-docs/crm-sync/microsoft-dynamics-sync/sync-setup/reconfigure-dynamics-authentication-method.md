---
description: Riconfigura [!DNL Dynamics] Metodo di autenticazione - Documentazione di Marketo - Documentazione del prodotto
title: Riconfigura [!DNL Dynamics] Metodo di autenticazione
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 1%

---

# Riconfigurare il metodo di autenticazione Dynamics {#reconfigure-dynamics-authentication-method}

Per aggiornare il metodo di autenticazione [!DNL Dynamics], attenersi alla procedura riportata di seguito.

>[!PREREQUISITES]
>
>Configurare l&#39;applicazione in [!DNL Microsoft Dynamics] e Active Directory (Azure AD/ADFS) utilizzando il metodo di autenticazione desiderato da uno degli articoli seguenti:
>
>* [Passaggio 2 di 3: configurare una soluzione Marketo con connessione server-server](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}
>* [Passaggio 2 di 4: configurare la soluzione Marketo con la connessione di controllo password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. In Marketo fare clic su **[!UICONTROL Admin]**.

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. Fai clic su **Microsoft Dynamics**, quindi su **[!UICONTROL Disable Sync]**.

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >Per aggiornare il metodo di autenticazione, è necessario disattivare temporaneamente la sincronizzazione globale.

1. Fare clic sulla scheda **[!UICONTROL Reconfigure New Auth Method]**.

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. Seleziona il nuovo metodo di autenticazione desiderato (in questo esempio stiamo scegliendo API web).

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. Immettere le credenziali richieste per il nuovo metodo di autenticazione e fare clic su **[!UICONTROL Validate]**.

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* I campi specifici variano a seconda del metodo di autenticazione scelto e il modulo viene aggiornato automaticamente a seconda del metodo di autenticazione precedente.
   >* Se hai eseguito la sincronizzazione in precedenza, i dati nel modulo di cui sopra potrebbero essere precompilati. Immetti nuovamente tutte le credenziali per garantire i valori corretti.

1. Se tutto funziona correttamente, la sincronizzazione di convalida genererà tutti i segni di spunta verdi ![](assets/green-check.png). Rivedere il messaggio e fare clic su **[!UICONTROL Switch]** per aggiornare il metodo di autenticazione.

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >Se viene visualizzato un ![](assets/red-x.png), il passaggio presenta un problema. Consulta [Correzione [!DNL Dynamics] Problemi di sincronizzazione della convalida](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) per identificare e risolvere i problemi. Quindi esegui nuovamente i passaggi di convalida della sincronizzazione fino a quando il risultato non si presenta come nell’immagine precedente.

1. Fare clic su **[!UICONTROL Confirm]** per continuare.

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. Fare di nuovo clic su **[!UICONTROL Confirm]**.

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. Fai clic su **[!UICONTROL OK]**.

   >[!IMPORTANT]
   >
   >Il sistema impiega 15 minuti per accettare la nuova modalità di autenticazione. Attendere 15 minuti dall&#39;ora dello switch prima di riattivare la sincronizzazione.
