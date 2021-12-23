---
unique-page-id: 3571807
description: Passaggio 2 di 3 - Configurazione dell’utente di sincronizzazione Marketo in Dynamics (On-Premises 2011) - Documentazione Marketo - Documentazione del prodotto
title: Passaggio 2 di 3 - Configurazione dell’utente di sincronizzazione Marketo in Dynamics (On-Premises 2011)
exl-id: 807c8902-24a6-48b6-a5c9-96a72764fdef
source-git-commit: d4461e1bb73b7494970b4fde30fe551d9a5775d2
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Passaggio 2 di 3: Configurazione di Marketo Sync User in Dynamics (On-Premises 2011) {#step-of-set-up-marketo-sync-user-in-dynamics-on-premises}

Ottimo lavoro per completare i passaggi precedenti, continuiamo a farlo.

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: Installare la soluzione Marketo (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md)

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegna il ruolo utente di sincronizzazione Marketo solo all&#39;utente di sincronizzazione Marketo. Non è necessario assegnarlo ad altri utenti.

>[!NOTE]
>
>Questo vale per il plug-in Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare Marketo, vedi [Aggiornare la soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Impostazione della lingua dell&#39;utente di sincronizzazione [deve essere impostato su Inglese](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Nel menu in basso a sinistra, seleziona **Impostazioni**.

   ![](assets/image2015-4-2-14-3a2-3a40.png)

1. Nella struttura, seleziona **Amministrazione**.

   ![](assets/image2015-4-2-14-3a3-3a30.png)

1. Seleziona **Utenti**.

   ![](assets/image2015-4-2-14-3a4-3a37.png)

1. Verrà visualizzato un elenco di utenti qui. Seleziona l&#39;utente dedicato di sincronizzazione Marketo o contatta il tuo [Servizi federativi di Active Directory (AFDS)](https://msdn.microsoft.com/en-us/library/bb897402.aspx) per creare un nuovo utente dedicato a Marketo. Fai clic su **Gestisci ruoli**.

   ![](assets/image2015-4-2-14-3a11-3a7.png)

1. Controlla **Marketo Sync User** e fai clic su **OK**.

   ![](assets/image2015-4-2-14-3a15-3a0.png)

   >[!TIP]
   >
   >Se il ruolo non viene visualizzato, torna a [passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md) e importa la soluzione.

   >[!NOTE]
   >
   >Eventuali aggiornamenti effettuati nel CRM dall&#39;utente di sincronizzazione verranno **not** essere sincronizzati di nuovo in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi finito! Abbiamo solo qualche ultima configurazione prima di passare al prossimo articolo.

1. Seleziona **Impostazioni**. Quindi seleziona **Configurazione Marketo** nell&#39;albero.

   ![](assets/image2015-4-2-14-3a20-3a51.png)

   >[!NOTE]
   >
   >Se manca la configurazione Marketo, prova ad aggiornare la pagina. Se il problema persiste, [pubblicare nuovamente la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md) oppure disconnettiti e accedi di nuovo.

1. Fai clic su **Predefinito**.

   ![](assets/image2015-4-2-14-3a27-3a30.png)

1. Fai clic su ![](assets/image2015-4-2-14-3a29-3a1.png)

   ![](assets/image2015-4-2-14-3a28-3a40.png)

1. Nella finestra a comparsa, seleziona l’utente di sincronizzazione. Quindi fai clic su **OK**.

   ![](assets/image2015-4-2-14-3a32-3a43.png)

1. Fai clic su **Salva** per salvare le modifiche.

   ![](assets/image2015-4-2-14-3a34-3a15.png)

1. Fai clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/publish-all-customizations1.png)

## Prima di procedere al passaggio 3 {#before-proceeding-to-step}

    * Per limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ora.
    * Esegui il processo [Validate Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) . Verifica che le impostazioni iniziali siano state eseguite correttamente.
    * Accedi all’utente di sincronizzazione Marketo in Microsoft Dynamics CRM.

Ottimo lavoro!

>[!MORELIKETHIS]
>
>[Passaggio 3 di 3: Collegare Microsoft Dynamics con Marketo (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-3-of-3-connect.md)
