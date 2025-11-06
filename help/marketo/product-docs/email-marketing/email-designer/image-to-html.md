---
title: Integrazione di GenStudio per Marketo Engage
description: Scopri come utilizzare GenStudio in Marketo Engage.
solution: Marketo Engage
product: marketo
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: 4667062002f24cd4f09aed3f747d82cd003351f6
workflow-type: tm+mt
source-wordcount: '1272'
ht-degree: 1%

---

# Conversione di immagini in modelli HTML {#image-to-html}

## Panoramica {#overview}

Il convertitore da immagine a HTML accelera in modo significativo la creazione di e-mail convertendo immagini statiche in modelli di contenuto e-mail HTML modulari e completamente personalizzabili. Questo strumento senza codice consente di trasformare le progettazioni visive di designer grafici o strumenti di progettazione in modelli e-mail dinamici e modificabili che possono essere riutilizzati più volte.

Sfruttando la tecnologia di intelligenza artificiale generativa, il convertitore da immagine a HTML analizza il layout, la tipografia, i colori e gli elementi visivi dell’immagine e genera un codice HTML pulito e modulare che mantiene la fedeltà di progettazione, garantendo al contempo la piena modificabilità e compatibilità con E-mail Designer.

>[!PREREQUISITES]
>
>* Devi innanzitutto accettare i [Termini Gen-AI di base e i termini supplementari](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} per l&#39;utilizzo della funzionalità Gen-AI in E-mail Designer. Per informazioni, contatta il team dell’account di Adobe (il tuo account manager).
>* Devi avere _Accedi al modello di e-mail_ e le autorizzazioni _Modifica/Genera modello di e-mail_ abilitate [nel tuo ruolo Marketo](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#edit-a-role).

## Conversione di un’immagine {#convert-an-image}

Per convertire un’immagine in un modello e-mail di HTML completamente personalizzabile, effettua le seguenti operazioni.

>[!NOTE]
>
>Per ottenere risultati ottimali, utilizza immagini di alta qualità con elementi visivi chiari e testo leggibile. Le immagini dovrebbero idealmente avere una larghezza compresa tra 600 e 800 pixel, in modo da corrispondere alle dimensioni standard delle e-mail.

1. In _Design Studio_, fai clic su **Modelli e-mail**, quindi su **Modelli e-mail (nuovi)**.

   ![](assets/image-to-html-1.png)

1. Fai clic su **[!UICONTROL Convert image to template]**.

   ![](assets/image-to-html-2.png)

1. Immettere un _nome modello_ e una descrizione facoltativa. Inoltre, è possibile scegliere lo stile del brand. Carica o trascina l’immagine desiderata.

   ![](assets/image-to-html-3.png)

1. Scorrere verso il basso e selezionare la casella di controllo _Il file di caricamento non contiene..._. Fare clic su **Converti**.

   ![](assets/image-to-html-4.png)

   >[!NOTE]
   >
   >Il processo di generazione può richiedere fino a cinque minuti a seconda della complessità e delle dimensioni del progetto dell&#39;immagine. L’elaborazione basata su IA avviene in background, per consentirti di allontanarti da questa schermata e lavorare su altre attività mentre la conversione è in corso. Potrebbe essere necessario aggiornare la schermata della libreria del _modello e-mail_ per visualizzare il cambiamento di stato.

1. Una volta completata la conversione, il modello viene salvato automaticamente come bozza. Selezionala..

   ![](assets/image-to-html-5.png)

1. Il modello convertito si apre in E-mail Designer con funzionalità di modifica complete. Ora puoi:

   * Modificare il contenuto di testo e applicare la personalizzazione
   * Modificare le immagini e aggiungere collegamenti
   * Regolazione di colori, caratteri e stile
   * Aggiungere, rimuovere o ridisporre i componenti di contenuto
   * Sfrutta tutte le funzioni di E-mail Designer come con qualsiasi altro modello

   ![](assets/image-to-html-6.png){width="800" zoomable="yes"}

1. Puoi apportare le modifiche necessarie per perfezionare il modello e allinearlo alle linee guida del tuo marchio.

1. Una volta completato il modello, fai clic su **[!UICONTROL Save & close]**, quindi su **Pubblica**.

Il modello è ora disponibile nella libreria _Modelli e-mail_ e può essere utilizzato per creare e-mail.

## Casi d’uso comuni {#use-cases}

Il convertitore immagine-HTML è ideale per:

* **Migrazione piattaforma**: migrazione da un&#39;altra piattaforma di e-mail marketing? Converti le progettazioni e-mail esistenti in modelli HTML pronti per Marketo Engage senza ricompilare da zero
* **Conversione di modelli di progettazione**: trasforma i modelli di progettazione da strumenti come Photoshop, Figma o altri software di progettazione in modelli e-mail funzionali
* **Creazione rapida di modelli**: generazione rapida di modelli e-mail per campagne sensibili al tempo senza attendere risorse per sviluppatori
* **Creazione di librerie di modelli**: crea una libreria completa di modelli coerenti con il marchio che i membri del team non tecnici possono personalizzare e distribuire

## Best practice {#best-practices}

**Prima di iniziare**

* **Salva contenuto esistente**: la conversione di un&#39;immagine in HTML sostituirà tutto il contenuto esistente nel messaggio e-mail. Salvare sempre il lavoro corrente prima di utilizzare questa funzione.
* **Pianifica il flusso di lavoro**: utilizza l&#39;immagine per il convertitore HTML all&#39;inizio del processo di creazione dell&#39;e-mail oppure assicurati di essere pronto a sostituire tutto il contenuto corrente.

**Preparazione immagine**

* **Risoluzione**: utilizza immagini ad alta risoluzione per migliorare il riconoscimento del testo e il rilevamento degli elementi.
* **Chiarezza**: verifica che il testo sia chiaramente leggibile e che gli elementi visivi siano ben definiti.
* **Larghezza**: progettare immagini con larghezze di posta elettronica standard (600-800 px) corrispondenti ai requisiti tipici del client di posta elettronica.
* **Formato file**: usa il formato JPEG o PNG. Evita immagini compresse o di bassa qualità.
* **Progettazione completa**: include la progettazione completa delle e-mail in un&#39;unica immagine, dall&#39;intestazione al piè di pagina.

**Considerazioni sulla progettazione**

* **Layout semplici**: i layout semplici e ben strutturati vengono convertiti in modo più accurato rispetto alle progettazioni molto complesse.
* **Elementi standard**: utilizza pattern comuni per la progettazione di e-mail (intestazione, sezioni del corpo, CTA, piè di pagina).
* **Leggibilità del testo**: garantire un contrasto sufficiente tra testo e sfondi.
* **Tipi di carattere sicuri per il Web**: le progettazioni che utilizzano tipi di carattere comuni per il Web avranno una maggiore fedeltà.
* **Evita elementi sovrapposti**: separa chiaramente gli elementi di progettazione per un migliore riconoscimento della struttura.

**Dopo la conversione**

* **Rivedi la bozza**: una volta completata la conversione, il modello viene salvato automaticamente come bozza. Prenditi del tempo per verificare attentamente la precisione del HTML generato.
* **Verifica approfondita**: verifica l&#39;e-mail tra client e dispositivi diversi. Per risultati più rapidi, sfrutta l&#39;integrazione di [Litmus](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).
* **Perfeziona manualmente**: apporta le modifiche necessarie utilizzando le funzionalità di modifica completa di E-mail Designer.
* **Allineamento marchio**: verifica che colori, font e stile corrispondano alle linee guida del tuo marchio.
* **Personalization**: aggiungi contenuto dinamico e token di personalizzazione come desiderato.
* **Accessibilità**: se necessario, rivedere e migliorare le funzioni di accessibilità.

## Limitazioni e considerazioni {#limitations}

Tieni presente le seguenti limitazioni quando utilizzi il convertitore da immagine a HTML.

* **Interpretazione IA**: l&#39;intelligenza artificiale genera HTML in base a un&#39;interpretazione visiva dell&#39;immagine. Progetti complessi o insoliti possono richiedere regolazioni manuali dopo la conversione.

* **Precisione del testo**: mentre l&#39;intelligenza artificiale tenta di riconoscere e riprodurre il testo con precisione, verifica sempre il contenuto del testo e apporta le correzioni necessarie.

* **Contenuto dinamico**: il processo di conversione crea un HTML statico in base all&#39;immagine. Dopo la conversione, dovrai aggiungere manualmente personalizzazione, contenuto dinamico e tracciamento.

* **Layout complessi**: le progettazioni molto complesse con livelli complessi, forme insolite o elementi non standard potrebbero non convertirsi perfettamente. Le progettazioni più semplici danno generalmente risultati migliori.

* **Tempo di elaborazione**: il processo di conversione può richiedere fino a cinque minuti a seconda della complessità e delle dimensioni dell&#39;immagine. L’elaborazione basata su IA viene eseguita in background, consentendoti di lavorare su altre attività senza mantenere aperta la schermata. Il modello viene salvato automaticamente come bozza al termine della conversione.

>[!NOTE]
>
>Il convertitore da immagine a HTML è progettato per fornire un forte punto di partenza per la creazione di e-mail. Il HTML generato deve essere rivisto e perfezionato utilizzando E-mail Designer per garantire che soddisfi le tue esigenze.

## Domande frequenti {#faq}

+++Cosa succede al contenuto delle e-mail esistenti quando utilizzo il convertitore immagine-HTML?

Tutto il contenuto esistente nel messaggio e-mail verrà eliminato e sostituito con il modello appena generato quando carichi un’immagine per la conversione. Prima di utilizzare questa funzione, assicurati di salvare tutti i contenuti importanti. È meglio utilizzare il convertitore da immagine a HTML all’inizio del processo di creazione dell’e-mail.

+++

+++Quali formati di file sono supportati?

Il convertitore da immagine a HTML supporta i formati immagine JPEG (.jpg, .jpeg) e PNG (.png).

+++

+++Quanto tempo ci vuole per il processo di conversione?

La conversione può richiedere fino a cinque minuti, a seconda della complessità e delle dimensioni del design dell’immagine. L’elaborazione basata su intelligenza artificiale avviene in background, per consentirti di spostarti e lavorare su altre attività; non è necessario tenere aperta la schermata. Una volta completata la conversione, il file verrà automaticamente salvato come bozza da rivedere e modificare.

+++

+++Posso modificare il modello generato?

Sì! Il modello HTML generato si apre in E-mail Designer con funzionalità di modifica complete. È possibile modificare tutti gli aspetti del modello, inclusi testo, immagini, stile, layout e struttura.

+++

+++Cosa succede se la conversione non corrisponde esattamente al mio progetto?

L’intelligenza artificiale fa del suo meglio per interpretare accuratamente il tuo progetto, ma potrebbe essere necessario un qualche perfezionamento manuale. Utilizza E-mail Designer per modificare tutti gli elementi che richiedono un’ottimizzazione.

+++

+++Posso utilizzare questa funzione per pagine di destinazione o altri tipi di contenuto?

Il convertitore da immagine a HTML è attualmente progettato in modo specifico per i modelli e-mail. Per altri tipi di contenuto, utilizza le opzioni standard di progettazione e importazione disponibili in E-mail Designer.

+++

+++Posso riutilizzare i modelli convertiti in più campagne e-mail?

Sì! I modelli creati con l&#39;immagine nel convertitore HTML vengono salvati automaticamente nella libreria _Modelli e-mail_. Potrai accedervi e riutilizzarli in qualsiasi e-mail successiva.

+++
