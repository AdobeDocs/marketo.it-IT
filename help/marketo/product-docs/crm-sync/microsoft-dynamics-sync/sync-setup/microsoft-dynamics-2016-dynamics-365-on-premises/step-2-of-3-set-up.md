---
description: Installazione di Marketo per Microsoft Dynamics 2016/Dynamics 365 on-premises Passaggio 2 di 3 - Documentazione di Marketo - Documentazione del prodotto
title: Installazione di Marketo per Microsoft Dynamics 2016/Dynamics 365 on-premises Passaggio 2 di 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Passaggio 2 di 3: configurazione di Marketo per Dynamics (on-prem/Dynamics 365 on-premise 2016){#step-of-set-up-for-marketo-on-premises-2016}

Ottimo lavoro per completare i passaggi precedenti. Continuiamo a muoverci in questa direzione.

>[!PREREQUISITES]
>
>[Installazione di Marketo per Microsoft Dynamics 2016/Dynamics 365 on-premises Passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Crea un nuovo utente {#create-a-new-user}

1. Accedi a Dynamics. Fai clic sull’icona Impostazioni e seleziona Impostazioni avanzate.

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Clic **Impostazioni** e seleziona **Sicurezza**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Clic **Utenti**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Clic **Nuovo**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Clic **Aggiungi e concedi licenze agli utenti**. Dovrebbe aprirsi una nuova scheda.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Clic **Amministratore** nella parte superiore della pagina. Viene aperta un’altra nuova scheda.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Clic **Aggiungi un utente**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Immettere tutte le informazioni. Al termine, fai clic su **Aggiungi**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Questo nome deve essere un utente di sincronizzazione dedicato e non un account utente CRM esistente. Non deve essere un indirizzo e-mail effettivo.

1. Immetti l’e-mail per ricevere le nuove credenziali utente e fai clic su Invia e-mail e chiudi.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Creare una nuova applicazione client {#create-a-new-client-application}

Segui i passaggi descritti in [questo articolo di Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later) per creare una nuova applicazione client e concedere le autorizzazioni. Prendi nota dell’ID client/segreto dell’applicazione client Dynamics.

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegnare il ruolo Utente di sincronizzazione Marketo solo all&#39;utente di sincronizzazione Marketo. Non è necessario assegnarla ad altri utenti.

>[!NOTE]
>
>Questo vale per Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare il Marketo, consulta [Aggiornamento della soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Impostazione della lingua dell&#39;utente di sincronizzazione [deve essere impostato su English](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Sotto **Impostazioni**, fai clic su **Sicurezza**.

   ![](assets/assign1.png)

1. Clic **Utenti**.

   ![](assets/assign2.png)

1. Qui verrà visualizzato un elenco di utenti. Selezionare l&#39;utente Marketo Sync dedicato o contattare il [Servizi federativi Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) per creare un utente dedicato per Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selezionare l&#39;utente di sincronizzazione. Clic **Gestisci ruoli**.

   ![](assets/assign4.png)

   Selezionare Marketo Sync User e fare clic su OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Se non vedi il ruolo, torna a [passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) e importa la soluzione.

   >[!NOTE]
   >
   >Qualsiasi aggiornamento effettuato nel CRM dall&#39;utente di sincronizzazione **non** essere sincronizzato di nuovo in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi completato! Abbiamo solo alcune ultime configurazioni prima di passare al prossimo articolo.

1. Sotto **Impostazioni**, fai clic su **Configurazione Marketo**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se manca la configurazione Marketo, prova ad aggiornare la pagina. Se il problema persiste, [pubblicare la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) oppure disconnettersi e accedere di nuovo.

1. Clic **Predefinito**.

   ![](assets/configure2.png)

1. Fai clic su **Utente Marketo** e selezionare l&#39;utente di sincronizzazione.

   ![](assets/configure3.png)

1. Fai clic sull’icona Salva nell’angolo in basso a destra.

   ![](assets/configure4.png)

1. Clic **Pubblica tutte le personalizzazioni**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere al punto 3 {#before-proceeding-to-step}

* Se si desidera limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ora.
* Esegui il [Convalida sincronizzazione Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) processo. Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedere a Marketo Sync User in Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installazione di Marketo per Microsoft Dynamics 2016/Dynamics 365 on-premises Passaggio 3 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
