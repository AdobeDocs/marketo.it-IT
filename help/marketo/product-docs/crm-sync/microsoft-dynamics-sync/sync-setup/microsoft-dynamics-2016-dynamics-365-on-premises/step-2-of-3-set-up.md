---
unique-page-id: 7504739
description: Installare Marketo per Microsoft Dynamics 2016/Dynamics 365 On-Premises Passaggio 2 di 3 - Documentazione Marketo - Documentazione del prodotto
title: Installare Marketo per Microsoft Dynamics 2016/Dynamics 365 On-Premises, passaggio 2 di 3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
source-git-commit: 1e20fdd1d3c6bba265ceabe499e0d7a4babf4ef1
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Passaggio 2 di 3: configurare Marketo per Dynamics (On-Prem 2016/Dynamics 365 On-Premises){#step-of-set-up-for-marketo-on-premises-2016}

Ottimo lavoro per completare i passaggi precedenti. Continuiamo a muoverci.

>[!PREREQUISITES]
>
>[Installare Marketo per Microsoft Dynamics 2016/Dynamics 365 On-Premises, passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegna il ruolo utente di sincronizzazione Marketo solo all&#39;utente di sincronizzazione Marketo. Non è necessario assegnarlo ad altri utenti.

>[!NOTE]
>
>Questo vale per la versione 4.0.0.14 e successive di Marketo. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare il Marketo, vedi [Aggiornare la soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Impostazione della lingua dell&#39;utente di sincronizzazione [deve essere impostato su Inglese](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Sotto **Impostazioni**, fai clic su **Sicurezza**.

   ![](assets/assign1.png)

1. Fai clic su **Utenti**.

   ![](assets/assign2.png)

1. Verrà visualizzato un elenco di utenti qui. Seleziona l’utente dedicato di Marketo Sync o contatta il tuo [Servizi federativi Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) per creare un utente dedicato per Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Seleziona l’utente di sincronizzazione. Fai clic su **Gestisci ruoli**.

   ![](assets/assign4.png)

   Selezionare Marketo Sync User e fare clic su OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Se il ruolo non viene visualizzato, torna a [passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) e importa la soluzione.

   >[!NOTE]
   >
   >Eventuali aggiornamenti effettuati nel CRM dall&#39;utente di sincronizzazione verranno **not** essere sincronizzati di nuovo in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi finito! Abbiamo solo qualche ultima configurazione prima di passare al prossimo articolo.

1. Sotto **Impostazioni**, fai clic su **Configurazione Marketo**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se manca la configurazione Marketo, prova ad aggiornare la pagina. Se il problema persiste, [pubblicare la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) oppure prova a disconnettersi ed effettuare nuovamente l&#39;accesso.

1. Fai clic su **Predefinito**.

   ![](assets/configure2.png)

1. Fai clic sul pulsante **Utente Marketo** e seleziona l&#39;utente di sincronizzazione.

   ![](assets/configure3.png)

1. Fai clic sull’icona salva nell’angolo in basso a destra.

   ![](assets/configure4.png)

1. Fai clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere al passaggio 3 {#before-proceeding-to-step}

* Se si desidera limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ora.
* Esegui il [Convalida della sincronizzazione di Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) processo. Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedi all’utente di sincronizzazione Marketo in Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installare Marketo per Microsoft Dynamics 2016/Dynamics 365 On-Premises, passaggio 3 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)