---
unique-page-id: 2950524
description: Distribuzione di social network sul sito web - Documentazione di Marketo - Documentazione del prodotto
title: Distribuire social network sul sito web
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Distribuire social network sul sito web {#deploy-social-on-your-website}

Incorpora le app social nelle pagine non Marketo.

>[!AVAILABILITY]
>
>Per ulteriori informazioni, contatta il tuo rappresentante commerciale.

Puoi distribuire app di social network sul tuo sito web per coinvolgere il tuo pubblico e coinvolgere tutti nella conversazione più ampia sui social network. Quando le persone condividono le tue promozioni e i tuoi contenuti con i loro amici sui social network, generi più traffico sul tuo sito.

1. Seleziona un’app social approvata, ad esempio un video o un pulsante Social di YouTube.

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. Seleziona **Codice di incorporamento** dalle azioni eseguite nell’app social.

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. Copia il codice per l’intestazione della pagina del sito (`<head>`) e corpo (`<body>`).

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. Incolla il primo frammento di codice nell’intestazione della pagina del sito web.

   ![](assets/socialonsite-embedhead.png)

1. Incolla il secondo snippet di codice in ogni pagina, dove desideri che l’app social venga visualizzata nella pagina.

   ![](assets/socialonsite-embedwidget.png)

1. Se devi impostare le dimensioni dell&#39;app social su dimensioni specifiche nella pagina, aggiungi **outerHeight** e **outerWidth** al secondo frammento di codice. Ad esempio, puoi aggiungere `options='{"outerHeight":400, "outerWidth":600}'`, come in:

   ![](assets/socialonsite-resizewidget2.png)

   L’app social di Marketo ora aggiunge contenuti e interattività al sito web, invitando i fan, i visitatori e i clienti esistenti a parlare di te. Allo stesso tempo, aggiunge i dati del loro profilo al database e tiene traccia delle metriche di influenza social.

   >[!MORELIKETHIS]
   >
   >* [Pulsante Personalizza app social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [Imposta requisito condivisione social network](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Pubblicare pagine di destinazione in Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
