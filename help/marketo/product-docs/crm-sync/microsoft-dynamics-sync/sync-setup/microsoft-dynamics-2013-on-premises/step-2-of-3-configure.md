---
unique-page-id: 3571816
description: Passaggio 2 di 3 - Configurare l’utente di sincronizzazione per Marketo (On-Premises 2013) - Documenti Marketo - Documentazione del prodotto
title: Passaggio 2 di 3 - Configurare l’utente di sincronizzazione per Marketo (On-Premises 2013)
translation-type: tm+mt
source-git-commit: 9d8a6d9880de5d2af211906c2410f2057c1f454d
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# Passaggio 2 di 3: Configura l&#39;utente di sincronizzazione per Marketo (2013 On-Premises) {#step-of-configure-sync-user-for-marketo-on-premises}

Ottimo lavoro per completare i passaggi precedenti, continuiamo a farlo.

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: Installare la soluzione Marketo in Dynamics (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegna il ruolo Utente sincronizzazione Marketo solo all’utente di sincronizzazione Marketo. Non è necessario assegnarlo ad altri utenti.

>[!NOTE]
>
>Questo vale per il plug-in Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare Marketo, consulta [Aggiornare la soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. In **Impostazioni**, fai clic su **Amministrazione**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Seleziona **Utenti**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Verrà visualizzato un elenco di utenti qui. Seleziona l&#39;utente dedicato di Marketo Sync o contatta l&#39;amministratore di [Active Directory Federation Services (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [per creare un nuovo utente dedicato a Marketo.](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Seleziona l’utente di sincronizzazione. Fai clic su ![](assets/image2015-3-26-11-3a16-3a22.png) e seleziona **Gestisci ruoli**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Controllare **Marketo Sync User** e fare clic su **OK**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Se il ruolo non viene visualizzato, tornare al [passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) e importare la soluzione.

   >[!NOTE]
   >
   >Eventuali aggiornamenti effettuati nel CRM dall&#39;utente di sincronizzazione **non** verranno sincronizzati nuovamente in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi finito! Abbiamo solo qualche ultima configurazione prima di passare al prossimo articolo.

1. In **Impostazioni**, fai clic su **Configurazione Marketo**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Se manca **Configurazione Marketo**, prova ad aggiornare la pagina. Se il problema persiste, [pubblica nuovamente la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) oppure prova a disconnetterti e ad effettuare di nuovo l&#39;accesso.

1. Fare clic su **Predefinito**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Fai clic sul campo **Marketo User** e seleziona l&#39;utente di sincronizzazione.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Fai clic su ![](assets/image2015-3-13-15-3a10-3a11.png) nell’angolo in basso a destra per salvare le modifiche.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Fai clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere al passaggio 3 {#before-proceeding-to-step}

* Per limitare il numero di record sincronizzati, [imposta ora un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
* Esegui il processo [Convalida Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) . Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedi all’utente di sincronizzazione Marketo in Microsoft Dynamics CRM.

Ottimo lavoro!

>[!MORELIKETHIS]
>
>[Passaggio 3 di 3: Connetti Marketo e Dynamics (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
