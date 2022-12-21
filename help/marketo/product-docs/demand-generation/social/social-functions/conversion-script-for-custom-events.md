---
unique-page-id: 2950561
description: Script di conversione per eventi personalizzati - Documenti Marketo - Documentazione del prodotto
title: Script di conversione per eventi personalizzati
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Script di conversione per eventi personalizzati {#conversion-script-for-custom-events}

Puoi definire l’obiettivo di evasione quando crei un’offerta di riferimento. Se l&#39;azione che conta verso l&#39;obiettivo è un evento specifico sulla tua pagina web, puoi utilizzare uno script di conversione per chiamare la nostra API JavaScript.

## Recupera lo script di conversione {#retrieve-the-conversion-script}

1. Nell’editor delle offerte di riferimento, fai clic su **Dettagli offerta** quindi seleziona **Evento JavaScript del cliente** dal menu a discesa dell’obiettivo di realizzazione.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Copia lo script superiore nella casella grigia e inseriscilo nella pagina web all’interno del `<body>` tag. Lo script inferiore viene posizionato all&#39;interno del `<header>` tag.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >Ricordare di copiare e incollare entrambi gli script se si trovano in un sito Web non Marketo.

## Recupera lo script del caricatore {#retrieve-the-loader-script}

1. Seleziona l’offerta di riferimento dalla struttura, quindi fai clic su **Azioni di offerta di riferimento** e **Codice di incorporamento**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Fai clic con il pulsante destro del mouse sul pulsante **Codice intestazione** e inseriscilo nell&#39;intestazione della pagina web. Quindi fai lo stesso per il **Codice del corpo**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Incollare gli script nella pagina web {#pasting-the-scripts-onto-your-webpage}

Incolla gli script di conversione in HTML per il corpo e l’intestazione. Quindi, inserire gli script del caricatore in HTML per il corpo e l’intestazione.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Collegamento dello script di conversione {#connecting-the-conversion-script}

Qui è possibile scrivere una funzione JavaScript che utilizza l&#39;ID HTML specifico di qualsiasi elemento di pagina su cui desideri attivare il completamento dell&#39;obiettivo. Ad esempio:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

In questo esempio, sulla pagina web è presente un pulsante con ID &quot;#myButtonId&quot;. Quando fai clic su quel pulsante, la persona verrà registrata come se avesse completato l’obiettivo.

Fantastico! Il tuo sito web sta ora acquisendo obiettivi di promozione social personalizzati con Marketo.

>[!MORELIKETHIS]
>
>* [Specifica obiettivo per offerta di riferimento](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Creare un’offerta di riferimento](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Distribuisci Social sul tuo sito web](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)

