---
description: Passaggio 3 di 4 - Configurare l'app client in MS [!DNL Dynamics] - Documentazione Marketo - Documentazione del prodotto
title: Passaggio 3 di 4 - Configurare l'app client in MS [!DNL Dynamics]
exl-id: e7897174-3303-4c3b-8832-3e10f34fca96
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Passaggio 3 di 4: configurare l&#39;app client in MS [!DNL Dynamics] {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [Passaggio 1 di 4: installare la soluzione Marketo con la connessione di controllo password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [Passaggio 2 di 4: configurare la soluzione Marketo con la connessione di controllo password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. Passa a questo [articolo di Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Segui tutti i passaggi. Per il passaggio 3, immettere il nome di un&#39;applicazione pertinente, ad esempio &quot;[!DNL Marketo Integration]&quot;. In Tipi di account supportati, seleziona Account solo in questa directory organizzativa.

1. Annotare l&#39;ID applicazione (ClientId). Sarà necessario immetterlo in Marketo in un secondo momento.

1. Concedi il consenso all&#39;amministratore seguendo i passaggi descritti in [questo articolo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Generare un segreto client nell&#39;Admin Center facendo clic su **[!UICONTROL Certificates & secrets]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. Fai clic su **[!UICONTROL New client secret]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. Aggiungere una descrizione del segreto client e fare clic su **[!UICONTROL Add]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >Accertati di prendere nota del valore Segreto client (visualizzato nella schermata seguente), come sarà necessario in seguito. Viene visualizzato una sola volta e non sarà più possibile recuperarlo.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## [!DNL Azure AD] federato con [!DNL AD FS On-prem] {#azure-ad-federated-with-ad-fs-on-prem}

Per federare [!DNL Azure] AD a [!DNL ADFS Onprem] è necessario creare un criterio di individuazione del realm home per l&#39;applicazione specifica. Con questo criterio, [!DNL Azure] AD reindirizzerà la richiesta di autenticazione al servizio federativo. La sincronizzazione hash password deve essere abilitata in [!DNL AD Connect] per questo. Per ulteriori informazioni, vedere [[!DNL OAuth] with [!DNL ROPC]](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) e [Set an hrd policy for an application](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Ulteriori riferimenti [sono disponibili qui](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&text=This%20report%20also%20include%20federated,are%20federated%20to%20Azure%20AD.){target="_blank"}.

## Prima di procedere al punto 4 {#before-proceeding-to-step-4}

* Se si desidera limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
* Esegui il processo [Convalida [!DNL Microsoft Dynamics] Sincronizza](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedere all&#39;utente di Marketo Sync in [!DNL Microsoft Dynamics] CRM.

>[!MORELIKETHIS]
>
>* [Passaggio 4 di 4: connettere la soluzione Marketo con la connessione di controllo password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md){target="_blank"}
