---
unique-page-id: 1146995
description: Utilizzare i token nei passaggi del flusso - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzare i token nei passaggi del flusso
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 2%

---

# Utilizzare i token nei passaggi del flusso {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Un token è una variabile. Puoi utilizzarlo nelle e-mail, nelle pagine di destinazione e nelle campagne intelligenti per semplificare il lavoro. Puoi utilizzare [I miei token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"} (token personalizzati) nei passaggi del flusso, nei webhook, nelle e-mail e nelle pagine di destinazione. Puoi utilizzare i token per includere il contenuto delle variabili nei seguenti passaggi del flusso:

* Modifica valore dati
* Modifica dati membro programma
* Momento interessante
* [!DNL Salesforce] passaggi della campagna (aggiungere, rimuovere, modificare lo stato)
* Crea attività
* Invia avviso (solo in Campagne con trigger)

1. Nel passaggio del flusso, inizia a digitare `{{` per ottenere le categorie di token.

   ![](assets/use-tokens-in-flow-steps-1.png)

   >[!NOTE]
   >
   >Consulta [Panoramica dei token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} per un elenco di diversi token disponibili.

1. Continua a digitare finché non trovi il token desiderato e fai clic per selezionarlo.

   ![](assets/use-tokens-in-flow-steps-2.png)

   >[!TIP]
   >
   >È possibile utilizzare più token nei passaggi Momento di interesse, Crea attività e Invia avviso.

   >[!NOTE]
   >
   >I token di campo personalizzati dei membri del programma possono essere utilizzati in: Crea attività, Crea attività in Microsoft, Momenti di interesse, Azioni del flusso Modifica valore dati e Webhook.

   Fantastico! I dati verranno estratti dal token quando viene eseguita la campagna avanzata.

   >[!MORELIKETHIS]
   >
   >* [Gestione dei token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
   >* [Informazioni sui token in un programma](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"}
