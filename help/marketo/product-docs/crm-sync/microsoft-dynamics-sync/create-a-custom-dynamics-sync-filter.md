---
unique-page-id: 9437903
description: Creare un filtro di sincronizzazione di Dynamics personalizzato - Documenti Marketo - Documentazione del prodotto
title: Creare un filtro di sincronizzazione di Dynamics personalizzato
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
source-git-commit: ed4699ea4a94c787b8af109599f2a0c50591b956
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# Creare un filtro di sincronizzazione di Dynamics personalizzato {#create-a-custom-dynamics-sync-filter}

Non vuoi sincronizzare tutti gli elementi di Dynamics CRM in Marketo? Non ti preoccupare! Marketo consente di impostare un filtro di sincronizzazione e sincronizzare solo una parte dei record.

## Panoramica {#overview}

Per impostare un filtro di sincronizzazione Dynamics:

1. Crea un campo personalizzato Due opzioni (booleano) denominato new_synctomkto in Dynamics CRM per qualsiasi oggetto (lead, contatti, account, opportunità e altre entità personalizzate).
1. Assegnare un valore Sì/No a questo campo o lasciarlo vuoto.

>[!NOTE]
>
>Devi apportare queste modifiche in Dynamics CRM, non nel database o in Marketo.

Marketo cerca questo campo durante la sincronizzazione automatica in background e determina su quali record sincronizzare in base a questa logica:

| Valore campo | Sincronizzazione con Marketo? |
|---|---|
| Il campo non esiste | Sì |
| Campo vuoto | Sì |
| Il campo ha il valore Sì | Sì |
| Campo con valore No | No |

>[!CAUTION]
>
>L’unico modo per dire a Marketo di saltare un record è quello di impostare esplicitamente il valore del campo per **No**. Marketo continua a sincronizzare i record anche se i valori dei campi sono vuoti.

>[!PREREQUISITES]
>
>Installa la versione più recente del plug-in Marketo (3.0.0.1 o successivo). Vai a Marketo > Amministratore > Microsoft Dynamics > Scarica soluzione Marketo.

## Crea campo SyncToMkto {#create-synctomkto-field}

1. Accedi a Dynamics CRM. Fai clic su **Impostazioni** quindi fai clic su **Personalizzazioni**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Fai clic su **Personalizzare il sistema**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Fai clic su ![](assets/image2015-8-10-21-3a44-3a23.png) accanto a **Entità**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Fai clic su ![](assets/image2015-8-10-21-3a44-3a23.png) accanto a **Lead** e seleziona **Campi**. Quindi fai clic su **Nuovo**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Invio **SyncToMkto** in **Nome visualizzato** campo e seleziona **Due opzioni** come **Tipo di dati**. Quindi fai clic su **Salva e chiudi**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Scegliere un nome visualizzato qualsiasi per questo campo, ma il campo Nome deve essere esattamente **new_synctomkto**. È necessario utilizzare **nuovo** come prefisso predefinito. Se hai modificato il valore predefinito, vai qui in [reimpostare il prefisso predefinito per i nomi dei campi personalizzati](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md). È possibile modificarlo nuovamente dopo aver creato i nuovi campi.

   >[!NOTE]
   >
   >Se si dispone di un flusso di lavoro asincrono impostato, il record ottiene il valore predefinito SyncToMkto configurato nel campo e ottiene il valore corretto qualche secondo dopo al termine dell&#39;esecuzione del flusso di lavoro. Se il valore predefinito è impostato su Sì, tali record verranno creati in Marketo e quindi diventano obsoleti. Utilizzo **No** come valore predefinito per evitare questo problema.

1. Ripeti questo processo e crea il **SyncToMkto** per qualsiasi altra entità su cui si desidera limitare la sincronizzazione, ad esempio contatti, account, opportunità ed entità personalizzate.

## Selezionare il filtro in Marketo {#select-the-filter-in-marketo}

Anche se hai già eseguito la sincronizzazione iniziale, accedi e seleziona i campi da sincronizzare con Marketo.

1. Vai ad Amministratore e seleziona **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fai clic su **Modifica** in Dettagli sincronizzazione campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e controllalo. Il nome effettivo deve essere new_synctomkto ma il nome visualizzato può essere qualsiasi cosa. Fai clic su **Salva**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Ottimo, ora hai abilitato il filtro di sincronizzazione per Marketo.

## Creare un flusso di lavoro Dynamics per assegnare automaticamente i valori dei filtri di sincronizzazione {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

Puoi sempre assegnare manualmente un valore ai campi SyncToMkto per i record. Ma perché non sfruttare la potenza di un flusso di lavoro Dynamics e assegnare automaticamente un valore al campo SyncToMkto quando viene creato o aggiornato un record?

>[!NOTE]
>
>Non è possibile eseguire questa operazione a livello di database. Deve essere eseguito manualmente nel sistema di gestione delle relazioni con i clienti o utilizzando un flusso di lavoro.
>
>Un flusso di lavoro di Dynamics funziona solo sui nuovi record creati in futuro, non sui dati storici. Utilizzare un aggiornamento batch per spostare i record esistenti.

1. Vai a Dynamics CRM. Fai clic su **Impostazioni** quindi fai clic su **Processi**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Fai clic su **Nuovo**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Immetti un nome per il flusso di lavoro e seleziona **Flusso di lavoro** come categoria e **Lead** come entità. Quindi fai clic su **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Creare regole per assegnare un valore true o false al **SyncToMkto** in base alle preferenze dell&#39;organizzazione. Fai clic su **Salva e chiudi**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Definire un’azione predefinita dopo aver fatto clic su **Aggiungi passaggio** per aggiungere una condizione di controllo. Questo imposta i record a cui non si desidera eseguire la sincronizzazione **No**. In caso contrario, verranno sincronizzati.

1. Seleziona il flusso di lavoro e fai clic su **Attiva**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Vedi [Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md) per impostare regole per sincronizzare solo i record per le persone con indirizzi e-mail.

## Dettagli filtro di sincronizzazione {#sync-filter-details}

Di seguito sono riportati alcuni dettagli di implementazione che ritenevi dovessero essere noti:

1. Avvia un&#39;operazione di sincronizzazione

   Quando il **SyncToMkto** modifiche di valore da **No** a **Sì**, Dynamics notifica immediatamente Marketo per avviare la sincronizzazione di questo record. Se il record esiste già, Marketo lo aggiorna. In caso contrario, Marketo crea il record.

   >[!TIP]
   >
   >A `Create [StartSync]` quando questo accade, viene aggiunta al registro Marketo.

1. Interrompere un&#39;operazione di sincronizzazione

   Quando un record modifica il valore SyncToMkto da Sì a No, Marketo riceve una notifica per interrompere la sincronizzazione del record. Tuttavia, il record non viene eliminato, smette invece di ricevere aggiornamenti e diventa obsoleto.

>[!MORELIKETHIS]
>
>* [Filtro di sincronizzazione Microsoft Dynamics: Qualifica](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md)
>* [Filtro di sincronizzazione Microsoft Dynamics: Unisci](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md)
>* [Regole filtro di sincronizzazione personalizzate per un indirizzo e-mail](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md)

