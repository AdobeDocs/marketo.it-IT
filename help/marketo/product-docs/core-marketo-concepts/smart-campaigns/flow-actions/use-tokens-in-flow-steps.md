---
unique-page-id: 1146995
description: Utilizzare i token nei passaggi del flusso - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzare i token nei passaggi del flusso
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Utilizzare i token nei passaggi del flusso {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

Un token è una variabile. Puoi utilizzarlo nelle e-mail, nelle pagine di destinazione e nelle campagne intelligenti per semplificare il lavoro. È possibile utilizzare [I miei token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (token personalizzati) nei passaggi del flusso, nei webhook, nelle e-mail e nelle pagine di destinazione. Puoi utilizzare i token per includere il contenuto delle variabili nei seguenti passaggi del flusso:

* Modifica valore dati
* Modifica dati membro programma
* Momento di interesse
* Passaggi della campagna Salesforce (aggiungere, rimuovere, modificare lo stato)
* Crea attività
* Invia avviso (solo nelle campagne trigger)

1. Nel passaggio del flusso, inizia a digitare `{{` per ottenere le categorie dei token.

   ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >Estrai [Panoramica dei token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) per un elenco di diversi token disponibili.

1. Continua a digitare finché non trovi il token desiderato e fai clic per selezionarlo.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >È possibile utilizzare più token nei passaggi Momento di interesse, Crea attività e Invia avviso.

   >[!NOTE]
   >
   >I token di campo personalizzati dei membri del programma possono essere utilizzati in: Crea attività, Crea attività in Microsoft, Momenti di interesse, Azioni del flusso Modifica valore dati e Webhook.

   Fantastico! I dati verranno estratti dal token quando viene eseguita la campagna avanzata.

   >[!MORELIKETHIS]
   >
   >* [Gestione dei token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Informazioni sui token in un programma](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)
