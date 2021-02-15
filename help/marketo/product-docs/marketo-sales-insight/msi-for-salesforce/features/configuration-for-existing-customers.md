---
unique-page-id: 42762519
description: Configurazione per i clienti esistenti - Documenti Marketo - Documentazione prodotto
title: Configurazione per clienti esistenti
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---


# Configurazione per clienti esistenti {#configuration-for-existing-customers}

Configurate la seguente configurazione per iniziare a utilizzare il nuovo dashboard di Insights.

>[!PREREQUISITES]
>
>Accertati di aver aggiornato il pacchetto Salesforce alla versione più recente

## Configurare Sales Insight in Marketo {#configure-sales-insight-in-marketo}

1. Apri una nuova scheda nel browser per ottenere le credenziali Informazioni sulle vendite marketing dal tuo account Marketo.

1. Andate all&#39;area **Admin**.

   ![](assets/configure-1.png)

1. Fare clic su **Sales Insight**.

   ![](assets/configure-2.png)

1. Fare clic su **Visualizza** per compilare le credenziali API Rest.

   ![](assets/configure-3.png)

1. Vedrete un pop-up di conferma. Fare clic su **OK**.

## Configurare la funzione Sales Insight in Salesforce {#configure-sales-insight-in-salesforce}

1. In Salesforce, fare clic su **Setup**.

   ![](assets/sfdc-1.png)

1. Cercare e selezionare **Impostazioni del sito remoto**.

   ![](assets/sfdc-2.png)

1. Fare clic su **Nuovo sito remoto**.

   ![](assets/sfdc-3.png)

1. Immettete il nome del sito remoto (può essere simile a &quot;MarketoRestAPI&quot;) e l’URL del sito remoto (l’URL API dal pannello Configurazione API Rest in Marketo).

   ![](assets/sfdc-4.png)

1. Fare clic su **Salva**.

   ![](assets/sfdc-5.png)

   È stata creata l&#39;impostazione del sito remoto per l&#39;API Rest.

## Accesso al punto vendita marketing {#access-marketo-sales-insight}

1. Copia le credenziali dal pannello Rest API nella pagina Admin di Marketing’s Sales Insight. Incollateli nella sezione Rest API della pagina Sales Insight Configuration di Salesforce.

1. Immettete la chiave segreta API.

   ![](assets/config.png)
