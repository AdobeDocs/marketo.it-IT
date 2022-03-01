---
unique-page-id: 3571827
description: 'Passaggio 2 di 3: configurare la soluzione Marketo con la connessione server-to-server - Marketo Docs - Documentazione del prodotto'
title: 'Passaggio 2 di 3: configurare la soluzione Marketo con la connessione server-to-server'
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
source-git-commit: 48b8289994e000eafd72982ac1b4a0a809b10bab
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Passaggio 2 di 3: Configurare la soluzione Marketo con la connessione server-to-server {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: Installare la soluzione Marketo con la connessione server a server](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)

## Crea applicazione client in Azure AD {#create-client-application-in-azure-ad}

1. Passa a [questo articolo Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration).

1. Segui tutti i passaggi. Per il passaggio 3, immettere un nome applicazione pertinente (ad esempio, &quot;Integrazione Marketo&quot;). In Tipi di account supportati, seleziona **Account solo in questa directory organizzativa**.

1. Annotare l’ID applicazione (ClientId) e l’ID tenant. Sarà necessario inserirlo in Marketo in un secondo momento.

1. Concedi il consenso dell’amministratore seguendo i passaggi [nel presente articolo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. Genera un segreto client in Admin Center facendo clic su **Certificati e segreti**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. Fai clic sul pulsante **Nuovo segreto client** pulsante .

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. Immetti una descrizione del segreto client e fai clic su **Aggiungi**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>Accertati di prendere nota del valore Segreto client (mostrato nella schermata seguente), in quanto ne avrai bisogno in un secondo momento. Viene mostrato solo una volta e non potrai recuperarlo di nuovo.

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## Creare un utente dell’applicazione in Microsoft {#create-application-user-in-microsoft}

1. Segui i passaggi dal seguente collegamento a [configurare un utente dell&#39;applicazione in Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation).

   >[!IMPORTANT]
   >
   >* Quando si assegnano le autorizzazioni all&#39;utente dell&#39;applicazione, assicurarsi di assegnarlo a &quot;Ruolo utente di sincronizzazione Marketo&quot;.
   >* Osserva l’indirizzo e-mail dell’utente dell’applicazione dal [opzione visualizza dettagli](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) su Power Platform. Questo indirizzo e-mail verrà utilizzato come nome utente quando si imposta la connessione a MS Dynamics in Marketo.


## Azure AD Federated con AD FS On-Prem {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD to ADFS Onprem richiede la creazione di un criterio di individuazione dell&#39;area iniziale per l&#39;applicazione specifica. Con questo criterio, Azure AD reindirizzerà la richiesta di autenticazione al servizio federativo. A questo scopo, la sincronizzazione hash della password deve essere abilitata in AD Connect. Per ulteriori informazioni, consulta [OAuth con ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) e [Impostare un criterio hrd per un&#39;applicazione](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Riferimenti aggiuntivi [si trova qui](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20include%20federated, are%20federated%20to%20Azure%20AD.).

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi lì! Tutto quello che ci rimane è quello di informare Marketo Solution sul nuovo utente creato.

>[!IMPORTANT]
>
>Se stai effettuando l’aggiornamento dall’autenticazione di base a OAuth, dovrai contattare [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support) per informazioni sull’aggiornamento dei parametri aggiuntivi. L&#39;esecuzione di una modifica della configurazione all&#39;utente di sincronizzazione predefinita interrompe temporaneamente la sincronizzazione finché non vengono inserite nuove credenziali e la sincronizzazione non viene riabilitata. Su richiesta, il supporto Marketo può disattivare la funzione (fino ad aprile 2022) se desideri ripristinare il vecchio metodo di autenticazione.

1. Torna alla sezione Impostazioni avanzate e fai clic su ![](assets/image2015-5-13-15-3a49-3a19.png) accanto a Impostazioni e seleziona **Configurazione Marketo**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Se non vedi **Configurazione Marketo** nel menu Impostazioni , aggiorna la pagina. Se non funziona, prova a [pubblicare la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md) di nuovo o disconnettiti e accedi di nuovo.

1. Fai clic su **Predefinito**.

   ![](assets/fifteen.png)

1. Fai clic sul pulsante di ricerca nel **Utente Marketo** e seleziona l’utente di sincronizzazione creato.

   ![](assets/sixteen.png)

1. Fai clic sul pulsante ![](assets/image2015-3-13-15-3a10-3a11.png) nell’angolo in basso a destra per salvare le modifiche.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Fai clic sul pulsante **X** in alto a destra per chiudere lo schermo.

   ![](assets/seventeen.png)

1. Fai clic sul pulsante ![](assets/image2015-5-13-15-3a49-3a19-1.png) accanto a Impostazioni e seleziona **Soluzioni**.

   ![](assets/eighteen.png)

1. Fai clic sul pulsante **Pubblica tutte le personalizzazioni** pulsante .

   ![](assets/nineteen.png)

## Prima di procedere al passaggio 3 {#before-proceeding-to-step}

* Se si desidera limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ora.
* Esegui il [Convalida della sincronizzazione di Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) processo. Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedi all’utente di sincronizzazione Marketo in Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>* [Passaggio 3 di 3: Connessione della soluzione Marketo con la connessione server a server](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md)
>* [Riconfigura metodo di autenticazione Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)

