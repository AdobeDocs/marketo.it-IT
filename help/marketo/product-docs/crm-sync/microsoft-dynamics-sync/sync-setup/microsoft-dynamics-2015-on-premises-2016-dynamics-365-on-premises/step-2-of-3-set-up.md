---
unique-page-id: 7504739
description: Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 2 di 3 - Marketo Docs - Documentazione prodotto
title: Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 2 di 3
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---


# Passaggio 2 di 3

<!--Install Marketo for Dynamics 2015 On-Prem and 2016 365 On-Prem Step 2 of 3-->

Ottimo lavoro per completare i passaggi precedenti. Continuiamo a farlo.

>[!NOTE]
>
>**Prerequisiti**
>
>* [Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 1 di 3](step-1-of-3-install.md)

>



## Assegna ruolo utente sincronizzazione {#assign-sync-user-role}

Assegnate il ruolo di sincronizzazione utente Marketo solo all’utente di sincronizzazione Marketo. Non è necessario assegnarlo ad altri utenti.

>[!NOTE]
>
>Questo vale per Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo di utente di sincronizzazione. Per aggiornare Marketo, consulta [Aggiornamento della soluzione Marketo per Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. In **Impostazioni**, fate clic su **Protezione**.

   ![](assets/assign1.png)

1. Fate clic su **Utenti**.

   ![](assets/assign2.png)

1. Verrà visualizzato un elenco di utenti qui. Seleziona l&#39;utente dedicato di Marketing per la sincronizzazione o contatta il tuo amministratore ADFS ( [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)) per creare un utente dedicato per Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selezionate l’utente di sincronizzazione. Fate clic su **Gestisci ruoli**.

   ![](assets/assign4.png)

   Selezionate Marketo Sync User (Sincronizza utente) e fate clic su OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Se il ruolo non viene visualizzato, tornate al [punto 1 di 3](step-1-of-3-install.md) e importate la soluzione.

   >[!NOTE]
   >
   >Eventuali aggiornamenti apportati in CRM dall&#39;utente di sincronizzazione **non** verranno sincronizzati di nuovo su Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi fatto! Abbiamo solo qualche ultima configurazione prima di passare all&#39;articolo successivo.

1. In **Impostazioni**, fai clic su Configurazione **Marketo**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se manca la configurazione Marketo, provare ad aggiornare la pagina. Se il problema persiste, [pubblicate la soluzione](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) Marketo o provate a disconnettersi e rientrare.

1. Fate clic su **Predefinito**.

   ![](assets/configure2.png)

1. Fate clic sul campo **Marketo utente** e selezionate l’utente di sincronizzazione.

   ![](assets/configure3.png)

1. Fate clic sull&#39;icona Salva nell&#39;angolo in basso a destra.

   ![](assets/configure4.png)

1. Fate clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere allo stadio 3 {#before-proceeding-to-step}

* Se desiderate limitare il numero di record da sincronizzare, [impostate ora un filtro](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) di sincronizzazione personalizzato.
* Eseguire il processo [Validate Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) . Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedi a Marketing per sincronizzare l&#39;utente in Microsoft Dynamics CRM.

>[!NOTE]
>
>**Articoli correlati**
>
>[Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 3 di 3](step-3-of-3-connect.md)
