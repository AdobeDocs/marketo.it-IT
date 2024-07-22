---
unique-page-id: 2950561
description: Script di conversione per eventi personalizzati - Documentazione di Marketo - Documentazione del prodotto
title: Script di conversione per eventi personalizzati
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Script di conversione per eventi personalizzati {#conversion-script-for-custom-events}

Quando crei un’offerta di riferimento, definisci l’obiettivo di adempimento. Se l’azione che conta per raggiungere l’obiettivo è un evento specifico sulla tua pagina web, puoi utilizzare uno script di conversione per chiamare la nostra API JavaScript.

## Recuperare lo script di conversione {#retrieve-the-conversion-script}

1. Nell&#39;editor delle offerte di riferimento, fare clic su **Dettagli offerta** e quindi selezionare **Evento JavaScript cliente** dal menu a discesa obiettivo di evasione.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Copiare lo script superiore nella casella grigia e inserirlo nella pagina Web all&#39;interno dei tag `<body>`. Lo script inferiore si trova all&#39;interno dei tag `<header>`.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >Ricordati di copiare e incollare entrambi gli script se si trovano su un sito Web non Marketo.

## Recuperare lo script del caricatore {#retrieve-the-loader-script}

1. Seleziona l&#39;offerta di riferimento dalla struttura, quindi fai clic su **Azioni offerta di riferimento** e **Codice di incorporamento**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Fare clic con il pulsante destro del mouse su **Codice intestazione** e inserirlo nell&#39;intestazione della pagina Web. Eseguire quindi le stesse operazioni per il **codice corpo**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Incollare gli script nella pagina Web {#pasting-the-scripts-onto-your-webpage}

Incolla gli script di conversione nel HTML per il corpo e l’intestazione. Quindi, posiziona gli script loader nel HTML per il corpo e l’intestazione.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Collegamento dello script di conversione {#connecting-the-conversion-script}

Qui è dove scriverai una funzione JavaScript che utilizza l&#39;ID HTML specifico di qualsiasi elemento della pagina che desideri attivare il completamento dell&#39;obiettivo. Ad esempio:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

In questo esempio sulla pagina web è presente un pulsante con ID &quot;#myButtonId.&quot; Quando si fa clic su tale pulsante, la persona viene registrata come persona che ha completato l’obiettivo.

Fantastico! Il tuo sito web sta ora acquisendo obiettivi di promozione social personalizzati con Marketo.

>[!MORELIKETHIS]
>
>* [Specifica l&#39;obiettivo per l&#39;offerta di riferimento](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Crea un&#39;offerta di riferimento](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Distribuisci social network nel sito Web](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)
