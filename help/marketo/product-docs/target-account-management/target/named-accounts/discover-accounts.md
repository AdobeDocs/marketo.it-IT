---
unique-page-id: 11378812
description: Esplorare gli account - Documentazione di Marketo - Documentazione del prodotto
title: Individua account
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Individua account {#discover-accounts}

Utilizza l’opzione Discover per identificare potenziali account di destinazione.

## [!UICONTROL Discover CRM Accounts] {#discover-crm-accounts}

Identifica potenziali account di destinazione dal tuo CRM.

>[!NOTE]
>
>Dopo aver collegato il CRM al TAM di Marketo, **[!UICONTROL Discover CRM Accounts]** visualizzerà tutti gli account CRM e le informazioni rilevanti per aiutarti a scegliere gli account denominati corretti. Marketo aggiunge ulteriori informazioni oltre a quelle ricevute dal sistema CRM.

**[!UICONTROL People]** (In [!UICONTROL Discover CRM Accounts] e [!UICONTROL Discover Marketo Companies]): Include sia contatti che lead. I lead possono essere rilevati utilizzando la corrispondenza [lead-account](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md) di Marketo.

**[!UICONTROL Potential People]** (in [!UICONTROL Discover CRM Accounts] e [!UICONTROL Discover Marketo Companies]): mostra il numero di lead trovati da Marketo che potrebbero appartenere a un account CRM.

**Campo CRM personalizzato** (solo in Discover CRM Accounts): ti aiuterà ad allineare la tua organizzazione di vendita e marketing per la selezione di account di destinazione corretti. Una volta [mappato il campo CRM personalizzato](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) con Marketo TAM, ti mostreremo i dati mappati per aiutarti a identificare i tuoi account di destinazione.

1. In [!UICONTROL Named Accounts], fare clic sul menu a discesa **[!UICONTROL New]** e selezionare **[!UICONTROL Discover CRM Accounts]**.

   ![](assets/disc-crm-one.png)

1. Viene aperta una nuova finestra o scheda. Selezionare gli account CRM da aggiungere a [!UICONTROL Named Accounts] e fare clic su **[!UICONTROL Next]**.

   ![](assets/disc-crm-two.png)

1. La schermata di anteprima conferma la quantità di selezioni effettuate. Fai clic su **[!UICONTROL Create]**.

   ![](assets/disc-three.png)

   È tutto qui!

   ![](assets/disc-four.png)

## [!UICONTROL Discover Marketo Companies] {#discover-marketo-companies}

Identifica le aziende giuste per il targeting.

>[!NOTE]
>
>In [!UICONTROL Discover Marketo Companies], vedrai aziende Marketo che non provengono dal tuo CRM.

1. In [!UICONTROL Named Accounts], fare clic sul menu a discesa **[!UICONTROL New]** e selezionare **[!UICONTROL Discover Marketo Companies]**.

   ![](assets/one-1.png)

1. Viene aperta una nuova finestra o scheda. Selezionare le società da aggiungere a [!UICONTROL Named Accounts] e fare clic su **[!UICONTROL Next]**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >In [!UICONTROL Discover Marketo Companies] e Individua CRM, Marketo automaticamente:
   >
   >* Trova gli utenti del database Marketo che hanno tale società elencata nel record. Se vedi più valori per alcuni degli attributi (ad esempio, Industria), è perché Marketo ha trovato valori diversi elencati per queste singole persone. L’attributo con il maggior numero di hit vince
   >
   >Solo in **Individua CRM**, Marketo automaticamente:
   >
   >* Sincronizza e associa i contatti CRM con [!UICONTROL Named Account]
   >
   >Solo in **[!UICONTROL Discover Marketo Companies]**, Marketo automaticamente:
   >
   >* Filtra la maggior parte dei provider di servizi Internet e dei domini pubblici (ad esempio, yahoo.com, gmail.com) come nomi di società
   >
   >* Deduplica gli account CRM. Se hai &quot;Acme&quot; in un record e &quot;Acme Inc&quot; (o uno qualsiasi dei seguenti suffissi: Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, LP, Ltd, PA, PC, PLC, PLLC), li uniremo in TAM come semplicemente &quot;Acme&quot;

1. Fare clic sulla freccia giù sotto la colonna [!UICONTROL Named Account] per visualizzare il menu a discesa.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >In futuro, tutte le nuove persone di queste società selezionate verranno automaticamente assegnate ai loro rispettivi account denominati. Controllare queste società e assicurarsi che siano assegnate a [!UICONTROL Named Account] corretto.

1. Per selezionare un account esistente, fare clic sull&#39;elenco a discesa **[!UICONTROL Named Account]**, scegliere l&#39;account desiderato, quindi fare clic su **[!UICONTROL Next]**.

   ![](assets/disc-comp-four.png)

   È inoltre possibile creare un nuovo [!UICONTROL Named Account] digitando il nome desiderato direttamente nella casella a discesa. Al termine, fai clic lontano dalla casella...

   ![](assets/disc-comp-five.png)

   ...e vedrai il tuo nuovo [!UICONTROL Named Account]. A questo punto fare clic su **[!UICONTROL Next]** come nel passaggio 4.

   ![](assets/disc-comp-six.png)

1. Fai clic su **[!UICONTROL Create]**.

   ![](assets/disc-comp-seven.png)

   Bel lavoro!

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>Se noti una mancata corrispondenza tra gli account CRM selezionati e quelli presenti nella griglia di individuazione CRM, è probabile che sia dovuta a una o più delle seguenti cause:
>
>* Avere account CRM diversi con nomi simili che sono stati deduplicati
>* La prossima sincronizzazione pianificata non è ancora avvenuta

>[!MORELIKETHIS]
>
>[Lead per corrispondenza account](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
