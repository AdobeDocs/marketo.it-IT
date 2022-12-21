---
unique-page-id: 1146995
description: Utilizzare i token nei passaggi del flusso - Documenti Marketo - Documentazione del prodotto
title: Utilizzare i token nei passaggi del flusso
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Utilizzare i token nei passaggi del flusso {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

Un token è una variabile. Puoi utilizzarlo nelle e-mail, nelle pagine di destinazione e nelle campagne intelligenti per semplificare la tua vita. È possibile utilizzare [Token personali](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (token personalizzati) in passaggi di flusso, webhook, e-mail e pagine di destinazione. Puoi utilizzare i token per includere il contenuto variabile nei passaggi del flusso seguenti:

* Modifica valore dati
* Modifica dati dei membri del programma
* Momento interessante
* Passaggi della campagna Salesforce (aggiungi, rimuovi, cambia stato)
* Crea attività
* Invia avviso (solo nelle campagne di attivazione)

1. Nel passaggio del flusso, inizia a digitare `{{` per ottenere categorie di token.

   ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >Consulta [Panoramica dei token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) per un elenco dei diversi token disponibili.

1. Continua a digitare fino a trovare il token desiderato e fai clic su per selezionare.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >È possibile utilizzare più token nei passaggi del flusso di avvisi relativi a Momento interessante, Crea attività e Invia avviso.

   >[!NOTE]
   >
   >I token di campo personalizzati dei membri del programma possono essere utilizzati in: Crea attività, Crea attività in Microsoft, Momenti interessanti, Modifica azioni di flusso di valore dei dati e Webhook.

   Calmo! I dati verranno estratti dal token quando la campagna avanzata viene eseguita.

   >[!MORELIKETHIS]
   >
   >* [Gestione dei token personali](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Informazioni sui token personali in un programma](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)

