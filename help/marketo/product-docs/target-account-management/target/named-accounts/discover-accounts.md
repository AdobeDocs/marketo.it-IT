---
unique-page-id: 11378812
description: Esplorare gli account - Documentazione di Marketo - Documentazione del prodotto
title: Individua account
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
feature: Target Account Management
source-git-commit: dd4c8472ec3f453462bd8046daf70c89c587724a
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Individua account {#discover-accounts}

Utilizza l’opzione Discover per identificare potenziali account di destinazione.

## Scopri gli account CRM {#discover-crm-accounts}

Identifica potenziali account di destinazione dal tuo CRM.

>[!NOTE]
>
>Dopo aver collegato il CRM al TAM di Marketo, **Scopri gli account CRM** mostrerà tutti gli account CRM e le informazioni rilevanti per aiutarti a scegliere gli account denominati corretti. Marketo aggiunge ulteriori informazioni oltre a quelle ricevute dal sistema CRM.

**Persone** (In Discover CRM Accounts &amp; Discover Marketo Companies): Include sia contatti che lead. I lead possono essere rilevati utilizzando la corrispondenza [lead-account](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md) di Marketo.

**Persone potenziali** (in Discover CRM Accounts &amp; Discover Marketo Companies): mostra quanti lead Marketo ha trovato che potrebbero appartenere a un account CRM.

**Campo CRM personalizzato** (solo in Discover CRM Accounts): ti aiuterà ad allineare la tua organizzazione di vendita e marketing per la selezione di account di destinazione corretti. Una volta [mappato il campo CRM personalizzato](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) con Marketo TAM, ti mostreremo i dati mappati per aiutarti a identificare i tuoi account di destinazione.

1. In Account denominati fare clic sull&#39;elenco a discesa **Nuovo** e selezionare **Individua account CRM**.

   ![](assets/disc-crm-one.png)

1. Viene aperta una nuova finestra o scheda. Seleziona gli account CRM che desideri aggiungere ai tuoi account denominati e fai clic su **Avanti**.

   ![](assets/disc-crm-two.png)

1. La schermata di anteprima conferma la quantità di selezioni effettuate. Fai clic su **Crea**.

   ![](assets/disc-three.png)

   È tutto qui!

   ![](assets/disc-four.png)

## Scopri le aziende Marketo {#discover-marketo-companies}

Identifica le aziende giuste per il targeting.

>[!NOTE]
>
>In Discover Marketo Companies, vedrai aziende Marketo che non provengono dal tuo sistema CRM.

1. In Account denominati fare clic sull&#39;elenco a discesa **Nuovo** e selezionare **Individua società Marketo**.

   ![](assets/one-1.png)

1. Viene aperta una nuova finestra o scheda. Seleziona le società da aggiungere ai tuoi account denominati e fai clic su **Avanti**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >In Discover Marketo Companies and Discover CRM, Marketo automaticamente:
   >
   >* Trova gli utenti del database Marketo che hanno tale società elencata nel record. Se vedi più valori per alcuni degli attributi (ad esempio, Industria), è perché Marketo ha trovato valori diversi elencati per queste singole persone. L’attributo con il maggior numero di hit vince
   >
   >Solo in **Individua CRM**, Marketo automaticamente:
   >
   >* Sincronizza e associa i contatti CRM con l&#39;account denominato
   >
   >Solo in **Individua società Marketo**, Marketo:
   >
   >* Filtra la maggior parte dei provider di servizi Internet e dei domini pubblici (ad esempio, yahoo.com, gmail.com) come nomi di società
   >
   >* Deduplica gli account CRM. Se hai &quot;Acme&quot; in un record e &quot;Acme Inc&quot; (o uno qualsiasi dei seguenti suffissi: Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, LP, Ltd, PA, PC, PLC, PLLC), li uniremo in TAM come semplicemente &quot;Acme&quot;

1. Fai clic sulla freccia rivolta verso il basso sotto la colonna Account denominato per visualizzare il menu a discesa.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >In futuro, tutte le nuove persone di queste società selezionate verranno automaticamente assegnate ai loro rispettivi account denominati. Ricontrollare queste società e assicurarsi che siano assegnate all&#39;account denominato corretto.

1. Per selezionare un account esistente, fai clic sull&#39;elenco a discesa **Account denominato**, scegli l&#39;account desiderato, quindi fai clic su **Avanti**.

   ![](assets/disc-comp-four.png)

   Puoi anche creare un nuovo Account denominato digitando il nome desiderato direttamente nella casella a discesa. Al termine, fai clic lontano dalla casella...

   ![](assets/disc-comp-five.png)

   ...e vedrai il tuo nuovo account con nome. A questo punto, fai clic su **Avanti** come nel passaggio 4.

   ![](assets/disc-comp-six.png)

1. Fai clic su **Crea**.

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
