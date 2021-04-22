---
description: Impostare MSD per Azure AD Federated con Active Directory FS on-prem, tenant e Microsoft Online - Marketo Docs - Documentazione del prodotto
title: Impostare MSD per Azure AD Federated con Active Directory FS On-Prem, Tenant e Microsoft Online
exl-id: b6c10048-d27e-4135-beef-232deddc2984
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Impostare MSD per Azure AD Federated con AD FS On-Prem, Tenant e Microsoft Online {#set-up-msd-for-azure-ad-federated-with-ad-fs-on-prem-tenant-and-microsoft-online}

## Configurare l’app Microsoft Dynamics CRM {#set-up-microsoft-dynamics-crm-app}

1. Vai su https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration.

1. Segui tutti i passaggi. Per il passaggio 3, immettere un nome applicazione pertinente (ad esempio, &quot;Integrazione Marketo&quot;). In Tipi di account supportati, seleziona Account solo in questa directory organizzativa.

1. Annotare l&#39;ID applicazione (ClientId). Sarà necessario inserirlo in Marketo in un secondo momento.

1. Concedi il consenso dell&#39;amministratore seguendo i passaggi descritti in [questo articolo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/grant-consent-for-client-id-and-app-registration.md).

1. Genera un segreto client in Admin Center facendo clic su **Certificati e segreti**.

   ![](assets/set-up-msd-for-azure-ad-federated-1.png)

1. Fare clic su **Nuovo segreto client**.

   ![](assets/set-up-msd-for-azure-ad-federated-2.png)

1. Aggiungi una descrizione del segreto client e fai clic su **Aggiungi**.

   ![](assets/set-up-msd-for-azure-ad-federated-3.png)

   >[!CAUTION]
   >
   >Accertati di prendere nota del valore Segreto client (mostrato nella schermata seguente), in quanto ne avrai bisogno in un secondo momento. Viene mostrato solo una volta e non potrai recuperarlo di nuovo.

   ![](assets/set-up-msd-for-azure-ad-federated-4.png)

Marketo si autentica in Azure AD con OAuth utilizzando le credenziali per la password del proprietario della risorsa di tipo Grant_type ( ROPC). Questo scenario richiede la creazione di un criterio Home Realm Discovery per l&#39;applicazione specifica. Con questo criterio, Azure AD reindirizzerà la richiesta di autenticazione al servizio federativo. A questo scopo, la sincronizzazione hash della password deve essere abilitata in AD Connect. Per ulteriori informazioni, consulta [OAuth with ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) e [Imposta un criterio hrd per un&#39;applicazione](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Ulteriori riferimenti [sono disponibili qui](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20include%20federated, are%20federated%20to%20Azure%20AD.).

Al termine, è il momento di **immettere in Marketo** l’ID client generato e il segreto di Dynamics CRM in.

## Immetti l’ID client e il segreto generati da Dynamics CRM in Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/set-up-msd-for-azure-ad-federated-5.png)

1. Fare clic su **Microsoft Dynamics**.

   ![](assets/set-up-msd-for-azure-ad-federated-6.png)

1. Fare clic su **Disattiva sincronizzazione**.

   ![](assets/set-up-msd-for-azure-ad-federated-7.png)

1. Accanto alle credenziali, fare clic su **Modifica**.

   ![](assets/set-up-msd-for-azure-ad-federated-8.png)

1. Immetti i **ID client** e **Segreto client** recuperati in precedenza e premi **Salva**.

   ![](assets/set-up-msd-for-azure-ad-federated-9.png)

1. Fare clic su **Convalida configurazione sincronizzazione**.

   ![](assets/set-up-msd-for-azure-ad-federated-10.png)

1. Fare clic su **Avanti**.

   ![](assets/set-up-msd-for-azure-ad-federated-11.png)

1. Dovresti visualizzare tutti i segni di spunta verdi. Fare clic su **Chiudi**.

   ![](assets/set-up-msd-for-azure-ad-federated-12.png)

   >[!NOTE]
   >
   >Se trovi una X rossa tra i segni di spunta verdi, consulta [questo articolo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) per le opzioni di correzione.

1. Fare clic su **Abilita sincronizzazione**.

   ![](assets/set-up-msd-for-azure-ad-federated-13.png)

Ed è tutto!
