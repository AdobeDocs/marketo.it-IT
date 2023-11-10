---
unique-page-id: 3571807
description: 'Passaggio 2 di 3: configurare l’utente di Marketo Sync in Dynamics (on-premises 2011) - Documentazione di Marketo - Documentazione del prodotto'
title: 'Passaggio 2 di 3: configurare l''utente di Marketo Sync in Dynamics (on-premises 2011)'
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---

# Passaggio 2 di 3: configurare l’utente di Marketo Sync in Dynamics (on-premises 2011) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Ottimo lavoro per completare i passaggi precedenti, continuiamo a muoverci attraverso questo.

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: installare la soluzione Marketo (on-premise 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"}

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegnare il ruolo Utente di sincronizzazione Marketo solo all&#39;utente di sincronizzazione Marketo. Non è necessario assegnarla ad altri utenti.

>[!NOTE]
>
>Questo vale per il plug-in Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare Marketo, consulta [Aggiornamento della soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Impostazione della lingua dell&#39;utente di sincronizzazione [deve essere impostato su English](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Nel menu in basso a sinistra, seleziona **[!UICONTROL Impostazioni]**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Nella struttura, seleziona **[!UICONTROL Amministrazione]**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Seleziona **[!UICONTROL Utenti]**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Qui verrà visualizzato un elenco di utenti. Selezionare l&#39;utente Marketo Sync dedicato o contattare il [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} per creare un nuovo utente dedicato a Marketo. Clic **[!UICONTROL Gestisci ruoli]**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Verifica **[!UICONTROL Utente Marketo Sync]** e fai clic su **[!UICONTROL OK]**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Se non vedi il ruolo, torna a [passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} e importa la soluzione.

   >[!NOTE]
   >
   >Qualsiasi aggiornamento effettuato nel CRM dall&#39;utente di sincronizzazione _non_ essere sincronizzato di nuovo in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi completato! Abbiamo solo alcune ultime configurazioni prima di passare al prossimo articolo.

1. Seleziona **[!UICONTROL Impostazioni]**. Quindi seleziona **[!UICONTROL Configurazione Marketo]** nell&#39;albero.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Se manca la configurazione Marketo, prova ad aggiornare la pagina. Se il problema persiste, [pubblicare di nuovo la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md){target="_blank"} oppure disconnettiti e accedi di nuovo.

1. Clic **[!UICONTROL Predefinito]**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Fai clic su ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Nel pop-up, selezionare l&#39;utente di sincronizzazione. Quindi fai clic su **[!UICONTROL OK]**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Clic **[!UICONTROL Salva]** per salvare le modifiche.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Clic **[!UICONTROL Pubblica tutte le personalizzazioni]**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere al punto 3 {#before-proceeding-to-step}

* Se si desidera limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} ora.
* Esegui il [Convalida sincronizzazione Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} processo. Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedere a Marketo Sync User in Microsoft Dynamics CRM.

  Ottimo lavoro!

>[!MORELIKETHIS]
>
>[Passaggio 3 di 3: collegare Microsoft Dynamics a Marketo (on-premise 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2011.md){target="_blank"}
