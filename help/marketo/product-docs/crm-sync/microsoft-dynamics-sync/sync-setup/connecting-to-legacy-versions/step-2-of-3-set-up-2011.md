---
unique-page-id: 3571807
description: 'Passaggio 2 di 3: configurare l''utente di Marketo Sync in [!DNL Dynamics] (2011 on-premise) - Documentazione di Marketo - Documentazione del prodotto'
title: 'Passaggio 2 di 3: configurare l''utente di Marketo Sync in [!DNL Dynamics] (2011 on-premise)'
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 1%

---

# Passaggio 2 di 3: configurare l&#39;utente di Marketo Sync in [!DNL Dynamics] (on-premise 2011) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Ottimo lavoro per completare i passaggi precedenti, continuiamo a muoverci attraverso questo.

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: installare la soluzione Marketo (on-premise 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegnare il ruolo Utente di sincronizzazione Marketo solo all&#39;utente di sincronizzazione Marketo. Non è necessario assegnarla ad altri utenti.

>[!NOTE]
>
>Questo vale per il plug-in di Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare Marketo, vedere [Aggiornare la soluzione Marketo per  [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>L&#39;impostazione della lingua dell&#39;utente di sincronizzazione [ deve essere inglese](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. Nel menu in basso a sinistra, selezionare **[!UICONTROL Settings]**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Nella struttura, selezionare **[!UICONTROL Administration]**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Seleziona **[!UICONTROL Users]**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Qui verrà visualizzato un elenco di utenti. Selezionare l&#39;utente Marketo Sync dedicato o contattare l&#39;amministratore [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) per creare un nuovo utente dedicato a Marketo. Fai clic su **[!UICONTROL Manage Roles]**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Selezionare **[!UICONTROL Marketo Sync User]** e fare clic su **[!UICONTROL OK]**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Se il ruolo non è visualizzato, torna al [passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} e importa la soluzione.

   >[!NOTE]
   >
   >Eventuali aggiornamenti apportati nel CRM dall&#39;utente di sincronizzazione _non_ verranno sincronizzati di nuovo in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi completato! Abbiamo solo alcune ultime configurazioni prima di passare al prossimo articolo.

1. Selezionare **[!UICONTROL Settings]**. Selezionare quindi **[!UICONTROL Marketo Config]** nella struttura.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Se manca [!UICONTROL Marketo Config], provare ad aggiornare la pagina. Se il problema persiste, [pubblica di nuovo la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md) oppure esci e accedi di nuovo.

1. Fai clic su **[!UICONTROL Default]**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Fai clic su ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Nel pop-up, selezionare l&#39;utente di sincronizzazione. Quindi fai clic su **[!UICONTROL OK]**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Fare clic su **[!UICONTROL Save]** per salvare le modifiche.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Fai clic su **[!UICONTROL Publish All Customizations]**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere al punto 3 {#before-proceeding-to-step}

    * Se si desidera limitare il numero di record sincronizzati, [configurare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ora.
    * Eseguire il processo [Validate [!DNL Microsoft Dynamics] Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Verifica che le impostazioni iniziali siano state eseguite correttamente.
    * Accedi all&#39;utente di Marketo Sync in [!DNL Microsoft Dynamics] CRM.

Ottimo lavoro!

>[!MORELIKETHIS]
>
>[Passaggio 3 di 3: Connessione [!DNL Microsoft Dynamics] con Marketo (2011 on-premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2011.md)
