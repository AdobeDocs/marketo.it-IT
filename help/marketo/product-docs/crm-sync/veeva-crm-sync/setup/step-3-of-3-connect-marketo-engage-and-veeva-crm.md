---
description: Passaggio 3 di 3 - Connessione a Marketo Engage e [!DNL Veeva] CRM - Documentazione di Marketo - Documentazione del prodotto
title: Passaggio 3 di 3 - Connessione a Marketo Engage e  [!DNL Veeva] CRM
exl-id: aff91540-1d9d-448c-aae9-e6fa92a8ae01
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 1%

---

# Passaggio 3 di 3: connettere Marketo Engage e [!DNL Veeva] CRM {#step-3-of-3-connect-marketo-engage-and-veeva-crm}

In questo articolo configurerai Marketo Engage per la sincronizzazione con l&#39;istanza di CRM [!DNL Veeva] configurata. **Vedrai [!DNL Salesforce] in alcuni dei popup** poiché [!DNL Veeva] CRM è basato sulla piattaforma [!DNL Salesforce].

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: aggiunta di campi Marketo a [!DNL Veeva]](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}
>* [Passaggio 2 di 3: creazione di un  [!DNL Veeva] utente per Marketo](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-2-of-3-create-a-veeva-crm-user-for-marketo-engage.md){target="_blank"}

>[!IMPORTANT]
>
>È possibile connettere una sola istanza di Marketo a un&#39;istanza di CRM [!DNL Veeva] alla volta.

## Connetti a [!DNL Veeva] CRM tramite OAuth {#connect-to-veeva-crm-using-oauth}

1. In Marketo, Fare Clic Su **[!UICONTROL Admin]**. Selezionare **[!UICONTROL CRM]** e fare clic su **[!UICONTROL Sync with Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-1.png)

   >[!NOTE]
   >
   >Assicurarsi di [nascondere tutti i campi non necessari](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} in Marketo dall&#39;utente sincronizzato prima di fare clic su Sincronizza campi. Dopo aver fatto clic su Sincronizza campi, tutti i campi visualizzati dall&#39;utente verranno creati in Marketo in modo permanente e non potranno essere eliminati.

1. Fai clic su **[!UICONTROL Login with Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-2.png)

   >[!NOTE]
   >
   >Seleziona [!UICONTROL Sandbox] se stai sincronizzando una sandbox di Marketo in una sandbox di gestione delle relazioni con i clienti [!DNL Veeva].

1. Fai clic su **[!UICONTROL Confirm Credentials]**.

   ![](assets/step-3-of-3-connect-marketo-engage-3.png)

1. Verrà visualizzato un popup con la pagina di accesso [!DNL Salesforce]. Immettere le credenziali &quot;Utente Marketo Sync&quot; e fare clic su **[!UICONTROL Log In]**.

   ![](assets/step-3-of-3-connect-marketo-engage-4.png)

1. Immettere il codice di verifica ricevuto tramite e-mail (inviato da [!DNL Salesforce]) e fare clic su **[!UICONTROL Verify]**.

   ![](assets/step-3-of-3-connect-marketo-engage-5.png)

1. Una volta completata la verifica, viene visualizzata la pagina di accesso che richiede l’accesso. Fai clic su **[!UICONTROL Allow]**.

   ![](assets/step-3-of-3-connect-marketo-engage-6.png)

1. In pochi minuti verrà visualizzato un pop-up in Marketo Engae. Fai clic su **[!UICONTROL Confirm Credentials]**.

   ![](assets/step-3-of-3-connect-marketo-engage-7.png)

## Avvia sincronizzazione [!DNL Veeva] {#start-veeva-sync}

1. Fare clic su **[!UICONTROL Start Veeva Sync]** per avviare la sincronizzazione persistente di [!DNL Marketo-Veeva] CRM.

   ![](assets/step-3-of-3-connect-marketo-engage-8.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione su una sincronizzazione CRM [!DNL Veeva] o quando si immettono manualmente i lead.

1. Fai clic su **[!UICONTROL Start Sync]**.

   ![](assets/step-3-of-3-connect-marketo-engage-9.png)

>[!NOTE]
>
>Il tempo necessario per completare la sincronizzazione iniziale varia a seconda delle dimensioni e della complessità del database.

## Verifica sincronizzazione {#verify-sync}

Marketo fornisce messaggi di stato per la sincronizzazione CRM [!DNL Veeva] nell&#39;area di amministrazione. Per verificare che la sincronizzazione funzioni correttamente, segui la procedura riportata di seguito.

1. In Marketo, fai clic su **[!UICONTROL Admin]**, quindi su **[!UICONTROL Veeva]**.

   ![](assets/step-3-of-3-connect-marketo-engage-10.png)

1. Lo stato di sincronizzazione è visibile nell&#39;angolo superiore destro. Verrà visualizzato uno dei tre messaggi seguenti: Ultima sincronizzazione, Sincronizzazione in corso o Non riuscita.

>[!MORELIKETHIS]
>
>[Configura oggetti personalizzati](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}
