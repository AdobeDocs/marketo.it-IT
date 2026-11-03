---
unique-page-id: 7512270
description: Aggiungi Adobe Connect as a LaunchPoint Service in modo che Marketo gestisca la registrazione e la partecipazione ai webinar.
title: Aggiungi [!DNL Adobe Connect] come servizio [!DNL LaunchPoint]
exl-id: 21beb156-6674-46a8-bdc5-345fcb4bb272
feature: Administration, Integrations
TQID: https://experienceleague.adobe.com/5FY-AYMAy60RGDnuFas2QP1PexqhIMohWh8egyllFNY
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f9fe6ecbdea51b51d14bd3faeef52ca9c02c831b
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 1%
---
# Aggiungi [!DNL Adobe Connect] come servizio [!DNL LaunchPoint] {#add-adobe-connect-as-a-launchpoint-service}

Marketo gestisce la registrazione e la partecipazione al webinar [!DNL Adobe Connect].

>[!PREREQUISITES]
>
>* Sono necessari una sottoscrizione esistente a [!DNL Adobe Connect] e diritti di amministrazione. Sono disponibili i seguenti dettagli: nome utente, password, password partecipante e URL della cartella della riunione.

>[!NOTE]
>
>* **Autorizzazioni amministratore richieste**
>* [!DNL Adobe Connect On Site] non è attualmente supportato.

1. Nel Marketo personale, fare clic su **[!UICONTROL Admin]**.

1. In **[!UICONTROL Integration]**, selezionare **[!UICONTROL LaunchPoint]**.

   ![](assets/add-adobe-connect-as-a-launchpoint-service-1.png)

1. Fare clic su **[!UICONTROL New]** e selezionare **[!UICONTROL New Service]**.

   ![](assets/add-adobe-connect-as-a-launchpoint-service-2.png)

1. Immetti **[!UICONTROL Display Name]**. Nel menu a discesa **[!UICONTROL Service]**, selezionare **[!UICONTROL Adobe Connect]**.

   ![](assets/add-adobe-connect-as-a-launchpoint-service-3.png)

1. Immetti **[!UICONTROL Username]**, **[!UICONTROL Access Code]**, **[!UICONTROL Meeting Folder URL]** e **[!UICONTROL Participant Password]**, quindi fai clic su **[!UICONTROL Create]**.

   ![](assets/add-adobe-connect-as-a-launchpoint-service-4.png)

   >[!TIP]
   >
   >Quando crei la password del partecipante, il valore scelto viene incluso in una stringa di query quando i collegamenti vengono inviati per l&#39;evento. Si consiglia di renderlo di facile utilizzo per il cliente.

   >[!NOTE]
   >
   >Dopo aver effettuato l&#39;accesso all&#39;account [!DNL Adobe Connect], selezionare la scheda **[!UICONTROL Seminars]**. Senza approfondire in alcun seminario specifico, copia l&#39;URL dalla barra del browser nell&#39;impostazione **[!UICONTROL Meeting Folder URL]**.

Il servizio [!DNL Adobe Connect] è ora sincronizzato con Marketo Engage.

>[!MORELIKETHIS]
>
>Scopri come [creare un evento con [!DNL Adobe Connect]](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-adobe-connect.md){target="_blank"}.
