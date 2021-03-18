---
unique-page-id: 7504739
description: Installa Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 2 di 3 - Documenti Marketo - Documentazione del prodotto
title: Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 2 di 3
translation-type: tm+mt
source-git-commit: 9d8a6d9880de5d2af211906c2410f2057c1f454d
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---


# Passaggio 2 di 3: configurare Marketo per Dynamics (On-Prem 2015 e On-Prem 2016 365){#step-of-set-up-for-marketo-on-premises-and-365}

Ottimo lavoro per completare i passaggi precedenti. Continuiamo a muoverci.

>[!PREREQUISITES]
>
>[Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegna il ruolo Utente sincronizzazione Marketo solo all’utente di sincronizzazione Marketo. Non è necessario assegnarlo ad altri utenti.

>[!NOTE]
>
>Questo vale per Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare Marketo, consulta [Aggiornare la soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. In **Impostazioni**, fai clic su **Sicurezza**.

   ![](assets/assign1.png)

1. Fare clic su **Utenti**.

   ![](assets/assign2.png)

1. Verrà visualizzato un elenco di utenti qui. Selezionare l&#39;utente dedicato di Marketo Sync o contattare l&#39;amministratore [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) per creare un utente dedicato per Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Seleziona l’utente di sincronizzazione. Fare clic su **Gestisci ruoli**.

   ![](assets/assign4.png)

   Selezionare Utente sincronizzazione Marketo e fare clic su OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Se il ruolo non viene visualizzato, tornare al [passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) e importare la soluzione.

   >[!NOTE]
   >
   >Eventuali aggiornamenti effettuati nel CRM dall&#39;utente di sincronizzazione **non** verranno sincronizzati nuovamente in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi finito! Abbiamo solo qualche ultima configurazione prima di passare al prossimo articolo.

1. In **Impostazioni**, fai clic su **Configurazione Marketo**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se manca la configurazione Marketo, prova ad aggiornare la pagina. Se il problema persiste, [pubblicare la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-1-of-3-install.md) oppure provare a disconnettersi e riprovare.

1. Fare clic su **Predefinito**.

   ![](assets/configure2.png)

1. Fai clic sul campo **Marketo User** e seleziona l&#39;utente di sincronizzazione.

   ![](assets/configure3.png)

1. Fai clic sull’icona salva nell’angolo in basso a destra.

   ![](assets/configure4.png)

1. Fai clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere al passaggio 3 {#before-proceeding-to-step}

* Per limitare il numero di record sincronizzati, [imposta ora un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
* Esegui il processo [Convalida Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) . Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedi all’utente di sincronizzazione Marketo in Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 3 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
