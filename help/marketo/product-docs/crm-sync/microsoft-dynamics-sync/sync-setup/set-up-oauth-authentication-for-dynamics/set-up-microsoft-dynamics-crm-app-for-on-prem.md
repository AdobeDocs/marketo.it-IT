---
description: Configurare l’app Microsoft Dynamics CRM per On-Prem - Documenti Marketo - Documentazione del prodotto
title: Configurare l’app Microsoft Dynamics CRM per On-Prem
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---


# Configurare l’app Microsoft Dynamics CRM per On-Prem {#set-up-microsoft-dynamics-crm-app-for-on-prem}

È possibile eseguire la configurazione basata su ID client/segreto client in Marketo per On-Prem con AD FS (ver. 2016 o successivo). Per le versioni precedenti di On-Prem, contatta il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) per far sì che il metodo di autenticazione venga modificato in base solo all&#39;ID utente e alla password.

## Configurare l’app Microsoft Dynamics CRM {#set-up-microsoft-dynamics-crm-app}

Segui i passaggi descritti in [questo articolo di Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later).

Al termine, il passaggio successivo è **Immettere l&#39;ID client e il segreto generati da Dynamics CRM in Marketo**.

## Immetti l’ID client e il segreto generati da Dynamics CRM in Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

I passaggi seguenti sono applicabili alle versioni online e on-prem.

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-1.png)

1. Fare clic su **Microsoft Dynamics**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-2.png)

1. Fare clic su **Disattiva sincronizzazione**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-3.png)

1. Accanto alle credenziali, fare clic su **Modifica**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-4.png)

1. Immetti i **ID client** e **Segreto client** recuperati in precedenza e premi **Salva**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-5.png)

1. Fare clic su **Convalida configurazione sincronizzazione**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-6.png)

1. Fare clic su **Avanti**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-7.png)

1. Dovresti visualizzare tutti i segni di spunta verdi. Fare clic su **Chiudi**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-8.png)

   >[!NOTE]
   >
   >Se trovi una X rossa tra i segni di spunta verdi, consulta [questo articolo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) per le opzioni di correzione.

1. Fare clic su **Abilita sincronizzazione**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-9.png)

Ed è tutto!
