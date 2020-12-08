---
unique-page-id: 2950561
description: Script di conversione per eventi personalizzati - Documenti Marketo - Documentazione prodotto
title: Script di conversione per eventi personalizzati
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# Script di conversione per eventi personalizzati {#conversion-script-for-custom-events}

Definite l&#39;obiettivo di evasione quando create un&#39;offerta di riferimento. Se l&#39;azione che conta verso l&#39;obiettivo è un evento specifico sulla tua pagina Web, puoi utilizzare uno script di conversione per chiamare la nostra API JavaScript.

## Recuperare lo script di conversione {#retrieve-the-conversion-script}

1. Nell&#39;editor delle offerte di riferimento, fate clic su Dettagli **** offerta, quindi selezionate Evento **JavaScript** cliente dal menu a discesa dell&#39;obiettivo di evasione.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Copiate lo script superiore nella casella grigia e inseritelo nella pagina Web all’interno dei `<body>` tag. Lo script inferiore viene posizionato all&#39;interno dei `<header>` tag.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >**Promemoria**
   >
   >
   >Ricordate di copiare e incollare entrambi gli script se si trovano su un sito Web non Marketo.

## Recuperare lo script Loader {#retrieve-the-loader-script}

1. Selezionate l&#39;offerta di riferimento dalla struttura, quindi fate clic su Azioni **offerta di** riferimento e codice **da** incorporare.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Fare clic con il pulsante destro del mouse sul codice **di** intestazione e inserirlo nell&#39;intestazione della pagina Web. Quindi, effettuate la stessa operazione per il **codice** del corpo.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Incollare gli script sulla pagina Web {#pasting-the-scripts-onto-your-webpage}

Incollate gli script di conversione in HTML per il corpo e l&#39;intestazione. Posizionare quindi gli script di caricamento nell&#39;HTML per il corpo e l&#39;intestazione.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Collegamento dello script di conversione {#connecting-the-conversion-script}

Qui è possibile scrivere una funzione JavaScript che utilizza l&#39;ID HTML specifico di qualsiasi elemento di pagina su cui si desidera attivare il completamento dell&#39;obiettivo. Ad esempio:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

In questo esempio sulla pagina Web è presente un pulsante con ID &quot;#myButtonId&quot;. Quando si fa clic su quel pulsante, la persona verrà registrata come se avesse completato l&#39;obiettivo.

Fantastico! Il sito Web ora sta acquisendo obiettivi di promozione sociale personalizzati con Marketo.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Specificare l&#39;obiettivo per l&#39;offerta di riferimento](../../../../product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Creare un&#39;offerta di riferimento](../../../../product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Implementare Social nel sito Web](deploy-social-on-your-website.md)

