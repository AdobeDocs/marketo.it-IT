---
unique-page-id: 2950682
description: Creazione di un canale di programma - Documentazione di Marketo - Documentazione del prodotto
title: Creare un canale del programma
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Creare un canale del programma {#create-a-program-channel}

Un programma è una specifica iniziativa di marketing. Il canale deve essere il meccanismo di consegna, ad esempio webinar, sponsorizzazione o annunci online.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>Ulteriori informazioni su [programmi](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), l&#39;elemento più importante di Marketo.

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/create-a-program-channel-1.png)

1. Fai clic su **[!UICONTROL Tag]**.

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >Perché utilizzare i tag? Un canale è un modo per descrivere un programma, proprio come gli altri tag. Il canale ha solo speciali funzionalità extra.

1. Fai clic sul segno **+** accanto a [!UICONTROL Canale] per espandere e visualizzare i canali esistenti.

   ![](assets/create-a-program-channel-3.png)

1. In **[!UICONTROL Nuovo]**, fai clic su **[!UICONTROL Nuovo canale]**.

   ![](assets/create-a-program-channel-4.png)

   >[!NOTE]
   >
   >**Esempio**
   >
   >Canale: Affissioni
   >
   >* Applica a: predefinito
   >* Progressione: membro, coinvolto (in caso di dubbi, funzionano correttamente)
   >* Completato: Coinvolto
   >
   >Canale: Party
   >
   >* Applica a: Evento
   >* Progressione: Invitato, Registrato, No Show e Partecipato
   >* Operazione completata: partecipazione avvenuta
   >
   >Consulta le Progressioni dei canali esistenti per scoprire come utilizzarli.

1. Prendiamo l&#39;esempio del canale del partito. Assegna un nome al nuovo **Canale** e seleziona il tipo di programma a cui verrà applicato.

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >Applicare a cosa? Esistono diversi tipi di programmi. Abbina il canale al tipo corretto. In caso di dubbi, scegliere **[!UICONTROL Predefinito]**.

   >[!NOTE]
   >
   >Quando si utilizza &quot;[!UICONTROL Event with Webinar]&quot;, le mappature di sistema verranno bloccate (come richiesto dalle integrazioni del webinar) e non possono essere modificate.

1. Immettere i primi due nomi di stato del programma, quindi fare clic su **[!UICONTROL Aggiungi passaggio]**.

   ![](assets/create-a-program-channel-6.png)

1. Immetti un altro programma **[!UICONTROL Stato]** e il numero del **[!UICONTROL Passaggio]**, quindi fai clic su **[!UICONTROL Aggiungi passaggio]**.

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >Il numero del **[!UICONTROL passaggio]** viene utilizzato per ordinare gli stati dei programmi. Tieni presente che le persone non possono tornare indietro in questi passaggi di progressione. Possono cambiare lo stato solo a uno stato con valore maggiore o uguale. Utilizzare i valori uguali quando gli stati sono destinati a passare da una progressione all&#39;altra.

1. Immetti l&#39;ultimo programma **[!UICONTROL Stato]** e il numero del **[!UICONTROL Passaggio]**.

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >Quando si utilizza il tipo &quot;[!UICONTROL Event]&quot;, è necessario il mapping di sistema per gli stati Registrato, In lista d&#39;attesa e Partecipato. Di conseguenza, tali stati non possono essere nascosti.

1. Scegli lo **[!UICONTROL stato di archiviazione mobile]** per **[!UICONTROL Registrato]**.

   ![](assets/create-a-program-channel-9.png)

1. Selezionare lo **[!UICONTROL stato archiviazione dispositivi mobili]** per **[!UICONTROL Partecipazione avvenuta]**.

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >Le opzioni di **[!UICONTROL Stato archiviazione dispositivi mobili]** saranno disponibili solo se il canale sarà per i programmi evento.

   >[!NOTE]
   >
   >Solo le persone con **[!UICONTROL Stato archiviazione dispositivi mobili]** di **[!UICONTROL Registrato]** e **[!UICONTROL Partecipato]** saranno visibili nelle [App archiviazione dispositivi mobili](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md).

   >[!TIP]
   >
   >Se nell&#39;app di archiviazione per dispositivi mobili viene creata una nuova persona, questa verrà impostata su Registrata nel programma dell&#39;evento. Se una persona viene registrata nell’evento nell’app, verrà impostata su Partecipato nel programma dell’evento.

1. Seleziona lo stato del programma **[!UICONTROL Operazione completata]**, quindi fai clic su **[!UICONTROL Crea]**.

   ![](assets/create-a-program-channel-11.png)

   Ben fatto! Quando crei un nuovo programma di quel tipo, questo nuovo canale sarà una delle scelte.
