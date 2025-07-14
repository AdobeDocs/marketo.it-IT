---
solution: Marketo Engage
product: marketo
title: Aggiungere un CSS personalizzato al contenuto dell’e-mail
description: Scopri come aggiungere CSS personalizzati al contenuto delle e-mail direttamente nel Designer e-mail in Marketo Engage.
level: Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
exl-id: c191b44a-47ab-41f8-aa95-9268e359e5db
source-git-commit: 37938db9eafbe7860448d438e2fa03adccd043ec
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 3%

---

# Aggiungere un CSS personalizzato al contenuto dell’e-mail {#custom-css}

Aggiungi un CSS personalizzato direttamente in Marketo Engage Email Designer per uno stile avanzato e specifico.

## Definire CSS personalizzato {#define-custom-css}

1. Assicurati che nel Designer e-mail sia definito del contenuto aggiungendo almeno un componente.

1. Selezionare **[!UICONTROL Body]** da **[!UICONTROL Navigation tree]** a sinistra o nel riquadro di destra. **[!UICONTROL CSS styles]** viene visualizzato a destra.

   ![](assets/custom-css-1.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >La sezione **[!UICONTROL CSS styles]** è disponibile solo quando il contenuto è presente nell&#39;editor.

1. Fare clic sul pulsante **[!UICONTROL + Add custom CSS]**.

   >[!NOTE]
   >
   >Il pulsante **[!UICONTROL Add custom CSS]** è disponibile solo quando è selezionato **[!UICONTROL Body]**. Tuttavia, puoi applicare stili CSS personalizzati a tutti i componenti all’interno del contenuto.

1. Inserisci il codice CSS nell’area di testo dedicata visualizzata. Verificare che il file CSS personalizzato [ sia valido e che segua la sintassi corretta](#use-valid-css). Al termine, fai clic su **Salva**.

   ![](assets/custom-css-2.png)

   >[!NOTE]
   >
   >Non puoi aggiungere CSS personalizzati al contenuto quando utilizzi un modello [ con contenuto bloccato](/help/marketo/product-docs/email-marketing/email-designer/content-locking.md). L&#39;etichetta del pulsante diventa **[!UICONTROL View custom CSS]** ed eventuali CSS personalizzati visualizzati sono di sola lettura.

1. Assicurati che il CSS sia applicabile al contenuto. In caso contrario, controllare la sezione [Risoluzione dei problemi](#troubleshooting).

   ![](assets/custom-css-3.png)

   >[!NOTE]
   >
   >Se rimuovi tutto il contenuto, la sezione scompare e non viene più applicato il CSS personalizzato definito in precedenza. Aggiungere nuovamente il contenuto per visualizzare di nuovo la sezione **[!UICONTROL CSS styles]**. Il CSS personalizzato viene applicato nuovamente.

## Utilizzo di CSS validi {#using-valid-css}

È possibile immettere qualsiasi stringa CSS valida nell&#39;area di testo **[!UICONTROL Add custom CSS]**. I file CSS formattati correttamente vengono applicati immediatamente al contenuto.

>[!CAUTION]
>
>Sei responsabile della sicurezza del CSS personalizzato. Assicurati che il CSS non introduca vulnerabilità o conflitti con il contenuto esistente.
>
>Evita l’utilizzo di CSS che potrebbero interrompere involontariamente il layout o la funzionalità del contenuto.

+++ Esempi di CSS validi

Di seguito sono riportati alcuni esempi di CSS validi.

```css
.acr-component[data-component-id="form"] {
  display: flex;
  justify-content: center;
  background: none;
}

.acr-Form {
  width: 100%;
  padding: 20px 100px;
  border-spacing: 0px 8px;
  box-sizing: border-box;
  margin: 0;
}

.acr-Form .spectrum-FieldLabel {
  width: 20%;
}

.acr-Form.spectrum-Form--labelsAbove .spectrum-FieldLabel,
.acr-Form [data-form-item="checkbox"] .spectrum-FieldLabel {
  width: auto;
}

.acr-Form .spectrum-Textfield {
  width: 100%;
}

#acr-form-error,
#acr-form-confirmation {
  width: 100%;
  padding: var(--spectrum-global-dimension-static-size-500);
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  gap: var(--spectrum-global-dimension-static-size-200);
}

.spectrum-Form-item.is-required .spectrum-FieldLabel:after{
  content: '*';
  font-size: 1.25rem;
  margin-left: 5px;
  position: absolute;
}

/* Error field placeholder */
.spectrum-HelpText {
  display: none !important;
}

.spectrum-HelpText.is-invalid,
.is-invalid ~ .spectrum-HelpText {
  display: flex !important;
}
```

```css
@media only screen and (min-width: 600px) {
  .acr-paragraph-1 {
    width: 100% !important;
  }
}
```

+++


+++ Esempi di CSS non valido

Se viene immesso un file CSS non valido, viene visualizzato un messaggio di errore che indica che il file CSS non può essere salvato. Di seguito sono riportati alcuni esempi di file CSS non validi.

L&#39;utilizzo di `<style>` tag non è accettato:

```html
<style type="text/css">
  .acr-Form {
    width: 100%;
    padding: 20px 100px;
    border-spacing: 0px 8px;
    box-sizing: border-box;
    margin: 0;
  }
</style>
```

Sintassi non valida, ad esempio parentesi graffe mancanti, non accettata:

```css
body {
  background: red;
```

+++

## Implementazione tecnica {#implementation}

Il file CSS personalizzato viene aggiunto alla fine della sezione `<head>` come parte di un tag `<style>` con l&#39;attributo `data-name="global-custom"`, come nell&#39;esempio seguente. In questo modo gli stili personalizzati vengono applicati globalmente al contenuto.

+++ Vedi esempio

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="content-version" content="3.3.31">
    <meta name="x-apple-disable-message-reformatting">
    <meta name="viewport" content="width=device-width,initial-scale=1.0">
    <style data-name="default" type="text/css">
      td { padding: 0; }
      th { font-weight: normal; }
    </style>
    <style data-name="grid" type="text/css">
      .acr-grid-table { width: 100%; }
    </style>
    <style data-name="acr-theme" type="text/css" data-theme="default" data-variant="0">
      body { margin: 0; font-family: Arial; }
    </style>
    <style data-name="media-default-max-width-500px" type="text/css">
      @media screen and (max-width: 500px) {
        body { width: 100% !important; }
      }
    </style>
    <style data-name="global-custom" type="text/css">
      /* Add you custom CSS here */
    </style>
  </head>
  <body>
    <!-- Minimal content -->
  </body>
</html>
```

+++


Il CSS personalizzato non viene interpretato o convalidato dal riquadro **[!UICONTROL Settings]** di E-mail Designer. È completamente indipendente e può essere modificata solo tramite l&#39;opzione **[!UICONTROL Add Custom CSS]**.

### Guardrail - Contenuto importato {#guardrails}

Se desideri utilizzare CSS personalizzati con il contenuto importato nel Designer e-mail, considera quanto segue:

* Se [si importa contenuto HTML](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html) esterno, inclusi i file CSS, a meno che non si converta tale contenuto, il contenuto si troverà in **[!UICONTROL Compatibility mode]**, dove la sezione **[!UICONTROL CSS styles]** non è disponibile.

* Se l&#39;importazione del contenuto creato con E-mail Designer include CSS applicati tramite l&#39;opzione **[!UICONTROL Add custom CSS]**, il CSS applicato in precedenza sarà visibile e modificabile dalla stessa opzione.

## Risoluzione dei problemi {#troubleshooting}

Se il CSS personalizzato non è applicato, prova i suggerimenti riportati di seguito.

* Assicurati che il CSS sia valido e privo di errori di sintassi (ad esempio parentesi graffe mancanti, nomi di proprietà errati). [Scopri come](#use-valid-css)

* Verificare che il file CSS venga aggiunto al tag `<style>` con l&#39;attributo `data-name="global-custom"`.

* Verificare se l&#39;attributo `global-custom` del tag di stile `data-disabled` è impostato su `true`. In tal caso, il CSS personalizzato non viene applicato.

+++ Ad esempio:

  ```html
  <style data-name="global-custom" type="text/css" data-disabled="true"> body: { color: red; } </style>
  ```

+++

* Assicurati che il CSS non sia sostituito da altre regole CSS.

   * Utilizza gli strumenti di sviluppo del browser per esaminare il contenuto e verificare che i CSS stiano eseguendo il targeting dei selettori corretti.

   * Prendi in considerazione l&#39;aggiunta di `!important` alle tue dichiarazioni per assicurarti che abbiano la precedenza.

+++ Ad esempio:

     ```css
     .acr-Form {
       background: red !important;
     }
     ```

+++

>[!NOTE]
>
>Il supporto Marketo Engage non è configurato per assistere nella risoluzione dei problemi relativi ai file CSS personalizzati. Per assistenza CSS, consulta uno sviluppatore web.
