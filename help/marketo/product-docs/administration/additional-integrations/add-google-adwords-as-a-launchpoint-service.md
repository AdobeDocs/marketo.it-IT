---
unique-page-id: 6095008
description: Aggiungere Google AdWords as a LaunchPoint Service - Marketo Docs - Documentazione del prodotto
title: Aggiungere Google AdWords come servizio LaunchPoint
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Aggiungere Google AdWords as a LaunchPoint Service {#add-google-adwords-as-a-launchpoint-service}

Collega il tuo account Google AdWords a Marketo per caricare automaticamente i dati di conversione offline da Marketo a Google AdWords. Quindi, dall&#39;interfaccia utente di AdWords, potrai vedere facilmente quali clic hanno portato a lead qualificati, opportunità e nuovi clienti (o qualsiasi fase di ricavo desideri monitorare) dopo aver [aggiunto colonne personalizzate](https://support.google.com/adwords/answer/3073556) in AdWords. Queste informazioni non vengono visualizzate nell’interfaccia utente di Marketo.

Ulteriori informazioni sulla [funzionalità di importazione delle conversioni offline di Google](https://support.google.com/adwords/answer/2998031?hl=en).

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>È inoltre possibile integrare un servizio [Google AdWords as a Launchpoint con un account manager](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md).

1. Vai alla sezione **Amministratore** .

   ![](assets/login-admin.png)

1. Seleziona **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Selezionare **Nuovo** e **Nuovo servizio**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Immetti un nome visualizzato e seleziona **Google AdWords**.

   ![](assets/new-service-google.png)

1. Seleziona **Autorizza Marketo**.

   >[!NOTE]
   >
   >Assicurati di disconnetterti dal tuo account Gmail personale e di abilitare i pop-up.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Seleziona il tuo account associato a Google AdWords.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Selezionare **Accept**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. Lo stato viene visualizzato come **Success**. Selezionare **Avanti**.

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Carica le conversioni offline da Marketo a Google AdWords **Settimanale** o **Giornaliero**.

   ![](assets/image2015-2-23-16-3a53-3a4.png)

1. Conversione degli attributi in **Primo clic** o **Ultimo clic**.

   | Tipo | Definizione |
   |---|---|
   | Primo clic | Le conversioni offline saranno attribuite ai primi AdWords e che una persona ha fatto clic negli ultimi 90 giorni |
   | Ultimo clic | Le conversioni offline saranno attribuite alle ultime AdWords e una persona ha fatto clic su di esse |

   >[!NOTE]
   >
   >L’utilizzo di un modello di attribuzione coerente in Marketo e AdWords fornisce i dati più precisi.

   ![](assets/image2015-2-23-16-3a57-3a49.png)

1. Fare clic su **Crea**.

   ![](assets/image2015-2-23-17-3a50-3a9.png)

   >[!NOTE]
   >
   >[Per il corretto funzionamento di questa funzione, è necessario selezionare ](https://support.google.com/adwords/answer/1752125?hl=en) l’opzione di assegnazione tag automatica. La disattivazione deve essere eseguita in AdWords.

Fantastico! Ora consulta l’articolo correlato di seguito per scoprire come mappare le conversioni offline di AdWords nel modello di ricavi.

>[!MORELIKETHIS]
>
>[Impostare le conversioni di Google AdWords nel modello dei ricavi](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md)
