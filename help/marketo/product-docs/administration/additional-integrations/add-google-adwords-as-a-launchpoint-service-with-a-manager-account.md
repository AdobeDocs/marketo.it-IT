---
unique-page-id: 7504893
description: "Aggiungi [!DNL Google AdWords] as a [!DNL Launchpoint] Service con un account Manager - Documentazione di Marketo - Documentazione del prodotto"
title: "Aggiungi [!DNL Google AdWords] as a [!DNL Launchpoint] Service con un account Manager"
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
feature: Administration, Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Aggiungi [!DNL Google AdWords] come servizio [!DNL Launchpoint] con un account Manager {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Collega l&#39;account [!DNL Google AdWords] a Marketo per caricare automaticamente i dati di conversione offline da Marketo a [!DNL Google AdWords]. Dall&#39;interfaccia utente di [!DNL AdWords], potrai vedere facilmente quali clic hanno generato lead qualificati, opportunità e nuovi clienti (o qualsiasi fase di ricavi desideri monitorare) dopo [aver aggiunto colonne personalizzate](https://support.google.com/adwords/answer/3073556){target="_blank"} in [!DNL AdWords]. Queste informazioni non vengono visualizzate nell’interfaccia utente di Marketo.

Se si dispone di più account [!DNL Google Adwords], è possibile utilizzare un account [[!DNL Google AdWords Manager Account]](https://www.google.com/adwords/manager-accounts/){target="_blank"} (precedentemente noto come [!DNL My Client Center]) per integrarli con Marketo.

Ulteriori informazioni sulla [funzionalità di importazione della conversione offline di Google](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Non tutti gli utenti del Marketo Engage hanno acquistato questa funzionalità. Per ulteriori informazioni, contatta l’Adobe Account Team (il tuo Account Manager).

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>È inoltre possibile integrare un account [autonomo [!DNL Google AdWords] come  [!DNL Launchpoint] servizio](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"}.

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. Selezionare **[!UICONTROL LaunchPoint]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. Fai clic sul menu a discesa **[!UICONTROL Nuovo]** e seleziona **[!UICONTROL Nuovo servizio]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. Immetti un **[!UICONTROL Nome visualizzato]** e seleziona **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. Selezionare **[!UICONTROL Autorizza Marketo]**.

   >[!NOTE]
   >
   >Assicurarsi di disconnettersi dall&#39;account [!DNL Gmail] personale e abilitare i popup.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. Seleziona il tuo account associato a **[!DNL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. Fare clic su **[!UICONTROL Accetta]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. Lo stato verrà visualizzato come **[!UICONTROL Operazione completata]**. Seleziona **[!UICONTROL Avanti]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. Carica le conversioni offline da Marketo a [!DNL Google AdWords] **[!UICONTROL Ogni settimana]** o **[!UICONTROL Ogni giorno]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. Conversione dell&#39;attributo in **[!UICONTROL Primo clic]** o **[!UICONTROL Ultimo clic]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | Tipo | Definizione |
   |---|---|
   | [!UICONTROL Primo clic] | Le conversioni offline saranno attribuite al primo [!DNL AdWords] e a una persona che ha fatto clic negli ultimi 90 giorni |
   | [!UICONTROL Ultimo clic] | Le conversioni offline saranno attribuite all&#39;ultimo [!DNL AdWords] e che una persona ha fatto clic |

   >[!NOTE]
   >
   >È necessario selezionare [Auto-tagging](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} affinché questa funzione funzioni. Deve essere attivato in [!DNL AdWords].

1. Fai clic su **[!UICONTROL Avanti]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. Deseleziona gli account da non aggiornare. Fai clic su **[!UICONTROL Crea]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   Ora consulta l&#39;articolo correlato seguente per informazioni su come mappare [!DNL AdWords] conversioni offline nel modello di ricavo.

   >[!MORELIKETHIS]
   >
   >[Imposta [!DNL Google AdWords] Conversioni nel modello di ricavi con un account Manager](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target="_blank"}
