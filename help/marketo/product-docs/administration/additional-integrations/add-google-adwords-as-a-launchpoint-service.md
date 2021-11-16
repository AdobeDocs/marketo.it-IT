---
unique-page-id: 6095008
description: Aggiungere Google AdWords as a LaunchPoint Service - Documentazione Marketo - Documentazione del prodotto
title: Aggiungere Google AdWords as a LaunchPoint Service
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
source-git-commit: ab8eb044b89c925accc3b6a4ac4def53e3927321
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Aggiungere Google AdWords as a LaunchPoint Service {#add-google-adwords-as-a-launchpoint-service}

Collega il tuo account Google AdWords a Marketo per caricare automaticamente i dati di conversione offline da Marketo a Google AdWords. Quindi, dall’interfaccia utente di AdWords, potrai vedere facilmente quali clic hanno generato lead qualificati, opportunità e nuovi clienti (o qualsiasi fase di ricavo desideri monitorare) dopo aver [aggiungere colonne personalizzate](https://support.google.com/adwords/answer/3073556) in AdWords. Queste informazioni non vengono visualizzate nell’interfaccia utente di Marketo.

Ulteriori informazioni [Funzione di importazione della conversione offline di Google](https://support.google.com/adwords/answer/2998031?hl=en).

>[!AVAILABILITY]
>
>Non tutti i clienti hanno acquistato questa funzione. Contatta il tuo Customer Success Manager per i dettagli.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>È inoltre possibile integrare un [Servizio Google AdWords as a Launchpoint con un account manager](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md).

1. Vai a **Amministratore** sezione .

   ![](assets/login-admin.png)

1. Seleziona **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Seleziona **Nuovo** e **Nuovo servizio**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Immettere un nome visualizzato e selezionare **Google AdWords**.

   ![](assets/new-service-google.png)

1. Seleziona **Autorizzare Marketo**.

   >[!NOTE]
   >
   >Assicurati di disconnetterti dal tuo account Gmail personale e di abilitare i pop-up.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Seleziona il tuo account associato a Google AdWords.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Seleziona **Accetta**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. Lo stato verrà visualizzato come **Completato**. Seleziona **Successivo**.

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

1. Fai clic su **Crea**.

   ![](assets/image2015-2-23-17-3a50-3a9.png)

   >[!NOTE]
   >
   >[Assegnazione tag automatica](https://support.google.com/adwords/answer/1752125?hl=en) deve essere selezionato per il funzionamento di questa funzione. La disattivazione deve essere eseguita in AdWords.

Fantastico! Ora consulta l’articolo correlato di seguito per scoprire come mappare le conversioni offline di AdWords nel modello di ricavi.

>[!MORELIKETHIS]
>
>[Impostare le conversioni Google AdWords nel modello di ricavi](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md)
