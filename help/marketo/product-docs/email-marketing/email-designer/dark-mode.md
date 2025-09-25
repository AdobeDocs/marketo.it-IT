---
description: Modalità scura - Documentazione di Marketo - Documentazione del prodotto
title: Modalità scura
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: f960d7918d97a2c5e3d16673bc4c5c592004ff1e
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 1%

---

# Modalità scura {#dark-mode}

Durante la progettazione delle e-mail, il Designer e-mail consente di passare alla visualizzazione **[!UICONTROL Dark mode]**.

In **[!UICONTROL Dark mode]** è possibile definire impostazioni personalizzate specifiche da visualizzare supportando i client di posta elettronica quando la modalità scura è attiva.

## Cos’è la modalità scura? {#what-is-dark-mode}

La modalità scura consente ai client e-mail e alle app di visualizzare e-mail con sfondi più scuri e colori più chiari per testo, pulsanti e altri elementi dell’interfaccia utente. Aiuta a ridurre l&#39;affaticamento degli occhi, a risparmiare la durata della batteria e a migliorare la leggibilità in ambienti scarsamente illuminati, per un&#39;esperienza di visualizzazione più confortevole.

## Guardrail {#guardrails}

Il rendering in modalità scura può variare in modo significativo nei diversi client e-mail.

Prima di utilizzare la modalità scura, è importante comprendere in che modo i client e-mail principali la gestiscono. Ci sono tre casi da distinguere:

### Client che non supportano la modalità scura {#not-supporting}

Alcuni client di posta elettronica non supportano affatto questa funzione, ad esempio:

* Yahoo!Posta
* AOL

Che tu definisca o meno le impostazioni personalizzate della modalità scura, questi client e-mail non visualizzano mai alcun rendering della modalità scura.

### Client che applicano la propria modalità scura {#default-support}

Alcuni client e-mail applicano sistematicamente la propria modalità scura predefinita per tutte le e-mail ricevute. Colori, sfondi, immagini e così via vengono regolati automaticamente con le impostazioni della modalità scura specifiche per quel client e-mail. Non è possibile alcuna modifica esterna.

Questi client, ad esempio:

* Gmail (Posta sul desktop, iOS, Android, Posta sul web mobile)
* Windows Outlook
* Outlook Windows Mail

In questo caso, se definisci le impostazioni della modalità scura personalizzata in E-mail Designer, queste vengono ignorate dalle impostazioni del client e-mail.

Pertanto, anche se questi client e-mail gestiscono la modalità scura, la progettazione specifica della modalità scura non verrà renderizzata.

### Client che supportano la modalità scura personalizzata {#custom-support}

Altri client di posta elettronica offrono l&#39;opzione di eseguire il rendering della modalità scura personalizzata con la query `@media (prefers-color-scheme: dark)`, che è il metodo utilizzato dal Designer di posta elettronica [!DNL Marketo Engage].

Elenco dei client principali che gestiscono questa opzione:

* Apple Mail macOS
* Apple Mail iOS
* MacOS di Outlook
* Outlook.com
* IOS di Outlook
* Android di Outlook

In questo caso, devono essere visualizzate le impostazioni definite nel Designer e-mail.

>[!NOTE]
>
>Scopri come definire impostazioni personalizzate in modalità scura con E-mail Designer in [questa sezione](#define-custom-dark-mode).

Tuttavia, possono essere applicate alcune restrizioni in base a ciascun client e-mail. Ad esempio, alcuni client come Apple Mail 16 (macOs 13) non genereranno la modalità scura se le immagini sono presenti.

Per risultati ottimali, verifica il contenuto nei client e-mail di destinazione. Per visualizzare una simulazione che si avvicina il più possibile al risultato finale per ogni client, utilizzare la funzionalità [Rendering di e-mail](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md) in E-mail Designer.

## Modalità scura in E-mail designer {#dark-mode-email-designer}

Quando si tratta della modalità scura in E-mail Designer, ci sono due aspetti da considerare:

* Puoi ottenere un’anteprima di come verrà riprodotto il rendering della modalità scura predefinita nella maggior parte dei client e-mail che supportano. [Ulteriori informazioni](#preview-dark-mode)

* Se desideri ignorare le impostazioni predefinite di supporto dei client e-mail, puoi definire le impostazioni personalizzate della modalità scura nell’e-mail che stai modificando. [Ulteriori informazioni](#define-custom-dark-mode)

### Anteprima modalità scura predefinita {#preview-dark-mode}

Per accedere alla modalità scura in E-mail Designer e visualizzare un’anteprima delle impostazioni predefinite della modalità scura, segui la procedura riportata di seguito.

1. Dalla home page di E-mail Designer, selezionare l&#39;opzione **[!UICONTROL Design from scratch]**.

1. Aggiungi [strutture e contenuto](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#add-structure-and-content) alla tua e-mail.

1. In alto a destra, abilita l&#39;interruttore **[!UICONTROL Dark mode]**.

   SCHERMATA

1. Viene visualizzata l&#39;anteprima predefinita in modalità scura.

   SCHERMATA

Per impostazione predefinita, l’anteprima in modalità scura di E-mail Designer applica la combinazione di colori &quot;inversione completa dei colori&quot; a tutti gli elementi eccetto immagini e icone.

Significa che rileva aree con elementi chiari e scuri e le inverte, in modo che gli sfondi chiari diventino testo scuro e chiaro, mentre gli sfondi scuri diventino chiari e il testo chiaro diventi scuro.

>[!CAUTION]
>
>Il rendering finale può variare a seconda del client e-mail del destinatario. Per visualizzare una simulazione che si avvicina il più possibile al risultato finale per ogni client e-mail, utilizza l&#39;opzione [Rendering e-mail](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).

### Definire la modalità scura personalizzata {#define-custom-dark-mode}

Dopo il passaggio a **[!UICONTROL Dark mode]**, puoi scegliere di modificare elementi di stile specifici del contenuto che verranno visualizzati solo quando la modalità scura è abilitata nel client e-mail del destinatario, purché supporti tale funzione.

>[!WARNING]
>
>Il rendering finale in modalità scura dipende da ciascun client e-mail, pertanto i risultati possono variare da un client all’altro. [Ulteriori informazioni](#guardrails)

Per sfruttare lo stile personalizzato della modalità scura di E-mail Designer, Journey Optimizer utilizza la query CSS `@media (prefers-color-scheme: dark)` che rileva se il client e-mail dell&#39;utente è impostato sulla modalità scura e applica la progettazione a tema scuro definita nell&#39;e-mail.

Per definire le impostazioni personalizzate della modalità scura, effettua le seguenti operazioni.

1. Assicurarsi di passare all&#39;anteprima di **[!UICONTROL Dark mode]** nel Designer e-mail. [Scopri come](#preview-dark-mode)

1. Modifica gli attributi dei colori di stile come testo, sfondi, pulsante e così via.

1. Non è possibile modificare i colori delle immagini e delle icone, ma è possibile definire risorse specifiche solo per la modalità scura. A questo scopo, seleziona un’immagine. Passa a **[!UICONTROL Dark mode]** utilizzando l&#39;interruttore dedicato nel riquadro **[!UICONTROL Settings]** e seleziona un&#39;altra risorsa.

   SCHERMATA

1. In qualsiasi momento è possibile **[!UICONTROL Switch to live view]** per verificare come il contenuto potrebbe essere riprodotto su dispositivi di varie dimensioni. Da questa vista, seleziona l’opzione Modalità scura nella parte superiore dello schermo per visualizzare in anteprima la versione in modalità scura del contenuto tra i diversi dispositivi.

   SCHERMATA

   >[!CAUTION]
   >
   >La visualizzazione live è un’anteprima generica progettata per confrontare l’aspetto del rendering tra le varie dimensioni dei dispositivi. Il rendering finale può variare a seconda del client e-mail del destinatario.

1. Dopo aver apportato le modifiche desiderate per la modalità scura, fare clic su **[!UICONTROL Simulate Content]**.

   ![](assets/dark-mode-simulate.png)

1. Selezionare **[!UICONTROL Render email]** e connettersi all&#39;account Litmus. Puoi vedere il rendering finale in modalità scura per vari client e-mail. Ulteriori informazioni sul rendering di [e-mail](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).

   >[!WARNING]
   >
   >Anche se la simulazione si avvicina molto al modo in cui le e-mail appariranno in modalità scura, il rendering effettivo potrebbe variare a causa delle variazioni nei provider di servizi e-mail o nelle impostazioni a livello di dispositivo.

## Best practice {#best-practices}

Poiché l&#39;adozione della modalità scura aumenta tra i principali client e-mail, è essenziale considerare il rendering delle e-mail in ambienti chiari e scuri, indipendentemente dal fatto che si utilizzi la [modalità scura personalizzata](#define-custom-dark-mode) o meno.

La modalità scura può alterare i colori, gli sfondi e le immagini, a volte ignorando le scelte di progettazione. Per garantire coerenza visiva, accessibilità e integrità del brand, segui le best practice elencate di seguito.

**Ottimizza immagini e logo**

* Salvare logo e icone come file PNG con sfondi trasparenti per evitare la presenza di caselle bianche visibili in modalità scura.

* Evitare le immagini con sfondi bianchi o chiari codificati.

* Se la trasparenza non è un&#39;opzione, posizionate le immagini su uno sfondo a tinta unita nel progetto per evitare scomode inversioni di colore.

**Guarda gli sfondi**

* Assicurati un contrasto sufficiente tra il testo e i colori di sfondo per garantire leggibilità sia nelle modalità chiara che in quelle scure.

* Evita di utilizzare solo i colori di sfondo per i contenuti critici. Alcuni client ignorano i colori di sfondo in modalità scura, quindi assicurati che le informazioni chiave siano ancora visibili.

**Progettare contenuti accessibili in modalità scura**

* Utilizza combinazioni di colori facili da distinguere per le persone con daltonismo.

* Utilizza una palette di mezzitoni per garantire il contrasto sia contro gli sfondi chiari che scuri.

* Utilizza combinazioni di colori accessibili con contrasto elevato per migliorare la leggibilità e soddisfare gli standard delle linee guida per l’accessibilità dei contenuti web (WCAG). Utilizza strumenti come Verifica contrasto di WebAIM per verificare il contrasto dei colori.

* Evita i font sottili in quanto possono influire sulla leggibilità. Se il tuo marchio richiede un font sottile, grassetto in modalità scura.

* Salta il bianco puro sul nero puro in quanto può causare affaticamento degli occhi e potrebbe essere automaticamente invertito da alcuni client e-mail.

* Se la modalità scura non è supportata, fornisci uno stile di fallback accessibile.

**Verifica le e-mail in ambiente in modalità scura**

* Utilizza l&#39;[anteprima in modalità scura](#preview-dark-mode) di E-mail Designer che utilizza combinazioni di colori invertite per individuare in anticipo i problemi.

* Utilizza l&#39;opzione [Rendering di e-mail](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md) che sfrutta Litmus per simulare le progettazioni tra i principali client e-mail (Apple Mail, Gmail, Outlook) e vedere come si comportano i colori e le immagini in modalità scura.
