---
unique-page-id: 3571827
description: Passaggio 2 di 3 - Configurare la soluzione Marketo con connessione server-server - Documentazione di Marketo - Documentazione del prodotto
title: 'Passaggio 2 di 3: configurare la soluzione Marketo con connessione server-server'
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Passaggio 2 di 3: configurare una soluzione Marketo con connessione server-server {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: installare la soluzione Marketo con connessione server-server](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}

## Crea applicazione client in Azure AD {#create-client-application-in-azure-ad}

1. Passa a [questo articolo di Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Segui tutti i passaggi. Per il passaggio 3, immettere il nome di un&#39;applicazione pertinente, ad esempio &quot;Integrazione Marketo&quot;. In Tipi di account supportati, selezionare **Account solo in questa directory organizzativa**.

1. Annotare l&#39;ID applicazione (ClientId) e l&#39;ID tenant. Sarà necessario immetterlo in Marketo in un secondo momento.

1. Concedi il consenso all&#39;amministratore seguendo i passaggi [descritti in questo articolo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Generare un segreto client nell&#39;Admin Center facendo clic su **[!UICONTROL Certificati e segreti]**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. Fare clic sul pulsante **[!UICONTROL Nuovo segreto client]**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. Immettere una descrizione del segreto client e fare clic su **[!UICONTROL Aggiungi]**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>Accertati di prendere nota del valore Segreto client (visualizzato nella schermata seguente), come sarà necessario in seguito. Viene visualizzato una sola volta e non sarà più possibile recuperarlo.

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## Creazione di un utente dell’applicazione in Microsoft {#create-application-user-in-microsoft}

1. Segui i passaggi del seguente collegamento per [configurare un utente dell&#39;applicazione in Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation){target="_blank"}.

   >[!IMPORTANT]
   >
   >* Quando si assegnano le autorizzazioni all&#39;utente dell&#39;applicazione, assicurarsi di assegnarle al &quot;Ruolo utente di Marketo Sync&quot;.
   >* Prendere nota dell&#39;indirizzo di posta elettronica dell&#39;utente dell&#39;applicazione dall&#39;opzione [visualizza dettagli](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user){target="_blank"} in Power Platform. Questo indirizzo e-mail verrà utilizzato come nome utente durante la configurazione della connessione a MS Dynamics in Marketo.
   >* Eventuali aggiornamenti apportati nel CRM dall&#39;utente di sincronizzazione **non** verranno sincronizzati di nuovo in Marketo.

## Azure AD federato con ADFS on-premise {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD ad ADFS Onprem richiede la creazione di un criterio di individuazione del realm home per l&#39;applicazione specifica. Con questo criterio, Azure AD reindirizzerà la richiesta di autenticazione al servizio federativo. La sincronizzazione hash della password deve essere abilitata in AD Connect per questo. Per ulteriori informazioni, vedere [OAuth con ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc){target="_blank"} e [Impostare un criterio rigido per un&#39;applicazione](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application){target="_blank"}.

Ulteriori riferimenti [sono disponibili qui](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20include%20federated,are%20federated%20to%20Azure%20AD.){target="_blank"}.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Ci siamo quasi! Tutto ciò che ci rimane è informare Marketo Solution sul nuovo utente creato.

1. Torna alla sezione Impostazioni avanzate e fai clic sull&#39;icona ![](assets/image2015-5-13-15-3a49-3a19.png) accanto a Impostazioni, quindi seleziona **[!UICONTROL Configurazione Marketo]**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Se nel menu Settings (Impostazioni) non viene visualizzato &quot;Marketo Config&quot; (Configurazione), aggiorna la pagina. Se non funziona, prova a [pubblicare di nuovo la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"} oppure esci e accedi di nuovo.

1. Fare clic su **[!UICONTROL Predefinito]**.

   ![](assets/fifteen.png)

1. Fai clic sul pulsante Cerca nel campo **[!UICONTROL Utente Marketo]** e seleziona l&#39;utente di sincronizzazione creato.

   ![](assets/sixteen.png)

1. Fai clic sull&#39;icona ![](assets/image2015-3-13-15-3a10-3a11.png) nell&#39;angolo in basso a destra per salvare le modifiche.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Fai clic su **X** in alto a destra per chiudere la schermata.

   ![](assets/seventeen.png)

1. Fai clic sull&#39;icona ![](assets/image2015-5-13-15-3a49-3a19-1.png) accanto a Impostazioni e seleziona **[!UICONTROL Soluzioni]**.

   ![](assets/eighteen.png)

1. Fai clic sul pulsante **[!UICONTROL Tutte le personalizzazioni di Publish]**.

   ![](assets/nineteen.png)

   >[!NOTE]
   >
   >Se aggiorni l&#39;autenticazione di base a OAuth, puoi utilizzare [questo articolo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"} per riconfigurare l&#39;autenticazione.

## Prima di procedere al punto 3 {#before-proceeding-to-step}

* Se si desidera limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"}.
* Eseguire il processo [Convalida Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}. Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedere a Marketo Sync User in Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>* [Passaggio 3 di 3: connettere la soluzione Marketo con la connessione server-server](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md){target="_blank"}
>* [Riconfigura il metodo di autenticazione Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"}
