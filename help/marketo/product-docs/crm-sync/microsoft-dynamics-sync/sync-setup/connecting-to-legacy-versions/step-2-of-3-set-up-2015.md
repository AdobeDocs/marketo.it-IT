---
unique-page-id: 7504739
description: Installare Marketo per Microsoft Dynamics 2015 On-Premises Passaggio 2 di 3 - Documentazione Marketo - Documentazione del prodotto
title: Installare Marketo per Microsoft Dynamics 2015 On-Premises, passaggio 2 di 3
exl-id: 39f00749-4ba3-47f1-b2e3-72cbaa7caf2e
source-git-commit: 19c568cdc3d31d07e42e99eb7e48f10a017b44f9
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Passaggio 2 di 3: configurare Marketo per Dynamics (On-Prem 2015){#step-of-set-up-for-marketo-on-premises-2015}

Ottimo lavoro per completare i passaggi precedenti. Continuiamo a muoverci.

>[!PREREQUISITES]
>
>[Installare Marketo per Microsoft Dynamics 2015 On-Premises, passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md)

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

1. Controlla Marketo Sync User e fai clic su **OK**.

   ![](assets/assign5.png)

   >[!IMPORTANT]
   >
   >L&#39;utente di sincronizzazione deve disporre dell&#39;autorizzazione di lettura per la configurazione Marketo.

   >[!TIP]
   >
   >Se il ruolo non viene visualizzato, torna a [passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md) e importa la soluzione.

   >[!NOTE]
   >
   >Eventuali aggiornamenti effettuati nel CRM dall&#39;utente di sincronizzazione verranno **not** essere sincronizzati di nuovo in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi finito! Abbiamo solo qualche ultima configurazione prima di passare al prossimo articolo.

1. Sotto **Impostazioni**, fai clic su **Configurazione Marketo**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se manca la configurazione Marketo, prova ad aggiornare la pagina. Se il problema persiste, [pubblicare la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md) oppure prova a disconnettersi ed effettuare nuovamente l&#39;accesso.

1. Fai clic su **Predefinito**.

   ![](assets/configure2.png)

1. Fai clic sul pulsante **Utente Marketo** e seleziona l’utente di sincronizzazione.

   ![](assets/configure3.png)

1. Fai clic sull’icona salva nell’angolo in basso a destra.

   ![](assets/configure4.png)

1. Fai clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/publish-all-customizations1.png)

   >[!NOTE]
   >
   >L&#39;utente di sincronizzazione deve disporre dell&#39;autorizzazione di lettura per la configurazione Marketo.

## Prima di procedere al passaggio 3 {#before-proceeding-to-step}

* Se si desidera limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ora.
* Esegui il [Convalida della sincronizzazione di Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) processo. Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedi all’utente di sincronizzazione Marketo in Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installare Marketo per Microsoft Dynamics 2015 On-Premises, passaggio 3 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect-2015.md)
