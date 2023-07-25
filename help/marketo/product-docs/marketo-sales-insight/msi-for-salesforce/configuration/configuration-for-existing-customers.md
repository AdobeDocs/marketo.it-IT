---
unique-page-id: 42762519
description: Configurazione per clienti esistenti - Documentazione di Marketo - Documentazione del prodotto
title: Configurazione per clienti esistenti
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Configurazione per clienti esistenti {#configuration-for-existing-customers}

Imposta la seguente configurazione per iniziare a utilizzare la nuova dashboard di Insights.

>[!PREREQUISITES]
>
>Assicurati di aver aggiornato il pacchetto Salesforce all’ultima versione

## Configurare Sales Insight in Marketo {#configure-sales-insight-in-marketo}

1. Apri una nuova scheda nel browser per ottenere le credenziali di Marketo Sales Insights dal tuo account Marketo.

1. Vai a **Amministratore** area.

   ![](assets/configuration-for-existing-customers-1.png)

1. Clic **Insight sulle vendite**.

   ![](assets/configuration-for-existing-customers-2.png)

1. Clic **Visualizza** per popolare le credenziali API Rest.

   ![](assets/configuration-for-existing-customers-3.png)

1. Viene visualizzata una finestra a comparsa di conferma. Clic **OK**.

## Configurare Sales Insight in Salesforce {#configure-sales-insight-in-salesforce}

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/configuration-for-existing-customers-4.png)

1. Cerca e seleziona **Impostazioni sito remoto**.

   ![](assets/configuration-for-existing-customers-5.png)

1. Clic **Nuovo sito remoto**.

   ![](assets/configuration-for-existing-customers-6.png)

1. Immetti il nome del sito remoto (può essere ad esempio &quot;MarketoRestAPI&quot;) e l’URL del sito remoto (l’URL API dal pannello Configurazione API REST in Marketo).

   ![](assets/configuration-for-existing-customers-7.png)

1. Clic **Salva**.

   ![](assets/configuration-for-existing-customers-8.png)

   Ora hai creato l’impostazione per il sito remoto per l’API Rest.

## Accedi a Marketo Sales Insight {#access-marketo-sales-insight}

1. Copia le credenziali dal pannello API Rest nella pagina di amministrazione di Sales Insight di Marketo. Incollali nella sezione API REST della pagina Configurazione approfondimenti vendite di Salesforce.

1. Immetti la chiave segreta API.

   ![](assets/configuration-for-existing-customers-9.png)
