---
unique-page-id: 9438139
description: Aggiunta di una persona al Inserisco nell'elenco Bloccati di - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere persone all’elenco Bloccati
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 10%

---

# Aggiungere persone all’elenco Bloccati {#add-person-to-blocklist}

L’aggiunta di persone al tuo Elenco Bloccati di impedisce loro di ricevere la tua corrispondenza.

1. Creare un nuovo [programma predefinito](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} e denominarlo &quot;Aggiungi al Inserisco nell&#39;elenco Bloccati di&quot;.

1. Fare clic su **[!UICONTROL New]** e selezionare **[!UICONTROL New Local Asset]**.

   ![](assets/add-person-to-blocklist-1.png)

1. Seleziona **[!UICONTROL Smart List]**.

   ![](assets/add-person-to-blocklist-2.png)

1. Assegna un nome all&#39;elenco e fai clic su **[!UICONTROL Create]**.

   ![](assets/add-person-to-blocklist-3.png)

1. Aggiungi tutte le persone al tuo elenco avanzato che desideri aggiungere al tuo Inserisco nell&#39;elenco Bloccati di.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >Le persone nel tuo Inserisco nell&#39;elenco Bloccati di non riceveranno e-mail operative.

1. Torna al tuo programma.

   ![](assets/add-person-to-blocklist-5.png)

1. Fare clic su **[!UICONTROL New]** e selezionare **[!UICONTROL New Smart Campaign]**.

   ![](assets/add-person-to-blocklist-6.png)

1. Assegna un nome alla nuova Smart Campaign. Fai clic su **[!UICONTROL Create]**.

   ![](assets/add-person-to-blocklist-7.png)

1. Trascina **[!UICONTROL Member of Smart List]**.

   ![](assets/add-person-to-blocklist-8.png)

1. Seleziona l’elenco avanzato appena creato.

   ![](assets/add-person-to-blocklist-9.png)

1. Fai clic sulla scheda **[!UICONTROL Flow]**. Trascina e rilascia l&#39;azione di flusso **[!UICONTROL Change Data Value]**.

   ![](assets/add-person-to-blocklist-10.png)

1. Nell&#39;elenco a discesa **[!UICONTROL Attribute]** selezionare **[!UICONTROL Block Listed]** e impostare **[!UICONTROL New Value]** su **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Fare clic sulla scheda **[!UICONTROL Schedule]** e selezionare **[!UICONTROL Run Once]**.

   ![](assets/add-person-to-blocklist-12.png)

1. Seleziona **[!UICONTROL Run Now]** e fai clic su **[!UICONTROL Run]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Fare di nuovo clic su **[!UICONTROL Run]**.

   ![](assets/add-person-to-blocklist-14.png)

Queste persone non riceveranno più e-mail.

>[!TIP]
>
>Crea una [campagna Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} utilizzando **Modifica valore dati** con **Blocco inserito nell&#39;elenco true** per tutte le persone che in futuro avranno gli attributi che possono essere inseriti nell&#39;elenco Bloccati da.
