---
description: Passaggio 3 di 3 - Collegare il Marketo Engage e Veeva CRM - Documentazione di Marketo - Documentazione del prodotto
title: Passaggio 3 di 3 - Collegare Marketo Engage e Veeva CRM
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Passaggio 3 di 3: Collegare il Marketo Engage e Veeva CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

In questo articolo configurerai il Marketo Engage per la sincronizzazione con l’istanza di CRM Veeva configurata. **Vedrai Salesforce in alcuni dei pop-up** come Veeva CRM è costruito sulla piattaforma Salesforce.

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: aggiungere campi Marketo a Veeva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [Passaggio 2 di 3: creare un utente Veeva per Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>È possibile connettere una sola istanza di Marketo a un&#39;istanza di CRM Veeva alla volta.

## Connettersi a Veeva CRM tramite OAuth {#connect-to-veeva-crm-using-oauth}

1. In Marketo, Fai Clic Su **[!UICONTROL Amministratore]**. Seleziona **[!UICONTROL CRM]** e fai clic su **[!UICONTROL Sincronizza con Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >Assicurati di [nascondi tutti i campi non necessari](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} in Marketo dall&#39;utente di sincronizzazione prima di fare clic su Sincronizza campi. Dopo aver fatto clic su Sincronizza campi, tutti i campi visualizzati dall&#39;utente verranno creati in Marketo in modo permanente e non potranno essere eliminati.

1. Clic **[!UICONTROL Accedi con Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Seleziona Sandbox se stai sincronizzando una Sandbox Marketo in una Sandbox Veeva CRM.

1. Clic **[!UICONTROL Conferma credenziali]**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Viene visualizzata una finestra a comparsa con la pagina di accesso di Salesforce. Immetti le credenziali &quot;Marketo Sync User&quot; (Utente di sincronizzazione) e fai clic su **[!UICONTROL Accedi]**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Immetti il codice di verifica ricevuto tramite e-mail (inviato da Salesforce) e fai clic su **[!UICONTROL Verifica]**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. Una volta completata la verifica, viene visualizzata la pagina di accesso che richiede l’accesso. Clic **[!UICONTROL Consenti]**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. In pochi minuti verrà visualizzato un pop-up in Marketo Engae. Clic **[!UICONTROL Conferma credenziali]**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Avvia Veeva Sync {#start-veeva-sync}

1. Clic **[!UICONTROL Avvia Veeva Sync]** per avviare la sincronizzazione persistente di Marketo-Veeva CRM.

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione rispetto a una sincronizzazione CRM Veeva o quando si immettono manualmente i lead.

1. Clic **[!UICONTROL Avvia sincronizzazione]**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>Il tempo necessario per completare la sincronizzazione iniziale varia a seconda delle dimensioni e della complessità del database.

## Verifica sincronizzazione {#verify-sync}

Marketo fornisce messaggi di stato per la sincronizzazione di Veeva CRM nell’area di amministrazione. Per verificare che la sincronizzazione funzioni correttamente, segui la procedura riportata di seguito.

1. In Marketo, fai clic su **[!UICONTROL Amministratore]**, quindi **[!UICONTROL Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. Lo stato di sincronizzazione è visibile nell&#39;angolo superiore destro. Verrà visualizzato uno dei tre messaggi seguenti: Ultima sincronizzazione, Sincronizzazione in corso o Non riuscita.

>[!MORELIKETHIS]
>
>[Configura oggetti personalizzati](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
