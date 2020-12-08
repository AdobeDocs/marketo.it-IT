---
unique-page-id: 3571816
description: Passaggio 2 di 3 - Configura sincronizzazione utente per Marketo (2013 On-Premises) - Marketo Docs - Documentazione prodotto
title: Passaggio 2 di 3 - Configura sincronizzazione utente per Marketo (2013 On-Premises)
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---


# Passaggio 2 di 3: Configurare l&#39;utente di sincronizzazione per Marketo (On-Premises 2013) {#step-of-configure-sync-user-for-marketo-on-premises}

Ottimo lavoro per completare i passaggi precedenti, continuiamo a farlo.

>[!NOTE]
>
>**Prerequisiti**
>
>* [Passaggio 1 di 3: Installare la soluzione Marketo in Dynamics (On-Premises 2013)](step-1-of-3-install.md)


## Assegna ruolo utente sincronizzazione {#assign-sync-user-role}

Assegnate il ruolo di sincronizzazione utente Marketo solo all’utente di sincronizzazione Marketo. Non è necessario assegnarlo ad altri utenti.

>[!NOTE]
>
>Questo vale per il plug-in Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo di utente di sincronizzazione. Per aggiornare Marketo, consulta [Aggiornamento della soluzione Marketo per Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. In **Impostazioni**, fate clic su **Amministrazione**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Selezionate **Utenti**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Verrà visualizzato un elenco di utenti qui. Selezionate l&#39;utente dedicato di Marketing per la sincronizzazione o contattate il vostro [amministratore di](https://msdn.microsoft.com/en-us/library/bb897402.aspx) Active Directory Federation Services (AFDS) [per creare un nuovo utente dedicato a Marketo.](http://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Selezionate l’utente di sincronizzazione. Fate clic ![](assets/image2015-3-26-11-3a16-3a22.png)e selezionate **Gestisci ruoli**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Selezionate **Marketo per sincronizzare l’utente** e fate clic su **OK**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Se il ruolo non viene visualizzato, tornate al [punto 1 di 3](step-1-of-3-install.md) e importate la soluzione.

   >[!NOTE]
   >
   >Eventuali aggiornamenti apportati in CRM dall&#39;utente di sincronizzazione **non** verranno sincronizzati di nuovo su Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi fatto! Abbiamo solo qualche ultima configurazione prima di passare all&#39;articolo successivo.

1. In **Impostazioni**, fai clic su Configurazione **Marketo**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Se **manca la configurazione** Marketo, prova ad aggiornare la pagina. Se il problema persiste, [pubblicate nuovamente la soluzione](https://docs.marketo.com/pages/viewpage.action?pageId=3571813#Step1of3:InstalltheMarketoSolutioninDynamics(2013On-Premises)-PublishAllCustomizations) Marketo o provate a disconnettersi e rientrare.

1. Fate clic su **Predefinito**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Fate clic sul campo **Marketo utente** e selezionate l’utente di sincronizzazione.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Fate clic ![](assets/image2015-3-13-15-3a10-3a11.png) nell’angolo in basso a destra per salvare le modifiche.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Fate clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere allo stadio 3 {#before-proceeding-to-step}

* Se desiderate limitare il numero di record da sincronizzare, [impostate ora un filtro](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) di sincronizzazione personalizzato.
* Eseguire il processo [Validate Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) . Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedi a Marketing per sincronizzare l&#39;utente in Microsoft Dynamics CRM.

Ottimo lavoro!

>[!NOTE]
>
>**Articoli correlati**
>
>* [Passaggio 3 di 3: Connect Marketo e Dynamics (On-Premises 2013)](step-3-of-3-connect.md)

