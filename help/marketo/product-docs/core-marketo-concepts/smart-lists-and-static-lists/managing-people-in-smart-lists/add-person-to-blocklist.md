---
unique-page-id: 9438139
description: Aggiungere una persona al  di Inserire nell'elenco Bloccati - Documenti Marketo - Documentazione del prodotto
title: Aggiungi persona a  Inserii nell'elenco Bloccati
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# Aggiungi persona a  Inserii nell&#39;elenco Bloccati {#add-person-to-blocklist}

L&#39;aggiunta di persone al Inserire nell&#39;elenco Bloccati di  impedisce loro di ricevere la vostra corrispondenza.

>[!NOTE]
>
>Marketo sta cambiando termini come Blacklist e Whitelist per  Inserii nell&#39;elenco Bloccati e  Inserire nell&#39;elenco Consentiti nel nostro prodotto. Nel corso di questo aggiornamento, i vecchi termini possono essere visualizzati nella nostra interfaccia utente e nelle schermate della documentazione, nonché i nuovi termini nel nostro testo della documentazione. Ci scusiamo per ogni confusione.

1. [Create un nuovo ](../../../../product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) programma predefinito e denominatelo  **Aggiungi a  Inserii nell&#39;elenco Bloccati**.
1. Fare clic su **Nuovo** e selezionare **Nuova risorsa locale**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Assegnate un nome all&#39;elenco e fate clic su **Crea**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Aggiungi tutte le persone al tuo **Smart List** che desideri aggiungere al tuo Inserire nell&#39;elenco Bloccati .

   >[!NOTE]
   >
   >Le persone sul Inserire nell&#39;elenco Bloccati  non riceveranno e-mail operative.

   ![](assets/three-6.png)

1. Fare clic su **New** e selezionare **New Smart Campaign**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Denominate la **Nuova campagna intelligente**. Fare clic su **Crea**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Trascinare **Membro di Smart List**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Selezionate l’elenco avanzato appena creato.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Trascinare **Modifica valore dati**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Per **Flusso**, immettere **Blocca elencato** per l&#39; **Attributo** e impostare **Nuovo valore** su **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. Nella scheda **Pianificazione**, selezionare **Esegui una volta**.

   ![](assets/ten.png)

1. Selezionare **Esegui ora** e fare clic su **Esegui**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   SÌ! Queste persone non riceveranno più e-mail.

   >[!TIP]
   >
   >Creare una [campagna intelligente di attivazione](../../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) utilizzando **Change Data Value** con **Block List è true** per tutte le persone che in futuro avranno  attributi .

