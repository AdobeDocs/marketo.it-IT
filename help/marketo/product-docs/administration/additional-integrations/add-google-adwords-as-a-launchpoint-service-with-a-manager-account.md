---
unique-page-id: 7504893
description: Aggiungere Google AdWords as a Launchpoint Service con un account manager - Marketo Docs - Documentazione del prodotto
title: Aggiungere Google AdWords as a Launchpoint Service con un account Manager
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
source-git-commit: ab8eb044b89c925accc3b6a4ac4def53e3927321
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Aggiungere Google AdWords as a Launchpoint Service con un account Manager {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Collega il tuo account Google AdWords a Marketo per caricare automaticamente i dati di conversione offline da Marketo a Google AdWords. Quindi, dall’interfaccia utente di AdWords, potrai vedere facilmente quali clic hanno portato a lead qualificati, opportunità e nuovi clienti (o qualsiasi fase di ricavo desideri monitorare) dopo aver  [aggiungere colonne personalizzate](https://support.google.com/adwords/answer/3073556) in AdWords. Queste informazioni non vengono visualizzate nell’interfaccia utente di Marketo.

Se disponi di più account Google Adwords, puoi utilizzare un [Account Google AdWords Manager](https://www.google.com/adwords/manager-accounts/) (precedentemente noto come Centro client personale) per integrarli con Marketo.

Ulteriori informazioni [Funzione di importazione della conversione offline di Google](https://support.google.com/adwords/answer/2998031?hl=en).

>[!AVAILABILITY]
>
>Non tutti i clienti hanno acquistato questa funzione. Contatta il tuo Customer Success Manager per i dettagli.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>È inoltre possibile integrare un [account Google AdWords autonomo come servizio Launchpoint](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md).

1. Vai a **Amministratore** sezione .

   ![](assets/login-admin-1.png)

1. Seleziona **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Seleziona **Nuovo** e **Nuovo servizio**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Immettere un nome visualizzato e selezionare **Google AdWords**.

   ![](assets/new-service-google-1.png)

1. Seleziona **Autorizzare Marketo**.

   >[!NOTE]
   >
   >Assicurati di disconnetterti dal tuo account Gmail personale e di abilitare i pop-up.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Seleziona l&#39;account associato a **Google AdWords**.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Seleziona **Accetta**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. Lo stato verrà visualizzato come **Completato**. Seleziona **Successivo**.

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Carica le conversioni offline da Marketo a Google AdWords **Settimanale** o **Giornaliero**.

   ![](assets/image2015-3-27-14-3a7-3a45.png)

1. Conversione degli attributi in **Primo clic** o **Ultimo clic**.

   | Tipo | Definizione |
   |---|---|
   | Primo clic | Le conversioni offline saranno attribuite ai primi AdWords e che una persona ha fatto clic negli ultimi 90 giorni |
   | Ultimo clic | Le conversioni offline saranno attribuite alle ultime AdWords e una persona ha fatto clic su di esse |

   ![](assets/image2015-3-27-14-3a10-3a46.png)

   >[!NOTE]
   >
   >[Assegnazione tag automatica](https://support.google.com/adwords/answer/1752125?hl=en) deve essere selezionato per il funzionamento di questa funzione. Deve essere attivato in AdWords.

1. Fai clic su **Successivo**.

   ![](assets/image2015-3-27-14-3a11-3a31.png)

1. Deselezionare gli account che non si desidera aggiornare. Fai clic su **Crea**.

   ![](assets/image2015-3-27-14-3a12-3a51.png)

   Ora consulta l’articolo correlato di seguito per scoprire come mappare le conversioni offline di AdWords nel modello di ricavi.

   >[!MORELIKETHIS]
   >
   >[Impostare le conversioni Google AdWords nel modello dei ricavi con un account manager](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md)
