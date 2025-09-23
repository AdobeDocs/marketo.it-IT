---
unique-page-id: 11375827
description: Campi obbligatori per la sincronizzazione di Marketo con Dynamics - Documentazione di Marketo - Documentazione del prodotto
title: Campi obbligatori per la sincronizzazione di Marketo con Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 6%

---

# Campi obbligatori per la sincronizzazione di Marketo con [!DNL Dynamics] {#required-fields-for-syncing-marketo-with-dynamics}

I campi *must* devono essere sincronizzati con Marketo sia per [!UICONTROL Lead] che per [!UICONTROL Contact] affinché [!DNL Sales Insight] funzioni:

* Priorità
* Urgenza
* Punteggio relativo

Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, archiviare l&#39;istanza per verificare che i campi siano sincronizzati sia per **[!UICONTROL Lead]** che per **[!UICONTROL Contact]**. In caso contrario, aggiungili.

Ecco come verificare e aggiungere campi di sincronizzazione.

1. Vai a [!UICONTROL Admin] e fai clic su **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fare clic su **[!UICONTROL Edit]** il [!UICONTROL Field Sync Details].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. In [!UICONTROL Lead], selezionare la casella di controllo [!UICONTROL Priority].

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Ora scorri verso il basso e seleziona la casella di controllo [!UICONTROL Urgency]...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. e la casella di controllo [!UICONTROL Relative Score].

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Quindi, selezionare le caselle di controllo per [!UICONTROL Priority], [!UICONTROL Urgency] e [!UICONTROL Relative Score] per [!UICONTROL Contact].

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Prima di verificare di aver risolto il problema, attendi almeno 10 minuti per l’esecuzione di una sincronizzazione.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
