---
unique-page-id: 7504739
description: Installazione di Marketo per Microsoft Dynamics 2015 on-premises Passaggio 2 di 3 - Documentazione di Marketo - Documentazione del prodotto
title: Installazione di Marketo per Microsoft Dynamics 2015 on-premise - Passaggio 2 di 3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Passaggio 2 di 3: configurazione di Marketo per Dynamics (on-prem 2015){#step-of-set-up-for-marketo-on-premises-2015}

Ottimo lavoro per completare i passaggi precedenti. Continuiamo a muoverci in questa direzione.

>[!PREREQUISITES]
>
>[Installazione di Marketo per Microsoft Dynamics 2015 on-premise - Passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegnare il ruolo Utente di sincronizzazione Marketo solo all&#39;utente di sincronizzazione Marketo. Non è necessario assegnarla ad altri utenti.

>[!NOTE]
>
>Questo vale per Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare il Marketo, consulta [Aggiornamento della soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Impostazione della lingua dell&#39;utente di sincronizzazione [deve essere impostato su English](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Sotto **[!UICONTROL Impostazioni]**, fai clic su **[!UICONTROL Sicurezza]**.

   ![](assets/assign1.png)

1. Clic **[!UICONTROL Utenti]**.

   ![](assets/assign2.png)

1. Qui verrà visualizzato un elenco di utenti. Selezionare l&#39;utente Marketo Sync dedicato o contattare il [Servizi federativi Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS) per creare un utente dedicato per Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selezionare l&#39;utente di sincronizzazione. Clic **[!UICONTROL Gestisci ruoli]**.

   ![](assets/assign4.png)

1. Controlla l’utente di Marketo Sync e fai clic su **[!UICONTROL OK]**.

   ![](assets/assign5.png)

   >[!IMPORTANT]
   >
   >L&#39;utente Sync deve disporre dell&#39;autorizzazione di lettura per la configurazione di Marketo.

   >[!TIP]
   >
   >Se non vedi il ruolo, torna a [passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} e importa la soluzione.

   >[!NOTE]
   >
   >Qualsiasi aggiornamento effettuato nel CRM dall&#39;utente di sincronizzazione _non_ essere sincronizzato di nuovo in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi completato! Abbiamo solo alcune ultime configurazioni prima di passare al prossimo articolo.

1. Sotto **[!UICONTROL Impostazioni]**, fai clic su **[!UICONTROL Configurazione Marketo]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se manca la configurazione Marketo, prova ad aggiornare la pagina. Se il problema persiste, [pubblicare la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"} oppure disconnettersi e accedere di nuovo.

1. Clic **[!UICONTROL Predefinito]**.

   ![](assets/configure2.png)

1. Fai clic su **[!UICONTROL Utente Marketo]** e selezionare l&#39;utente di sincronizzazione.

   ![](assets/configure3.png)

1. Fai clic sull’icona Salva nell’angolo in basso a destra.

   ![](assets/configure4.png)

1. Clic **[!UICONTROL Pubblica tutte le personalizzazioni]**.

   ![](assets/publish-all-customizations1.png)

   >[!NOTE]
   >
   >L&#39;utente Sync deve disporre dell&#39;autorizzazione di lettura per la configurazione di Marketo.

## Prima di procedere al punto 3 {#before-proceeding-to-step}

* Se si desidera limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} ora.
* Esegui il [Convalida sincronizzazione Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} processo. Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedere a Marketo Sync User in Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installazione di Marketo per Microsoft Dynamics 2015 on-premise - Passaggio 3 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md){target="_blank"}
