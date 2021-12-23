---
unique-page-id: 3571816
description: Passaggio 2 di 3 - Configurare la sincronizzazione degli utenti per Marketo (On-Premises 2013) - Marketo Docs - Documentazione del prodotto
title: 'Passaggio 2 di 3: configurare l’utente per la sincronizzazione per Marketo (On-Premises 2013)'
exl-id: 27c4407e-0623-4ae0-8aa1-0b28c6c5c4f8
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Passaggio 2 di 3: Configura l’utente di sincronizzazione per Marketo (On-Premises 2013) {#step-of-configure-sync-user-for-marketo-on-premises}

Ottimo lavoro per completare i passaggi precedenti, continuiamo a farlo.

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: Installare la soluzione Marketo in Dynamics (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegna il ruolo utente di sincronizzazione Marketo solo all&#39;utente di sincronizzazione Marketo. Non è necessario assegnarlo ad altri utenti.

>[!NOTE]
>
>Questo vale per il plug-in Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare Marketo, vedi [Aggiornare la soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Impostazione della lingua dell&#39;utente di sincronizzazione [deve essere impostato su Inglese](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Sotto **Impostazioni**, fai clic su **Amministrazione**.

   ![](assets/image2014-12-11-11-3a13-3a19.png)

1. Seleziona **Utenti**.

   ![](assets/image2014-12-11-11-3a13-3a29.png)

1. Verrà visualizzato un elenco di utenti qui. Seleziona l&#39;utente dedicato di Marketo Sync o contatta il tuo [Servizi federativi di Active Directory (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) [per creare un nuovo utente dedicato a Marketo.](https://blogs.technet.com/b/askpfeplat/archive/2014/04/21/introduction-to-active-directory-federation-services-ad-fs-alternateloginid-feature.aspx)

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Seleziona l’utente di sincronizzazione. Fai clic su ![](assets/image2015-3-26-11-3a16-3a22.png) e seleziona **Gestisci ruoli**

   ![](assets/image2015-3-26-11-3a18-3a6.png)

1. Controlla **Marketo Sync User** e fai clic su **OK**.

   ![](assets/image2014-12-11-11-3a14-3a52.png)

   >[!TIP]
   >
   >Se il ruolo non viene visualizzato, torna a [passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) e importa la soluzione.

   >[!NOTE]
   >
   >Eventuali aggiornamenti effettuati nel CRM dall&#39;utente di sincronizzazione verranno **not** essere sincronizzati di nuovo in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi finito! Abbiamo solo qualche ultima configurazione prima di passare al prossimo articolo.

1. Sotto **Impostazioni**, fai clic su **Configurazione Marketo**.

   ![](assets/image2014-12-11-11-3a15-3a1.png)

   >[!NOTE]
   >
   >Se **Configurazione Marketo** mancante, prova ad aggiornare la pagina. Se il problema persiste, [pubblicare la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md) di nuovo o prova a disconnettersi e di nuovo ad entrare.

1. Fai clic su **Predefinito**.

   ![](assets/image2015-3-26-11-3a30-3a20.png)

1. Fai clic sul pulsante **Utente Marketo** e seleziona l&#39;utente di sincronizzazione.

   ![](assets/image2015-3-26-11-3a29-3a13.png)

1. Fai clic su ![](assets/image2015-3-13-15-3a10-3a11.png) nell’angolo in basso a destra per salvare le modifiche.

   ![](assets/image2014-12-11-11-3a15-3a32.png)

1. Fai clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere al passaggio 3 {#before-proceeding-to-step}

* Se si desidera limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ora.
* Esegui il [Convalida della sincronizzazione di Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) processo. Verifica che le impostazioni iniziali siano state eseguite correttamente.
* Accedi all’utente di sincronizzazione Marketo in Microsoft Dynamics CRM.

Ottimo lavoro!

>[!MORELIKETHIS]
>
>[Passaggio 3 di 3: Collegare Marketo e Dynamics (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-3-of-3-connect.md)
