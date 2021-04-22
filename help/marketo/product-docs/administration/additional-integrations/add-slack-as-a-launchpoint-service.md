---
unique-page-id: 12983619
description: Aggiungere Slack as a LaunchPoint Service - Documenti Marketo - Documentazione del prodotto
title: Aggiungere Slack come servizio LaunchPoint
exl-id: 38c1501d-27ac-4c6c-967d-4decd10e0cb3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Aggiungere Slack come servizio LaunchPoint {#add-slack-as-a-launchpoint-service}

Nell’integrazione dello Slack sono inclusi due tipi di notifica:

* **Notifiche** di sistema: Ottieni notifiche di Slack relative a eventi importanti nella tua istanza Marketo, come avvisi sugli stati della campagna corrente e su qualsiasi problema che richieda un’attenzione immediata (errori CRM e limiti API).
* **Momenti** interessanti: Quando Marketo Insight viene attivato da un individuo noto da un account di vendita, i proprietari lead possono essere informati tramite Slack. Le notifiche includono informazioni sui lead e dettagli sull’account di vendita.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!PREREQUISITES]
>
>Se non hai già abilitato le notifiche di sistema di Slack, contatta il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Vai a **LaunchPoint**, quindi in **Nuovo** fai clic su **Nuovo servizio**.

   ![](assets/image2017-11-27-14-3a13-3a18.png)

1. Immettere un nome visualizzato per l&#39;integrazione dello Slack. Nel menu a discesa **Servizio**, selezionare **Slack**. Fare clic su **Crea**.

   ![](assets/image2017-11-27-15-3a54-3a11.png)

1. Fare clic su **Autorizza**. Viene aperto uno Slack in una nuova scheda, in cui si completa l’autorizzazione e si concede a Marketo l’autorizzazione per estrarre informazioni dallo Slack.

   ![](assets/image2017-11-27-14-3a16-3a6.png)

1. Nella nuova scheda Slack, immetti l’URL dell’area di lavoro e fai clic su **Continua**.

   ![](assets/image2017-11-27-15-3a1-3a29.png)

1. Immetti le credenziali di Slack e fai clic su **Accedi**.

   ![](assets/image2017-11-27-15-3a1-3a3.png)

1. Nel menu a discesa **Post to** , seleziona il canale in cui vuoi inviare le notifiche da Marketo. Rivedi le autorizzazioni richieste, quindi fai clic su **Autorizza**.

   ![](assets/image2018-1-9-13-3a21-3a50.png)

1. Dovresti vedere la schermata di conferma qui sotto. La scheda si chiude automaticamente.

   ![](assets/image2017-11-27-15-3a51-3a57.png)

1. Aggiorna la scheda Marketo e conferma che lo Slack sia ora elencato come servizio attivo in LaunchPoint.

   ![](assets/image2017-11-27-15-3a55-3a37.png)

   Le notifiche inizieranno a essere inviate al canale selezionato al passaggio 6. Avranno un aspetto simile a questo:

   ![](assets/samplenotification.png)
