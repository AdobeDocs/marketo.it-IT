---
unique-page-id: 11378812
description: Scopri account - Documenti Marketo - Documentazione di prodotto
title: Scopri account
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---


# Scopri account {#discover-accounts}

Utilizzate l&#39;opzione Scopri per identificare potenziali account target.

## Scopri gli account CRM {#discover-crm-accounts}

Identificare potenziali account di destinazione dal CRM.

>[!NOTE]
>
>Dopo aver collegato CRM a Marketo ABM, **Scopri account CRM** mostrerà tutti gli account CRM e le informazioni pertinenti per aiutarti a scegliere gli account denominati giusti. Marketo aggiunge informazioni aggiuntive oltre a quelle ricevute dal CRM.

**Persone** (In Scopri Account CRM E Scopri Società Marketo): Include sia Contatti che Lead. I lead possono essere scoperti utilizzando la corrispondenza lead-to-account di Marketo [](http://docs.marketo.com/display/DOCS/Lead+to+Account+Matching). **Persone**  Potenziali (In Scopri Account CRM E Scopri Società Marketo): Mostra quanti lead ha trovato Marketo che potrebbe appartenere a un account CRM.

**Campo**  CRM personalizzato (solo in Scopri account CRM): Questo ti aiuterà ad allineare la tua organizzazione di vendita e marketing per la selezione di account di destinazione corretti. Una volta che [mappate il campo CRM personalizzato](http://docs.marketo.com/x/1wnG) con Marketo ABM, vi mostreremo i dati mappati per aiutarvi a identificare i vostri account di destinazione.

1. In Account denominati, fai clic sul menu a discesa **Nuovo** e seleziona **Scopri account CRM**.

   ![](assets/disc-crm-one.png)

1. Viene aperta una nuova finestra/scheda. Selezionare gli account CRM che si desidera aggiungere agli account denominati e fare clic su **Avanti**.

   ![](assets/disc-crm-two.png)

1. La schermata di anteprima conferma la quantità di selezioni effettuate. Fare clic su **Crea**.

   ![](assets/disc-three.png)

   È tutto quello che c&#39;è da fare!

   ![](assets/disc-four.png)

## Scopri le aziende Marketo {#discover-marketo-companies}

Identificate le aziende giuste per il targeting.

>[!NOTE]
>
>In Scopri le società Marketo vedrai le società Marketo che non sono venute dal CRM.

1. In Account denominati, fare clic sul menu a discesa **New** e selezionare **Discover Marketo Companies**.

   ![](assets/one-1.png)

1. Viene aperta una nuova finestra/scheda. Selezionate le società da aggiungere agli account denominati e fate clic su **Next**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >In Scopri le aziende Marketo e Scopri CRM, Marketo automaticamente:
   >
   > * Trova le persone del database Marketo che hanno la società indicata nel record. Se visualizzi più valori per alcuni degli attributi (ad es. Industria), è perché Marketo ha trovato valori diversi elencati per queste singole persone. L&#39;attributo con il maggior numero di hit vince
   >
   >Solo in **Scopri CRM**, Marketo automaticamente:
   >
   > * Sincronizza e associa i contatti CRM con l&#39;account denominato
   >
   >Solo in **Scopri Marketo Companies**, Marketo automaticamente:
   >
   > * Consente di escludere la maggior parte dei provider di servizi Internet e dei domini pubblici (ad esempio [Yahoo.com](https://yahoo.com), [Gmail.com](https://gmail.com) come nome della società
      >
      > 
   * Deduce gli account CRM. Se hai &quot;Acme&quot; in un record e &quot;Acme Inc&quot; (o uno dei seguenti suffissi: Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, LP, Ltd, PA, PC, PLC, PLLC), li fonderemo in ABM come &quot;Acme&quot;
   >
   >Se desideri che Marketo degeneri gli account in base all&#39;ID CRM o al proprietario dell&#39;account invece che in base al nome della società, contatta il [Supporto marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Fate clic sulla freccia rivolta verso il basso sotto la colonna Account con nome per visualizzare l’elenco a discesa.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >In futuro, tutte le nuove persone provenienti da queste società selezionate saranno automaticamente assegnate ai rispettivi account denominati. Verifica due volte queste società e accertati che siano assegnate all&#39;account denominato corretto.

1. Per selezionare un account esistente, fate clic sul menu a discesa **Account denominato**, scegliete l&#39;account desiderato, quindi fate clic su **Avanti**.

   ![](assets/disc-comp-four.png)

   Potete anche creare un nuovo account denominato digitando il nome desiderato direttamente nella casella a discesa. Al termine, fai clic lontano dalla casella...

   ![](assets/disc-comp-five.png)

   ...e vedrai il tuo nuovo Account con nome. A questo punto, fai clic su **Next** come nel passaggio 4.

   ![](assets/disc-comp-six.png)

1. Fare clic su **Crea**.

   ![](assets/disc-comp-seven.png)

   Bel lavoro!

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>Se si verifica una mancata corrispondenza tra gli account CRM selezionati e ciò che si trova nella griglia di Discover CRM, è probabile che sia dovuto a uno o più dei seguenti elementi:
>
>* Avere diversi account CRM con nomi simili che sono stati annullati
>* La successiva sincronizzazione pianificata non si è ancora verificata


>[!MORELIKETHIS]
>
>* [Lead per corrispondenza account](/help/marketo/product-docs/account-based-marketing/target/named-accounts/lead-to-account-matching.md)

