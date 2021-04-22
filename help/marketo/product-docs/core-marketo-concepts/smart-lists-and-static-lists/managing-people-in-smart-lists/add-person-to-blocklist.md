---
unique-page-id: 9438139
description: Aggiungi una persona all’Inserire nell'elenco Bloccati - Documenti Marketo - Documentazione del prodotto
title: Aggiungi persona a Inserire nell'elenco Bloccati
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Aggiungi persona all&#39;Inserire nell&#39;elenco Bloccati {#add-person-to-blocklist}

L&#39;aggiunta di persone al tuo Inserire nell&#39;elenco Bloccati impedisce loro di ricevere la tua corrispondenza.

>[!NOTE]
>
>Marketo sta cambiando termini come Blacklist e Whitelist in Inserii nell&#39;elenco Bloccati e Inserire nell&#39;elenco Consentiti nel nostro prodotto. Durante questo aggiornamento, potresti vedere i vecchi termini nella nostra interfaccia utente e le schermate della documentazione, e i nuovi termini nel nostro testo della documentazione. Ci scusiamo per ogni confusione.

1. [Crea un nuovo ](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) programma predefinito e denominalo  **Aggiungi all’Inserire nell&#39;elenco Bloccati**.

1. Fai clic su **Nuovo** e seleziona **Nuova risorsa locale**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Denomina l&#39;elenco e fai clic su **Crea**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Aggiungi tutte le persone al tuo **Smart List** che desideri aggiungere al tuo Inserire nell&#39;elenco Bloccati.

   >[!NOTE]
   >
   >Le persone sul tuo Inserire nell&#39;elenco Bloccati non riceveranno e-mail operative.

   ![](assets/three-6.png)

1. Fai clic su **Nuovo** e seleziona **Nuova campagna avanzata**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Assegna un nome alla **Nuova campagna avanzata**. Fare clic su **Crea**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Trascina **Membro di Smart List**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Seleziona l’elenco smart appena creato.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Trascina **Cambia valore dati**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Per il **Flusso**, immetti **Blocco elencato** per l&#39; **Attributo** e imposta **Nuovo valore** su **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. Nella scheda **Pianificazione**, selezionare **Esegui una volta**.

   ![](assets/ten.png)

1. Seleziona **Esegui ora** e fai clic su **Esegui**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   SÌ! Queste persone non riceveranno più e-mail.

   >[!TIP]
   >
   >Crea una [trigger smart campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) utilizzando **Change Data Value** con **Block List è true** per tutte le persone che in futuro avranno attributi inseriti nell&#39;elenco Bloccati.
