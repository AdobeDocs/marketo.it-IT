---
unique-page-id: 42762519
description: Configurazione per i clienti esistenti - Documenti Marketo - Documentazione prodotto
title: Configurazione per clienti esistenti
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# Configurazione per clienti esistenti {#configuration-for-existing-customers}

Configurate la seguente configurazione per iniziare a utilizzare il nuovo dashboard di Insights.

>[!NOTE]
>
>**Prerequisiti**
>
>Accertati di aver aggiornato il pacchetto Salesforce alla versione più recente

## Configurare Sales Insight in Marketo {#configure-sales-insight-in-marketo}

1. Apri una nuova scheda nel browser per ottenere le credenziali Informazioni sulle vendite marketing dal tuo account Marketo.
1. Andate all&#39;area **Admin** .

   ![](assets/configure-1.png)

1. Fare clic su **Vendite**.

   ![](assets/configure-2.png)

1. Fate clic su **Visualizza** per compilare le credenziali API Rest.

   ![](assets/configure-3.png)

1. Vedrete un pop-up di conferma. Fate clic su **OK**.

## Configurare l&#39;analisi delle vendite in Salesforce {#configure-sales-insight-in-salesforce}

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/sfdc-1.png)

1. Cercare e selezionare Impostazioni **sito** remoto.

   ![](assets/sfdc-2.png)

1. Fate clic su **Nuovo sito** remoto.

   ![](assets/sfdc-3.png)

1. Immettete il nome del sito remoto (può essere simile a &quot;MarketoRestAPI&quot;) e l’URL del sito remoto (l’URL API dal pannello Configurazione API Rest in Marketo).

   ![](assets/sfdc-4.png)

1. Fate clic su **Salva**.

   ![](assets/sfdc-5.png)

   È stata creata l&#39;impostazione del sito remoto per l&#39;API Rest.

## Accesso al punto vendita di Marketo {#access-marketo-sales-insight}

1. Copia le credenziali dal pannello Rest API nella pagina Admin di Marketing’s Sales Insight. Incollateli nella sezione Rest API della pagina Sales Insight Configuration di Salesforce.
1. Immettete la chiave segreta API.

   ![](assets/config.png)

