---
unique-page-id: 11378812
description: Scopri gli account - Documenti Marketo - Documentazione del prodotto
title: Scopri account
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Scopri account {#discover-accounts}

Utilizza l’opzione Scopri per identificare potenziali account target.

## Scopri gli account CRM {#discover-crm-accounts}

Identifica potenziali account target dal CRM.

>[!NOTE]
>
>Dopo aver collegato il CRM a Marketo TAM, **Scopri gli account CRM** mostrerà tutti gli account CRM e le informazioni rilevanti per aiutarti a scegliere gli account denominati giusti. Marketo aggiunge ulteriori informazioni su ciò che viene ricevuto dal CRM.

**Persone** (In Scopri gli account CRM e scopri le società Marketo): Include sia Contatti che Lead. I lead possono essere scoperti utilizzando Marketo [corrispondenza lead-to-account](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md).

**Persone potenziali** (In Scopri gli account CRM e scopri le società Marketo): Mostra quanti lead Marketo ha trovato che potrebbero appartenere a un account CRM.

**Campo CRM personalizzato** (Solo in Scopri account CRM): Questo ti aiuterà ad allineare la tua organizzazione di vendita e marketing per la selezione di account di destinazione corretti. Una volta [mappa il campo CRM personalizzato](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) con Marketo TAM, ti mostreremo i dati mappati per aiutarti a identificare gli account di destinazione.

1. In Account denominati, fai clic sul pulsante **Nuovo** a discesa e seleziona **Scopri gli account CRM**.

   ![](assets/disc-crm-one.png)

1. Viene aperta una nuova finestra/scheda. Seleziona gli account CRM che desideri aggiungere ai tuoi account denominati e fai clic su **Successivo**.

   ![](assets/disc-crm-two.png)

1. La schermata di anteprima conferma la quantità di selezioni effettuate. Fai clic su **Crea**.

   ![](assets/disc-three.png)

   È tutto quello che c&#39;è da fare!

   ![](assets/disc-four.png)

## Scopri le aziende Marketo {#discover-marketo-companies}

Identifica le aziende giuste per il targeting.

>[!NOTE]
>
>In Scopri le società Marketo vedrai le società Marketo che non provengono dal tuo sistema di gestione delle relazioni con i clienti.

1. In Account denominati, fai clic sul pulsante **Nuovo** a discesa e seleziona **Scopri le aziende Marketo**.

   ![](assets/one-1.png)

1. Viene aperta una nuova finestra/scheda. Seleziona le società da aggiungere ai tuoi account denominati e fai clic su **Successivo**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >In Scopri le aziende Marketo e Scopri CRM, Marketo automaticamente:
   >
   >* Trova le persone del database Marketo per le quali l&#39;azienda è elencata nel record. Se visualizzi più valori per alcuni degli attributi (ad esempio, Settore), è perché Marketo ha trovato valori diversi elencati per quelle singole persone. L&#39;attributo con il maggior numero di hit vince
   >
   >In **Scopri CRM** Solo, Marketo automaticamente:
   >
   >* Sincronizza e associa i contatti CRM con l&#39;account denominato
   >
   >In **Scopri le aziende Marketo** Solo, Marketo automaticamente:
   >
   >* Filtra la maggior parte dei provider di servizi Internet e i domini pubblici (ad esempio, yahoo.com, gmail.com) come nomi aziendali
   >
   >* Deduce gli account CRM. Se hai &quot;Acme&quot; in un record e &quot;Acme Inc&quot; (o uno dei seguenti suffissi: Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, LP, Ltd, PA, PC, PLC, PLLC), le fonderemo in TAM come &quot;Acme&quot;

   >
   >Se desideri che Marketo deduplichi gli account per ID CRM o per proprietario dell&#39;account invece che per nome società, contatta [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Fai clic sulla freccia rivolta verso il basso sotto la colonna Account con nome per visualizzare il menu a discesa.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >In futuro, tutte le nuove persone provenienti da queste società selezionate saranno automaticamente assegnate ai rispettivi account denominati. Controlla queste aziende e assicurati che siano assegnate all&#39;account con nome corretto.

1. Per selezionare un account esistente, fai clic sul pulsante **Account denominato** a discesa, scegli l’account desiderato, quindi fai clic su **Successivo**.

   ![](assets/disc-comp-four.png)

   Puoi anche creare un nuovo account con nome digitando il nome desiderato direttamente nella casella a discesa. Al termine, fai clic lontano dalla casella..

   ![](assets/disc-comp-five.png)

   ...e vedrai il tuo nuovo account denominato. A quel punto, fai clic su **Successivo** come nel passaggio 4.

   ![](assets/disc-comp-six.png)

1. Fai clic su **Crea**.

   ![](assets/disc-comp-seven.png)

   Ottimo lavoro!

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>Se si verifica una mancata corrispondenza tra gli account CRM selezionati e ciò che si trova nella griglia di Discover CRM, è probabile che ciò sia dovuto a uno o più dei seguenti elementi:
>
>* Avere diversi account CRM con nomi simili che sono stati deduplicati
>* La successiva sincronizzazione pianificata non si è ancora verificata


>[!MORELIKETHIS]
>
>[Corrispondenza lead a conto](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
