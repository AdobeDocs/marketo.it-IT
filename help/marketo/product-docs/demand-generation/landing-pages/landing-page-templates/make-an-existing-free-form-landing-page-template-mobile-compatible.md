---
unique-page-id: 5472348
description: Creare un modello di pagina di destinazione gratuito esistente compatibile con Mobile - Documenti Marketo - Documentazione prodotto
title: Creare un modello di pagina di destinazione gratuito esistente compatibile con Mobile
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Creare un modello di pagina di destinazione gratuito esistente compatibile con Mobile {#make-an-existing-free-form-landing-page-template-mobile-compatible}

>[!NOTE]
>
>I modelli delle pagine di destinazione creati prima del [rilascio di gennaio 2015](../../../../release-notes/2015/release-notes-january-2015.md)devono essere aggiornati in modo da essere compatibili con i dispositivi mobili.

Può essere eseguito in due posizioni: Editor modelli ed Editor pagina di destinazione.

## Aggiornamento dall&#39;Editor modelli {#upgrade-from-the-template-editor}

1. Andate a **Design Studio**.

   ![](assets/designstudio-1.png)

1. Selezionate **Modelli**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Selezionate un modello in cui **Mobile Compatible** è **No**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Fate clic su **Modifica bozza**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Fate clic su **Rendi compatibile** con i dispositivi mobili.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Fate clic su **Aggiorna**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   Il modello della pagina di destinazione è ora compatibile con i dispositivi mobili.

   >[!NOTE]
   >
   >L&#39;aggiornamento dovrebbe essere innocuo, ma assicurarsi di controllare le pagine per eventuali discrepanze. Con l’aggiornamento verranno create delle bozze di qualsiasi pagina di destinazione che utilizza tale modello.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## Cosa rende un modello compatibile con Mobile? {#what-makes-a-template-mobile-compatible}

Grandi domande! Il modello deve avere i seguenti tag:

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`  Se tutto ha un buon aspetto, vedrà questo messaggio.

![](assets/image2015-1-22-20-3a41-3a31.png)

Se si verifica un errore, viene visualizzato un messaggio di errore, fare clic su Ripristina per risolvere il problema e ripetere il processo di convalida.

![](assets/image2015-1-22-20-3a43-3a20.png)

Se apportate delle modifiche al modello, fate clic su Azioni modello e selezionate Convalida compatibilità mobile.

## Aggiornamento di un modello dall’Editor pagina di destinazione a forma libera {#upgrading-a-template-from-the-free-form-landing-page-editor}

Quando si modifica una pagina di destinazione e si fa clic sulla scheda mobile, talvolta si nota che il modello non è stato aggiornato. Non abbiate paura! Puoi aggiornarlo proprio qui.

1. Fate clic sulla scheda **Mobile** .

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Fate clic sulla casella di controllo e fate clic su **Attiva**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >Attivando la versione mobile di un modello si creano le bozze delle pagine di destinazione che lo utilizzano.

Fantastico! Ora potete [personalizzare la visualizzazione](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) mobile di tutte le pagine di destinazione che utilizzano questo modello.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Personalizza visualizzazione mobile per la pagina di destinazione a forma libera](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md)

>



