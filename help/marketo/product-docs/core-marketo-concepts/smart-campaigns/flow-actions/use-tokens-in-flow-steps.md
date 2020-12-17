---
unique-page-id: 1146995
description: Utilizzare i token nei passaggi di flusso - Documenti Marketo - Documentazione prodotto
title: Utilizzare i token nei passaggi di flusso
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# Utilizzare i token nei passaggi di flusso {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>* [Aggiunta di un passaggio di flusso a una campagna intelligente](add-a-flow-step-to-a-smart-campaign.md)


Un token è una variabile. Lo si utilizza nelle [e-mail](https://docs.marketo.com/pages/viewpage.action?pageId=557076), [pagine di destinazione](https://docs.marketo.com/pages/viewpage.action?pageId=2359689) e nelle [campagne intelligenti](https://docs.marketo.com/display/DOCS/Smart+Lists+and+Lists) per semplificare la vita. È possibile utilizzare [My Tokens](../../../../product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (token personalizzati) in passaggi di flusso, webhooks, e-mail e pagine di destinazione.  È possibile utilizzare i token per includere il contenuto variabile nei seguenti passaggi di flusso:

* Modifica valore dati
* Momento interessante
* Passaggi campagna Salesforce (aggiungere, rimuovere, modificare lo stato)
* Crea attività
* Invia avviso (solo nelle campagne di attivazione)

>[!NOTE]
>
>**Disponibilità**
>
>Non tutti i clienti hanno acquistato questa funzionalità. Per informazioni, contattate il rappresentante commerciale.

1. Nella fase di flusso, iniziate a digitare `{{` per ottenere le categorie di token. ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >**Tubo profondo**
   >
   >Per un elenco dei diversi token disponibili, consultare [Panoramica token](../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md).

1. Continuate a digitare fino a trovare il token desiderato e fate clic per selezionarlo.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Più token possono essere utilizzati nei passaggi del flusso Momento interessante, Crea attività e Invia avviso.

   >[!NOTE]
   >
   >**Articoli correlati**
   >
   >* [Gestione dei token personali](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Informazioni sui token personali in un programma](../../../../product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)


Fantastico! I dati verranno estratti dal token quando viene eseguita la campagna intelligente.