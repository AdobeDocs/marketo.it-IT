---
unique-page-id: 42762519
description: Configurazione per i clienti esistenti - Documenti Marketo - Documentazione del prodotto
title: Configurazione per i clienti esistenti
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
source-git-commit: 0701121597f33580ada09fe975c1740cb55f945d
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Configurazione per i clienti esistenti {#configuration-for-existing-customers}

Imposta la seguente configurazione per iniziare a utilizzare il nuovo dashboard Approfondimenti .

>[!PREREQUISITES]
>
>Assicurati di aver aggiornato il pacchetto Salesforce alla versione più recente

## Configurare la funzione Approfondimenti vendite in Marketo {#configure-sales-insight-in-marketo}

1. Apri una nuova scheda nel browser per ottenere le credenziali Marketo Sales Insights dal tuo account Marketo.

1. Vai a **Amministratore** area.

   ![](assets/configuration-for-existing-customers-1.png)

1. Fai clic su **Approfondimenti vendite**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Fai clic su **Visualizza** per popolare le credenziali API Rest.

   ![](assets/configuration-for-existing-customers-3.png)

1. Verrà visualizzato un pop-up di conferma. Fai clic su **OK**.

## Configurazione di Sales Insight in Salesforce {#configure-sales-insight-in-salesforce}

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Cerca e seleziona **Impostazioni del sito remoto**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Fai clic su **Nuovo sito remoto**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Inserisci il Nome del sito remoto (può essere simile a &quot;MarketoRestAPI&quot;) e l’URL del sito remoto (l’URL API dal pannello Configurazione API Rest in Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Fai clic su **Salva**.

   ![](assets/configuration-for-existing-customers-8.png)

   È stata ora creata l’impostazione del sito remoto per l’API Rest.

## Accedere a Marketo Sales Insight {#access-marketo-sales-insight}

1. Copia le credenziali dal pannello Rest API nella pagina Sales Insight Admin di Marketo. Incollali nella sezione Rest API della pagina Sales Insight Configuration di Salesforce.

1. Immetti la chiave segreto API.

   ![](assets/configuration-for-existing-customers-9.png)
