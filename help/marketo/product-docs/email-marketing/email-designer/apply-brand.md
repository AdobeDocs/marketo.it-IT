---
solution: Marketo Engage
product: marketo
title: TITOLO
description: Scopri come semplificare la creazione di e-mail con temi e moduli riutilizzabili, garantendo coerenza ed efficienza del design.
feature: Email Designer
role: User
level: Beginner, Intermediate
hide: true
hidefromtoc: true
exl-id: 349ee021-7341-40e0-8d8c-d041f1a8f343
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 4%

---

# Applicare temi al contenuto dell’e-mail {#apply-email-themes}

>[!AVAILABILITY]
>
>Questa funzionalità è disponibile attualmente in versione beta e solo per la clientela beta. Per partecipare al programma Beta, contatta il tuo rappresentante Adobe.

Con i temi, gli utenti non tecnici hanno la possibilità di creare contenuti riutilizzabili che si adattano a un marchio e a un linguaggio di progettazione specifici aggiungendo stili personalizzati sopra i modelli standard<!-- to achieve brand specific results-->.

Questa funzione consente agli addetti al marketing di sfruttare le e-mail visivamente accattivanti e coerenti con il brand in modo più rapido e con meno sforzo, fornendo al contempo opzioni di personalizzazione avanzate per esigenze di progettazione univoche.

<!--What is the Enhanced Email Authoring Experience?

This feature introduces two key components to simplify and enhance email creation:

* **Theme Management System**: A centralized system for creating, customizing, and applying reusable themes to emails. Themes ensure consistent styling across campaigns and eliminate the need for repetitive manual styling.

* **Modules**: Pre-designed, reusable content blocks that abstract common email elements (e.g., titles, descriptions, images, and links). Modules are built using customizable low-level components, offering flexibility while maintaining design standards.

Key Benefits:

- **Consistency**: Ensure all emails align with your brand's design guidelines.
- **Efficiency**: Save time by reusing themes and modules across campaigns.
- **Customization**: Add custom CSS and mobile-specific styles for advanced designs.
- **Scalability**: Eliminate repetitive styling tasks, enabling faster email creation.-->

## Guardrail e limitazioni {#themes-guardrails}

* Quando crei un’e-mail da zero, puoi scegliere di iniziare a creare i contenuti utilizzando un tema per applicare rapidamente uno stile specifico che si adatta al tuo marchio e design.

  Se scegli la modalità _Stile manuale_, non potrai applicare alcun tema a meno che non reimposti l&#39;e-mail.

* [I frammenti](/help/marketo/product-docs/email-marketing/email-designer/fragments.md) non sono compatibili tra le modalità _Usa temi_ e _Stile manuale_.

  Per poter utilizzare un frammento in un contenuto in cui è applicato un tema, è necessario creare il frammento in modalità _Usa temi_.

* Se utilizzi contenuto creato in HTML, sarai in [modalità di compatibilità](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html) e non puoi applicare temi a questo contenuto.

  Per sfruttare appieno tutte le funzionalità di E-mail Designer, inclusi i temi, è necessario creare nuovi contenuti in modalità _Usa temi_ o convertire i [contenuti HTML importati](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html).

<!--If using a content created in Manual Styling mode or HTML, you cannot apply themes to this content. You must create a new content in Use Themes mode.

If you apply a theme to a content using a [fragment](../content-management/fragments.md) created in Manual Styling mode, the rendering may not be optimal.-->

## Creare un tema {#create-and-edit-themes}

Per definire un tema che puoi sfruttare nei contenuti delle e-mail future, segui i passaggi indicati di seguito.

1. Per iniziare, crea un nuovo [modello e-mail](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template).

1. Selezionare l&#39;opzione **[!UICONTROL Create or edit themes]**.

   `![](assets/theme-create.png)`

1. Puoi selezionare il tema predefinito oppure utilizzare un modello Adobe o personalizzato. In questo esempio, selezionare il tema predefinito e fare clic su **[!UICONTROL Create]**.

   `![](assets/theme-select.png)`

1. Nella scheda **[!UICONTROL General settings]**, inizia a definire il tema assegnandogli un nome specifico per il tuo marchio. Puoi regolare la larghezza predefinita delle e-mail ed esportare il tema corrente per condividerlo tra le sandbox.

   `<!--![](assets/theme-general-settings.png)-->`

1. Utilizza la barra a destra per spostarti tra le diverse schede e aggiornare le impostazioni di progettazione.

   `![](assets/theme-right-pane.png)`

1. Dalla scheda **[!UICONTROL Colors]**:

   * Utilizza il pulsante **[!UICONTROL Edit]** per impostare **[!UICONTROL Color palette]** con i colori predefiniti per il tuo marchio. Selezionare **[!UICONTROL Preset]** per creare rapidamente una combinazione di colori o regolare singolarmente ogni colore del tema. Puoi anche utilizzare una combinazione di entrambi.

     `![](assets/theme-colors.gif)`

   * Fare clic su **[!UICONTROL Add variant]** per creare più varianti di colore, ad esempio la modalità chiara e scura, in cui ogni variante dispone di una propria tavolozza di colori e controlli sfumatura.

     `![](assets/theme-colors-variant.png)`

   * Per ogni variante, fai clic sull’icona Modifica per modificare un singolo elemento. Puoi utilizzare la palette predefinita creata oppure qualsiasi colore personalizzato.

     `![](assets/theme-colors-edit-variant.gif)`

1. In **[!UICONTROL Text settings]** è possibile impostare il tipo di carattere globale da utilizzare per l&#39;intero tema. Per un controllo più granulare, è inoltre possibile modificare ogni intestazione e tipo di paragrafo per regolare il carattere, le dimensioni, lo stile e così via.

   `![](assets/theme-text.png)`

1. Nella scheda **[!UICONTROL Spacing]**, selezionare un singolo elemento dall&#39;elenco per inserirlo correttamente tra i diversi componenti.

   `<!--![](assets/theme-spacing.png)-->`

1. Utilizzando le altre schede a destra, è possibile gestire separatamente ogni elemento pulsante, divisore, formattazione immagine aggiuntiva e spaziatura layout griglia per questo tema.

   `<!--![](assets/theme-buttons.png)-->`

1. Fare clic su **[!UICONTROL Save]** per memorizzare questo tema per utilizzi futuri.

## Applicare temi a un’e-mail {#apply-themes}

Per applicare temi di stile predefiniti o personalizzati a un’e-mail, segui la procedura riportata di seguito.

1. `In [!DNL Marketo Engage], [add an email](create-email.md) action to a journey or campaign, and [edit your email body](get-started-email-design.md#key-steps).`

1. Puoi selezionare una delle seguenti azioni:

   * `Select a built-in [email template](use-email-templates.md) to open the Email Designer. A default theme specific to each template is automatically applied.`

   * `Design a [new content from scratch](content-from-scratch.md) and select **[!UICONTROL Use Themes]** to start with a predefined styling theme.`

     `![](assets/theme-from-scratch.png)`

     >[!CAUTION]
     >
     >Se scegli la modalità _Stile manuale_, non potrai applicare alcun tema a meno che non reimposti l&#39;e-mail.
     >
     >Per utilizzare un [frammento](/help/marketo/product-docs/email-marketing/email-designer/fragments.md) in modalità _Usa temi_, è necessario che il frammento sia stato creato utilizzando la modalità _Usa temi_.

1. Una volta nel Designer di posta elettronica, fare clic sul pulsante **[!UICONTROL Themes]** nella barra a destra. Viene visualizzato il tema predefinito o il tema del modello. Per questo tema è possibile alternare tra le due varianti di colore.

   `![](assets/theme-default-hero.png)`

1. Fare clic sulla freccia accanto al tema attualmente utilizzato. Viene visualizzato l’elenco dei temi personalizzati e Adobe disponibili.

   `![](assets/theme-hero-change.png)`

1. Fare clic su **[!UICONTROL Custom themes]** e selezionare il tema creato.

   `![](assets/theme-select-custom.png)`

1. Fai clic all’esterno dell’elenco a discesa. Il tema personalizzato appena selezionato applica automaticamente i relativi stili a tutti i componenti e-mail. Puoi alternare tra le due varianti di colore.

1. Quando un componente è selezionato, è comunque possibile sbloccarne lo stile utilizzando l’icona dedicata.

   `![](assets/theme-unlock-style.png)`

È possibile cambiare tema in qualsiasi momento. Il contenuto dell’e-mail rimane invariato, ma gli stili vengono aggiornati per riflettere il nuovo tema.

<!--
>[!NOTE]
> - Themes apply styles globally. Ensure your theme is finalized before applying it to multiple emails.
> - Switching themes may override custom styles applied to individual components.

>[!CAUTION]
> - When using fragments, the email's theme will override the fragment's styles. A warning will be displayed in the editor if there is a conflict.

## Example Use Cases {#example-use-cases}

### 1. Creating a New Theme
- A marketer creates a theme with their brand's colors, fonts, and button styles.
- The theme is saved and reused across multiple email campaigns.

### 2. Switching Themes
- A marketer applies a holiday-themed design to an existing email by switching to a pre-designed holiday theme.-->
