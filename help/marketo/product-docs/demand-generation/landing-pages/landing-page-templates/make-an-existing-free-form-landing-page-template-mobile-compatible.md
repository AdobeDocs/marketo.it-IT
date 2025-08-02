---
unique-page-id: 5472348
description: Rendere compatibile per dispositivi mobili un modello di pagina di destinazione in formato libero esistente - Documenti Marketo - Documentazione del prodotto
title: Rendi compatibile con dispositivi mobili un modello di pagina di destinazione in formato libero esistente
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
feature: Landing Pages
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 1%

---

# Crea un modello di pagina di destinazione in formato libero esistente [!UICONTROL Mobile Compatible] {#make-an-existing-free-form-landing-page-template-mobile-compatible}

Questa operazione può essere eseguita in due posizioni, Editor modelli e Editor pagina di destinazione.

## Eseguire l’aggiornamento dall’Editor modelli {#upgrade-from-the-template-editor}

1. Passare a **[!UICONTROL Design Studio]**.

   ![](assets/designstudio-1.png)

1. Seleziona **[!UICONTROL Templates]**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Selezionare un modello in cui **[!UICONTROL Mobile Compatible]** è **[!UICONTROL No]**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Fai clic su **[!UICONTROL Edit Draft]**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Fai clic su **[!UICONTROL Make Mobile Compatible]**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Fai clic su **[!UICONTROL Upgrade]**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   Il modello della pagina di destinazione è ora compatibile con dispositivi mobili.

   >[!NOTE]
   >
   >L’aggiornamento dovrebbe essere innocuo, ma assicurati di controllare le pagine per eventuali discrepanze. L&#39;aggiornamento creerà le bozze di tutte le pagine di destinazione che utilizzano tale modello.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## Cosa crea un modello [!UICONTROL Mobile Compatible]? {#what-makes-a-template-mobile-compatible}

Grandi domande! Il modello deve avere i seguenti tag:

`Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV>`

Se tutto sembra a posto, vedrai questo messaggio.

![](assets/image2015-1-22-20-3a41-3a31.png)

Se si verifica un errore, viene visualizzato un messaggio di errore, fare clic su Ripristina per risolvere il problema e ripetere il processo di convalida.

![](assets/image2015-1-22-20-3a43-3a20.png)

Se si apportano modifiche al modello, fare clic su [!UICONTROL Template Actions] e selezionare [!UICONTROL Validate Mobile Compatibility].

## Aggiornamento di un modello dall’Editor pagina di destinazione in formato libero {#upgrading-a-template-from-the-free-form-landing-page-editor}

Quando modifichi una pagina di destinazione e fai clic sulla scheda mobile, a volte noterai che il modello non è stato aggiornato. Non abbiate paura! Puoi aggiornarla proprio qui.

1. Fare clic sulla scheda **[!UICONTROL Mobile]**.

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Selezionare la casella di controllo e fare clic su **[!UICONTROL Activate]**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >L’attivazione della versione mobile di un modello creerà le bozze di tutte le pagine di destinazione che lo utilizzano.

Fantastico! Ora puoi [personalizzare la visualizzazione per dispositivi mobili](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) di tutte le pagine di destinazione che utilizzano questo modello.
