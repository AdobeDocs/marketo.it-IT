---
unique-page-id: 2950524
description: Distribuzione di social network sul sito web - Documentazione di Marketo - Documentazione del prodotto
title: Distribuire social network sul sito web
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Distribuire social network sul sito web {#deploy-social-on-your-website}

Incorpora le app social nelle pagine non Marketo.

>[!IMPORTANT]
>
>Il 31 luglio 2024 è iniziato il processo di rimozione di questa funzione. Non è più possibile creare nuove risorse. Le risorse esistenti continueranno a funzionare fino al 31 gennaio 2025. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>Non tutti gli utenti del Marketo Engage hanno acquistato questa funzionalità. Per ulteriori informazioni, contatta l’Adobe Account Team (il tuo Account Manager).

Puoi distribuire app di social network sul tuo sito web per coinvolgere il tuo pubblico e coinvolgere tutti nella conversazione più ampia sui social network. Quando le persone condividono le tue promozioni e i tuoi contenuti con i loro amici sui social network, generi più traffico sul tuo sito.

1. Seleziona un’app social approvata, ad esempio un video o un pulsante Social di YouTube.

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. Seleziona **Codice da incorporare** dalle azioni delle app social.

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. Copiare il codice per l&#39;intestazione (`<head>`) e il corpo della pagina del sito (`<body>`).

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. Incolla il primo frammento di codice nell’intestazione della pagina del sito web.

   ![](assets/socialonsite-embedhead.png)

1. Incolla il secondo snippet di codice in ogni pagina, dove desideri che l’app social venga visualizzata nella pagina.

   ![](assets/socialonsite-embedwidget.png)

1. Se devi impostare la dimensione dell&#39;app social su dimensioni specifiche nella pagina, aggiungi le opzioni **outerHeight** e **outerWidth** al secondo snippet di codice. Ad esempio, puoi aggiungere `options='{"outerHeight":400, "outerWidth":600}'`, come in:

   ![](assets/socialonsite-resizewidget2.png)

   L’app social di Marketo ora aggiunge contenuti e interattività al sito web, invitando i fan, i visitatori e i clienti esistenti a parlare di te. Allo stesso tempo, aggiunge i dati del loro profilo al database e tiene traccia delle metriche di influenza social.

   >[!MORELIKETHIS]
   >
   >* [Pulsante Personalizza app social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [Imposta requisito condivisione social](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Pagine di destinazione Publish per Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
