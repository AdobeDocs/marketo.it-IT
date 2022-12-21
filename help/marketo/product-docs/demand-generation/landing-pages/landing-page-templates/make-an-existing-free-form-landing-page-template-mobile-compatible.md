---
unique-page-id: 5472348
description: Creare un modello di pagina di destinazione gratuito esistente compatibile con Mobile - Marketo Docs - Documentazione del prodotto
title: Rendere compatibile un modello mobile per pagina di destinazione in formato libero esistente
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# Rendere compatibile un modello mobile per pagina di destinazione in formato libero esistente {#make-an-existing-free-form-landing-page-template-mobile-compatible}

Questa operazione può essere eseguita in due posizioni: Editor modelli e Editor pagina di destinazione.

## Aggiornamento dall’Editor modelli {#upgrade-from-the-template-editor}

1. Vai a **Design Studio**.

   ![](assets/designstudio-1.png)

1. Seleziona **Modelli**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Selezionare un modello in cui **Compatibile con dispositivi mobili** è **No**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Fai clic su **Modifica bozza**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Fai clic su **Rendi compatibile con i dispositivi mobili**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Fai clic su **Aggiornamento**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   Il modello della pagina di destinazione è ora compatibile con i dispositivi mobili.

   >[!NOTE]
   >
   >L’aggiornamento dovrebbe essere innocuo, ma assicurati di controllare le pagine per eventuali discrepanze. L’aggiornamento crea bozze di qualsiasi pagina di destinazione che utilizza tale modello.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## Cosa rende un modello compatibile con dispositivi mobili? {#what-makes-a-template-mobile-compatible}

Grandi domande! Il modello deve avere i seguenti tag:

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`

Se tutto ha un buon aspetto, vedrete questo messaggio.

![](assets/image2015-1-22-20-3a41-3a31.png)

Se si verifica un errore, viene visualizzato un messaggio di errore, fare clic su ripristina per risolvere il problema e ripetere il processo di convalida.

![](assets/image2015-1-22-20-3a43-3a20.png)

Se apporti modifiche al modello, fai clic su Azioni modello e seleziona Convalida compatibilità mobile.

## Aggiornamento di un modello dall’Editor pagina di destinazione a forma libera {#upgrading-a-template-from-the-free-form-landing-page-editor}

Quando modifichi una pagina di destinazione e fai clic sulla scheda mobile, talvolta noti che il modello non è stato aggiornato. Non temete! Potete aggiornarlo proprio qui.

1. Fai clic sul pulsante **Mobile** scheda .

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Fai clic sulla casella di controllo e fai clic su **Attiva**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >L’attivazione della versione mobile di un modello crea le bozze di tutte le pagine di destinazione che lo utilizzano.

Fantastico! Ora puoi [personalizzare la visualizzazione mobile](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) di tutte le pagine di destinazione che utilizzano questo modello.
