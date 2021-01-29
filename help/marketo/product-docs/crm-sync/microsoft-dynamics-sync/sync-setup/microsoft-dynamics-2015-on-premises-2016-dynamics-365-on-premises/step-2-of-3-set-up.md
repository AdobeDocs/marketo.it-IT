---
unique-page-id: 7504739
description: Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 2 di 3 - Marketo Docs - Documentazione prodotto
title: Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 2 di 3
translation-type: tm+mt
source-git-commit: 309f299275bfe75e8af0150be0a5ffdf28a54cf8
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# Passaggio 2 di 3

<!--Install Marketo for Dynamics 2015 On-Prem and 2016 365 On-Prem Step 2 of 3-->

Ottimo lavoro per completare i passaggi precedenti. Continuiamo a farlo.

>[!PREREQUISITES]
>
>* [Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 1 di 3](step-1-of-3-install.md)

>



## Assegna ruolo utente sincronizzazione {#assign-sync-user-role}

Assegnate il ruolo di sincronizzazione utente Marketo solo all’utente di sincronizzazione Marketo. Non è necessario assegnarlo ad altri utenti.

>[!NOTE]
>
>Questo vale per Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo di utente di sincronizzazione. Per aggiornare Marketo, vedere [Aggiornamento della soluzione Marketo per Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. In **Impostazioni**, fare clic su **Protezione**.

   ![](assets/assign1.png)

1. Fare clic su **Utenti**.

   ![](assets/assign2.png)

1. Verrà visualizzato un elenco di utenti qui. Seleziona l&#39;utente dedicato di Marketing per la sincronizzazione oppure contatta l&#39;amministratore [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) per creare un utente dedicato per Marketo.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selezionate l’utente di sincronizzazione. Fare clic su **Gestisci ruoli**.

   ![](assets/assign4.png)

   Selezionate Marketo Sync User (Sincronizza utente) e fate clic su OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Se il ruolo non è visualizzato, tornare al [passaggio 1 di 3](step-1-of-3-install.md) e importare la soluzione.

   >[!NOTE]
   >
   >Eventuali aggiornamenti effettuati in CRM dall&#39;utente di sincronizzazione **non** verranno sincronizzati nuovamente in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi fatto! Abbiamo solo qualche ultima configurazione prima di passare all&#39;articolo successivo.

1. In **Impostazioni**, fare clic su **Configurazione marketing**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Se manca la configurazione Marketo, provare ad aggiornare la pagina. Se il problema persiste, [pubblicare la soluzione Marketo](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) oppure provare a disconnettersi e rientrare.

1. Fare clic su **Default**.

   ![](assets/configure2.png)

1. Fate clic sul campo **Marketing User** e selezionate l&#39;utente di sincronizzazione.

   ![](assets/configure3.png)

1. Fate clic sull&#39;icona Salva nell&#39;angolo in basso a destra.

   ![](assets/configure4.png)

1. Fate clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere al passaggio 3 {#before-proceeding-to-step}

* Se si desidera limitare il numero di record sincronizzati, [impostare ora un filtro di sincronizzazione personalizzato](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
* Eseguire il processo [Validate Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedi a Marketing per sincronizzare l&#39;utente in Microsoft Dynamics CRM.

>[!NOTE]
>
>**Articoli correlati**
>
>[Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 3 di 3](step-3-of-3-connect.md)
