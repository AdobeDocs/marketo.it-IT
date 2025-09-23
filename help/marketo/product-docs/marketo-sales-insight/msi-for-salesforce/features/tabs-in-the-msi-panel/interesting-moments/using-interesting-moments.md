---
unique-page-id: 2951640
description: Utilizzo dei momenti di interesse - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo di momenti di interesse
exl-id: ccf7664b-08e1-490a-a3f9-5fa3bd8fb05f
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 1%

---

# Utilizzo di momenti di interesse {#using-interesting-moments}

I momenti interessanti sono la chiave per comunicare con il tuo team di vendita tramite l&#39;app [!DNL Marketo Sales Insight].

>[!AVAILABILITY]
>
>Sono disponibili solo per [!DNL Marketo Sales Insight] e [[!DNL Marketo Sales Connect]](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-sales-connect.md) clienti.

## Qual è un momento interessante? {#what-is-an-interesting-moment}

Sta a te decidere! Decidi quali informazioni sono rilevanti per il tuo team di vendita. Il tuo team di vendita potrebbe voler sapere quando un lead:

* Visita la pagina dei prezzi sul sito Web
* Fa clic su un collegamento in un messaggio e-mail di annuncio di un nuovo prodotto.
* Richiede una demo del prodotto

## Come posso creare un momento interessante?  {#how-do-i-create-an-interesting-moment}

1. Scegli una [campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), preferibilmente una che il tuo team di vendita troverebbe interessante se venisse attivata.

   ![](assets/using-interesting-moments-1.png)

1. Trascinare sul passaggio del flusso **[!UICONTROL Interesting Moments]**.

   ![](assets/using-interesting-moments-2.png)

1. Selezionare un tipo **type** ([!UICONTROL Email], [!UICONTROL Milestone] o [!UICONTROL Web]).

   ![](assets/using-interesting-moments-3.png)

1. Scrivi un messaggio al tuo team vendite nel campo **[!UICONTROL Description]** che spiega perché questa azione è importante.

   ![](assets/using-interesting-moments-4.png)

   >[!NOTE]
   >
   >Marketo aggiungerà anche la data in cui si è verificato e come è stato aggiunto il momento interessante (ad esempio azione lead > passaggio di flusso, API SOAP).

## Come può diventare ancora più interessante?  {#how-can-this-get-even-more-interesting}

Token! Aggiungili nel campo di descrizione per fornire al team di vendita informazioni più specifiche, ad esempio l’oggetto dell’e-mail aperta dal lead o chi l’ha inviata. Scopri quali token sono disponibili per l&#39;utilizzo nel glossario [Token per i momenti di interesse](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md).

>[!TIP]
>
>Inizia con cinque momenti interessanti, quindi collabora con il tuo team di vendita per determinare quali informazioni sono interessati a vedere.

## Come appare un momento interessante in Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

I momenti interessanti verranno visualizzati nel registro attività di un [lead](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/using-interesting-moments-5.png)

## Come si presenta un momento di interesse in [!DNL Salesforce]?  {#what-does-an-interesting-moment-look-like-in-salesforce}

Dopo aver [installato l&#39;app [!DNL Marketo Sales Insight] App](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md), i momenti interessanti verranno visualizzati nelle pagine lead, contatto, account o opportunità. Vengono inoltre visualizzati nel dashboard [!DNL Sales Insight] nei feed lead, [!DNL Best Bets] e nell&#39;elenco di controllo.

![](assets/using-interesting-moments-6.png)

## Come si presenta un momento di interesse in [!DNL Salesforce1]? {#what-does-an-interesting-moment-look-like-in-salesforce-1}

Dopo aver installato o aggiornato [!DNL Marketo Sales Insight] per [!DNL Salesforce1], i momenti interessanti verranno visualizzati nei collegamenti correlati del lead.

![](assets/using-interesting-moments-7.png)

## Iscriviti ai momenti di interesse {#subscribe-to-interesting-moments}

È possibile sottoscrivere un momento di interesse facendo clic sul pulsante [!UICONTROL Subscribe] nella scheda Momento di interesse o nel feed lead. I passaggi seguenti sono gli stessi per entrambi.

1. Fai clic sull’icona Sottoscrivi. Passerai quindi alla scheda Iscrizione e-mail.

1. È possibile scegliere il tipo di avviso e-mail da ricevere in base a [!UICONTROL Name], [!UICONTROL Account], [!UICONTROL Type] o [!UICONTROL Description].

1. Scegli gli indirizzi e-mail a cui inviare gli avvisi (te stesso/i membri del gruppo)

1. Fai clic su **[!UICONTROL Subscribe]**.

>[!NOTE]
>
>Con l’abbonamento a Tipi di momento di interesse o Descrizioni, l’utente riceverà notifiche e-mail per le persone (lead/contatti) di cui è proprietario quando attiva un Momento di interesse che corrisponde a quel Tipo o Descrizione.

![](assets/using-interesting-moments-8.png)
