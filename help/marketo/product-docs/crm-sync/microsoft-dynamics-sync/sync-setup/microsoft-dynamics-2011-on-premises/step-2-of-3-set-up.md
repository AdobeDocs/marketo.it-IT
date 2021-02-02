---
unique-page-id: 3571807
description: Passaggio 2 di 3 - Configurare Marketo Sync User in Dynamics (On-Premises 2011) - Marketo Docs - Documentazione prodotto
title: Passaggio 2 di 3 - Imposta Marketo Sync User in Dynamics (On-Premises 2011)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---


# Passaggio 2 di 3: Impostazione della sincronizzazione degli utenti di Marketing in Dynamics (On-Premises 2011) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Ottimo lavoro per completare i passaggi precedenti, continuiamo a farlo.

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: Installare la soluzione Marketo (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)

## Assegna ruolo utente sincronizzazione {#assign-sync-user-role}

Assegnate il ruolo di sincronizzazione utente Marketo solo all’utente di sincronizzazione Marketo. Non è necessario assegnarlo ad altri utenti.

>[!NOTE]
>
>Questo vale per il plug-in Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo di utente di sincronizzazione. Per aggiornare Marketo, vedere [Aggiornamento della soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Nel menu in basso a sinistra, selezionare **Impostazioni**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Nella struttura ad albero, selezionare **Amministrazione**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Selezionare **Utenti**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Verrà visualizzato un elenco di utenti qui. Selezionate l&#39;utente dedicato di sincronizzazione di Marketo o contattate l&#39;amministratore di [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) per creare un nuovo utente dedicato a Marketo. Fare clic su **Gestisci ruoli**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Selezionare **Marketo Sync User** e fare clic su **OK**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Se il ruolo non è visualizzato, tornare al [passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) e importare la soluzione.

   >[!NOTE]
   >
   >Eventuali aggiornamenti effettuati in CRM dall&#39;utente di sincronizzazione **non** verranno sincronizzati nuovamente in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi fatto! Abbiamo solo qualche ultima configurazione prima di passare all&#39;articolo successivo.

1. Selezionare **Settings**. Selezionare **Configurazione marketing** nella struttura.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Se manca la configurazione Marketo, provare ad aggiornare la pagina. Se il problema persiste, [pubblicare nuovamente la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md) oppure disconnettersi e rientrare.

1. Fare clic su **Default**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Fare clic su ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Nella finestra a comparsa, selezionate l’utente di sincronizzazione. Fare clic su **OK**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Fare clic su **Salva** per salvare le modifiche.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Fate clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere al passaggio 3 {#before-proceeding-to-step}

    * Se si desidera limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ora.
    * Eseguire il processo [Validate Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Verifica che le impostazioni iniziali siano state eseguite correttamente.
    * Accedere all&#39;utente di sincronizzazione Marketo in Microsoft Dynamics CRM.

Ottimo lavoro!

>[!MORELIKETHIS]
>
>[Passaggio 3 di 3: Connect Microsoft Dynamics con Marketo (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-3-of-3-connect.md)
