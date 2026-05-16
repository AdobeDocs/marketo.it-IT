---
unique-page-id: 6095008
description: Collegamento [!DNL Google AdWords] a Marketo tramite LaunchPoint per caricare dati di conversione offline da utilizzare nei report in AdWords.
title: Aggiungi [!DNL Google AdWords] as a [!DNL LaunchPoint] Service
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
feature: Administration, Integrations
TQID: https://experienceleague.adobe.com/gpw57sy3WitNAh6g4mkajXuuFlRFzunZmfedM4aCrCk
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 259
ht-degree: 5%

---

# Aggiungi [!DNL Google AdWords] come servizio [!DNL LaunchPoint] {#add-google-adwords-as-a-launchpoint-service}

Collega l&#39;account [!DNL Google AdWords] a Marketo per caricare automaticamente i dati di conversione offline da Marketo a [!DNL Google AdWords]. Dall&#39;interfaccia utente di [!DNL AdWords], puoi vedere quali clic hanno generato lead qualificati, opportunità e nuovi clienti (o qualsiasi fase dei ricavi desideri monitorare) dopo [aver aggiunto colonne personalizzate](https://support.google.com/adwords/answer/3073556){target="_blank"} in [!DNL AdWords]. Queste informazioni non vengono visualizzate nell’interfaccia utente di Marketo.

Ulteriori informazioni sulla [funzionalità di importazione di conversione offline di Google](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Non tutti gli utenti di Marketo Engage hanno acquistato questa funzionalità. Per informazioni, contatta il team dell’account di Adobe (il tuo Account Manager).

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>È inoltre possibile integrare un servizio [[!DNL Google AdWords] as a [!DNL Launchpoint]  con un account manager](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md){target="_blank"}.

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-1.png)

1. Seleziona **[!UICONTROL LaunchPoint]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-2.png)

1. Selezionare **[!UICONTROL New]** e **[!UICONTROL New Service]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-3.png)

1. Immettere un [!UICONTROL display name] e selezionare **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-4.png)

1. Seleziona **[!UICONTROL Authorize Marketo]**.

   >[!NOTE]
   >
   >Assicurarsi di disconnettersi dall&#39;account [!DNL Gmail] personale e abilitare i popup.

   ![](assets/add-google-adwords-as-a-launchpoint-service-5.png)

1. Seleziona il tuo account associato a [!DNL Google AdWords].

   ![](assets/add-google-adwords-as-a-launchpoint-service-6.png)

1. Seleziona **[!UICONTROL Accept]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-7.png)

1. Lo stato viene visualizzato come **[!UICONTROL Success]**. Seleziona **[!UICONTROL Next]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-8.png)

1. Carica le conversioni offline da Marketo a [!DNL Google AdWords] **[!UICONTROL Weekly]** o **[!UICONTROL Daily]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-9.png)

1. Conversione degli attributi in **[!UICONTROL First Click]** o **[!UICONTROL Last Click]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-10.png)

   | Tipo | Definizione |
   |---|---|
   | [!UICONTROL First Click] | Le conversioni offline saranno attribuite al primo [!DNL AdWords] e a una persona che ha fatto clic negli ultimi 90 giorni |
   | [!UICONTROL Last Click] | Le conversioni offline saranno attribuite all&#39;ultimo [!DNL AdWords] e che una persona ha fatto clic |

   >[!NOTE]
   >
   >L&#39;utilizzo di un modello di attribuzione coerente in Marketo e [!DNL AdWords] fornisce i dati più precisi.

1. Fai clic su **[!UICONTROL Create]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-11.png)

   >[!NOTE]
   >
   >[Per il funzionamento di questa funzione è necessario selezionare l&#39;assegnazione automatica tag](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"}. La disattivazione deve essere eseguita in [!DNL AdWords].

Consulta l&#39;articolo correlato di seguito per scoprire come mappare [!DNL AdWords] conversioni offline nel tuo modello di ricavi.
