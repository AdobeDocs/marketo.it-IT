---
unique-page-id: 30082174
description: Momenti di interesse in Sales Connect - Documentazione Marketo - Documentazione del prodotto
title: Momenti di interesse in Sales Connect
exl-id: 210f31d1-606a-479d-8a2b-351b2b1a7678
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Momenti di interesse in [!DNL Sales Connect] {#interesting-moments-in-sales-connect}

Momenti interessanti sono la chiave per comunicare con il tuo team di vendita tramite [!DNL Marketo Sales Connect].

>[!AVAILABILITY]
>
>Sono disponibili solo per [i clienti Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/using-interesting-moments.md) e [!DNL Marketo Sales Connect].

>[!PREREQUISITES]
>
>* È necessario disporre di una connessione [a Salesforce CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md){target="_blank"}
>* Devi essere il lead o il proprietario del contatto in Salesforce
>* Devi avere accesso a [concedere l&#39;accesso alla connessione Marketo Engage](/help/marketo/product-docs/marketo-sales-connect/marketo/granting-access-to-users.md){target="_blank"}

## Qual è un momento interessante? {#what-is-an-interesting-moment}

Sta a te decidere! Decidi quali informazioni sono rilevanti per il tuo team di vendita. Il tuo team di vendita potrebbe voler sapere quando un lead:

* Visita la pagina dei prezzi sul sito Web
* Fa clic su un collegamento in un messaggio e-mail di annuncio di un nuovo prodotto.
* Richiede una demo del prodotto

## Come posso creare un momento interessante? {#how-do-i-create-an-interesting-moment}

1. Scegli una [campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), preferibilmente una che il tuo team di vendita troverebbe interessante se venisse attivata.

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. Trascinare sul passaggio del flusso **[!UICONTROL Interesting Moments]**.

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. Selezionare un tipo **type** ([!UICONTROL Email], [!UICONTROL Milestone] o [!UICONTROL Web]).

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. Scrivi un messaggio al tuo team vendite nel campo **[!UICONTROL Description]** che spiega perché questa azione è importante.

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >Marketo aggiungerà anche la data in cui si è verificato e come è stato aggiunto il momento interessante (ad esempio azione lead > passaggio di flusso, API SOAP).

## Come appare un momento interessante in Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

I momenti interessanti verranno visualizzati nel registro attività di un [lead](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/image2015-1-14-18-3a45-3a58.png)

## Come si presenta un momento di interesse in [!DNL Sales Connect]? {#what-does-an-interesting-moment-look-like-in-sales-connect}

I Momenti di interesse vengono visualizzati in tempo reale nel feed live di un utente. Utilizziamo l&#39;ID proprietario del lead in [!DNL Salesforce] per mostrare ai nostri utenti i momenti interessanti dei lead rilevanti di cui sono proprietari. Gli utenti possono seguire rapidamente i lead tramite e-mail/telefono/campagna di vendita facendo clic sull’elenco a discesa accanto al nome del lead.

![](assets/engagement.jpg)
