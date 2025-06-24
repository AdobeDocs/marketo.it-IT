---
description: Installazione di Marketo per Microsoft Dynamics 2016/Dynamics 365 on-premises Passaggio 2 di 3 - Documentazione di Marketo - Documentazione del prodotto
title: Installazione di Marketo per Microsoft Dynamics 2016/Dynamics 365 on-premises Passaggio 2 di 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 1%

---

# Passaggio 2 di 3: configurazione di Marketo per Dynamics (on-prem/Dynamics 365 on-premise 2016){#step-of-set-up-for-marketo-on-premises-2016}

Ottimo lavoro per completare i passaggi precedenti. Continuiamo a muoverci in questa direzione.

>[!PREREQUISITES]
>
>[Installa Marketo per Microsoft Dynamics 2016/Dynamics 365 On-Premises Passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}

## Crea un nuovo utente {#create-a-new-user}

1. Accedi a Dynamics. Fai clic sull’icona Impostazioni e seleziona Impostazioni avanzate.

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Fare clic su **[!UICONTROL Settings]** e selezionare **[!UICONTROL Security]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Fai clic su **[!UICONTROL Users]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Fai clic su **[!UICONTROL New]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Fare clic su **[!UICONTROL Add and License Users]**. Dovrebbe aprirsi una nuova scheda.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Fai clic su **[!UICONTROL Admin]** nella parte superiore della pagina. Viene aperta un’altra nuova scheda.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Fai clic su **[!UICONTROL Add a user]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Immettere tutte le informazioni. Al termine, fare clic su **[!UICONTROL Add]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Questo nome deve essere un utente di sincronizzazione dedicato e non un account utente CRM esistente. Non deve essere un indirizzo e-mail effettivo.

1. Immetti l’e-mail per ricevere le nuove credenziali utente e fai clic su Invia e-mail e chiudi.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Creare una nuova applicazione client {#create-a-new-client-application}

Segui i passaggi descritti in [questo articolo di Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later){target="_blank"} per creare una nuova applicazione client e concedere le autorizzazioni. Prendi nota dell’ID client/segreto dell’applicazione client Dynamics.

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegnare il ruolo Utente di sincronizzazione Marketo solo all&#39;utente di sincronizzazione Marketo. Non è necessario assegnarla ad altri utenti.

>[!NOTE]
>
>Applicabile a Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare il Marketo, vedi [Aggiornare la soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>L&#39;impostazione della lingua dell&#39;utente di sincronizzazione [ deve essere inglese](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. In **[!UICONTROL Settings]**, fare clic su **[!UICONTROL Security]**.

   ![](assets/assign1.png)

1. Fai clic su **[!UICONTROL Users]**.

   ![](assets/assign2.png)

1. Qui verrà visualizzato un elenco di utenti. Selezionare l&#39;utente Marketo Sync dedicato o contattare l&#39;amministratore di [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS) per creare un utente dedicato per Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selezionare l&#39;utente di sincronizzazione. Fai clic su **[!UICONTROL Manage Roles]**.

   ![](assets/assign4.png)

1. Controllare l&#39;utente di Marketo Sync e fare clic su **[!UICONTROL OK]**.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Se il ruolo non è visualizzato, torna al [passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) e importa la soluzione.

   >[!NOTE]
   >
   >Eventuali aggiornamenti apportati nel CRM dall&#39;utente di sincronizzazione _non_ verranno sincronizzati di nuovo in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi completato! Abbiamo solo alcune ultime configurazioni prima di passare al prossimo articolo.

1. In **[!UICONTROL Settings]**, fare clic su **[!UICONTROL Marketo Config]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se manca la configurazione Marketo, prova ad aggiornare la pagina. Se il problema persiste, [pubblicare la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"} o provare a disconnettersi e ad accedere di nuovo.

1. Fai clic su **[!UICONTROL Default]**.

   ![](assets/configure2.png)

1. Fare clic sul campo **[!UICONTROL Marketo User]** e selezionare l&#39;utente di sincronizzazione.

   ![](assets/configure3.png)

1. Fai clic sull’icona Salva nell’angolo in basso a destra.

   ![](assets/configure4.png)

1. Fai clic su **[!UICONTROL Publish All Customizations]**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere al punto 3 {#before-proceeding-to-step}

* Se si desidera limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}.
* Eseguire il processo [Convalida sincronizzazione Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedere a Marketo Sync User in Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installa Marketo per Microsoft Dynamics 2016/Dynamics 365 on-premise Passaggio 3 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md){target="_blank"}
