---
unique-page-id: 9437903
description: Creazione di un filtro di sincronizzazione personalizzato [!DNL Dynamics] - Documentazione di Marketo - Documentazione del prodotto
title: Crea un filtro di sincronizzazione  [!DNL Dynamics] personalizzato
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 1%

---

# Crea un filtro di sincronizzazione [!DNL Dynamics] personalizzato {#create-a-custom-dynamics-sync-filter}

Marketo consente di impostare un filtro di sincronizzazione e di sincronizzare solo una parte dei record.

## Panoramica {#overview}

Per impostare un filtro di sincronizzazione [!DNL Dynamics]:

1. Crea un campo personalizzato con due opzioni (booleano) denominato `new_synctomkto` in Dynamics CRM per qualsiasi oggetto (lead, contatto, account, opportunità e altre entità personalizzate).
1. Assegnare un valore Sì/No a questo campo.

È necessario apportare queste modifiche in Dynamics CRM, non nel database o in Marketo.

>[!CAUTION]
>
>Se non assegni il campo e lo lasci vuoto/NULL, verrà sincronizzato ma non aggiornato. I record con un valore di campo vuoto/NULL in Dynamics CRM visualizzeranno questo valore di campo in Marketo come &quot;false&quot;.

Marketo cerca questo campo durante la sincronizzazione in background automatica e determina quali record sincronizzare in base a questa logica:

| Valore campo | Sincronizzare con Marketo? |
|---|---|
| Il campo non esiste | Sì |
| Il campo è vuoto | Sì |
| Il campo ha valore Sì | Sì |
| Campo con valore No | No |

>[!CAUTION]
>
>L&#39;unico modo per indicare a Marketo di ignorare un record consiste nell&#39;impostare esplicitamente il valore del campo su **No**. Marketo sincronizza comunque i record anche se i valori dei campi sono vuoti.

>[!PREREQUISITES]
>
>Installare la versione più recente del plug-in di Marketo (3.0.0.1 o versione successiva). Vai a Marketo > [!UICONTROL Admin] > [!DNL Microsoft Dynamics] > [!UICONTROL Download Marketo Solution].

## Crea campo SyncToMkto {#create-synctomkto-field}

1. Accedi a Dynamics CRM. Fai clic su **Impostazioni**, quindi su **Personalizzazioni**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Fai clic su **[!UICONTROL Customize the System]**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Fai clic su ![](assets/image2015-8-10-21-3a44-3a23.png) accanto a **[!UICONTROL Entities]**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Fai clic su ![](assets/image2015-8-10-21-3a44-3a23.png) accanto a **[!UICONTROL Lead]** e seleziona **[!UICONTROL Fields]**. Quindi fai clic su **[!UICONTROL New]**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Immettere **SyncToMkto** nel campo **[!UICONTROL Display Name]** e selezionare **[!UICONTROL Two Options]** come **[!UICONTROL Data Type]**. Quindi fai clic su **[!UICONTROL Save and Close]**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Scegliere un nome visualizzato per questo campo, ma il campo Nome deve essere esattamente **new_synctomkto**. Utilizza **new** come prefisso predefinito. Se hai modificato il valore predefinito, vai qui per [reimpostare il prefisso predefinito per i nomi dei campi personalizzati](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md){target="_blank"}. Puoi ripristinarla dopo aver creato i nuovi campi.

   >[!NOTE]
   >
   >Se è stato configurato un flusso di lavoro asincrono, il record ottiene il valore SyncToMkto predefinito impostato nel campo e ottiene il valore corretto alcuni secondi dopo al termine dell&#39;esecuzione del flusso di lavoro. Se il valore predefinito è impostato su Sì, tali record verranno creati in Marketo e quindi diventeranno obsoleti. Utilizza **No** come valore predefinito per evitare questo problema.

1. Ripeti questo processo e crea il campo **SyncToMkto** per tutte le altre entità su cui desideri limitare la sincronizzazione, ad esempio contatto, account, opportunità ed entità personalizzate.

## Selezionare il filtro in Marketo {#select-the-filter-in-marketo}

Anche se la sincronizzazione iniziale è già stata eseguita, accedere e selezionare i campi da sincronizzare con Marketo.

1. Vai all&#39;amministratore e seleziona **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fare clic su **[!UICONTROL Edit]** in Dettagli sincronizzazione campi.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e selezionalo. Il nome effettivo deve essere new_synctomkto, ma il nome visualizzato può essere qualsiasi cosa. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Bene, ora hai attivato il filtro di sincronizzazione per Marketo.

## Crea un flusso di lavoro [!DNL Dynamics] per assegnare automaticamente i valori del filtro di sincronizzazione {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

È sempre possibile assegnare manualmente un valore ai campi SyncToMkto dei record. Ma perché non sfruttare la potenza di un flusso di lavoro [!DNL Dynamics] e assegnare automaticamente un valore al campo SyncToMkto quando un record viene creato o aggiornato?

>[!NOTE]
>
>Impossibile eseguire questa operazione a livello di database. Deve essere eseguito nel CRM manualmente o utilizzando un flusso di lavoro.
>
>Un flusso di lavoro [!DNL Dynamics] funziona solo sui nuovi record creati in futuro, non sui dati storici. Utilizzare un aggiornamento batch per spostarsi sui record esistenti.

1. Vai a Dynamics CRM. Fare clic su **Impostazioni**, quindi su **Processi**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Fai clic su **[!UICONTROL New]**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Immettere un nome per il workflow e selezionare **[!UICONTROL Workflow]** come [!UICONTROL Category] e **[!UICONTROL Lead]** come [!UICONTROL Entity]. Quindi fare clic su **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Crea regole per assegnare un valore true o false al campo **SyncToMkto** in base alle preferenze della tua organizzazione. Fai clic su **[!UICONTROL Save and Close]**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Definire un&#39;azione predefinita dopo aver fatto clic su **[!UICONTROL Add Step]** per aggiungere una condizione di controllo. Imposta i record che non desideri sincronizzare su **No**. In caso contrario, verranno sincronizzati.

1. Selezionare il workflow e fare clic su **[!UICONTROL Activate]**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Consulta [Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"} per impostare regole per sincronizzare solo i record per gli utenti con indirizzi e-mail.

## Dettagli filtro di sincronizzazione {#sync-filter-details}

Di seguito sono riportati alcuni dettagli di implementazione che pensavamo dovessi conoscere:

* Avvia un&#39;operazione di sincronizzazione

  Quando il valore **SyncToMkto** cambia da **No** a **Sì**, [!DNL Dynamics] notifica immediatamente a Marketo l&#39;avvio della sincronizzazione del record. Se il record esiste già, Marketo lo aggiorna. In caso contrario, Marketo crea il record.

* Interrompere un&#39;operazione di sincronizzazione

  Quando il valore SyncToMkto di un record viene modificato da Sì a No, a Marketo viene notificato di interrompere la sincronizzazione del record. Tuttavia, il record non viene eliminato, ma smette di ricevere aggiornamenti e diventa obsoleto.

>[!MORELIKETHIS]
>
>* [Filtro di sincronizzazione Microsoft Dynamics: qualificato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md){target="_blank"}
>* [Filtro sincronizzazione Microsoft Dynamics: Unisci](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md){target="_blank"}
>* [Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}
