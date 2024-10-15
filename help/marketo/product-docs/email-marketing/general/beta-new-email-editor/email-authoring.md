---
description: Authoring delle e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Authoring di e-mail
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 482c2955bbf3ad10d244ebc5e6b6d6a37d82c217
workflow-type: tm+mt
source-wordcount: '1212'
ht-degree: 1%

---

# Authoring di e-mail {#email-authoring}

Testo introduttivo qui.

>[!IMPORTANT]
>
>Questo articolo è valido solo per i membri della versione beta dell’Editor e-mail per il nuovo Marketo Engage. Non divulgare.

## Creare un messaggio e-mail {#create-an-email}

1. Accedi al Marketo Engage tramite [Adobe Experience Cloud](https://experiencecloud.adobe.com/){target="_blank"}.

1. In Il mio Marketo, seleziona **Design Studio**.

   ![](assets/create-an-email-1.png)

1. Nella struttura, seleziona **E-mail (nuovo editor)**.

   ![](assets/create-an-email-2.png)

1. Fai clic sul pulsante **Crea e-mail**.

   ![](assets/create-an-email-3.png)

1. Immetti un nome e un oggetto per l’e-mail. Fai clic su **Crea**.

   ![](assets/create-an-email-4.png)

Tutto qui. Ora è il momento di progettare la tua e-mail.

## Scegli il tipo di contenuto {#choose-your-content-type}

1. Nell&#39;e-mail appena creata, fare clic su **+ Aggiungi contenuto e-mail**.

   SCHERMATA

1. La pagina _Crea messaggio e-mail_ viene caricata. Puoi scegliere tra alcune opzioni:

* [Progetta da zero](#design-from-scratch) utilizzando l&#39;editor e-mail visivo

* [Importa il tuo HTML](#import-html) tramite un file HTML o zip

* [Seleziona un modello esistente](#choose-a-template) (uno dei nostri esempi o uno già salvato)

### Creare da zero {#design-from-scratch}

Quando inizi da zero, utilizza le opzioni seguenti per definire il contenuto.

1. Nella pagina _Crea messaggio e-mail_, seleziona **Progetta da zero**.

1. Aggiungi [struttura e contenuto](#add-structure-and-content) alla tua e-mail.

1. Aggiungi [immagini](#add-assets).

1. [Personalizza](#personalize-content) il contenuto.

1. Controlla i collegamenti e [modifica il tracciamento](#edit-url-tracking).

### Importa HTML {#import-html}

Puoi importare contenuti HTML esistenti per progettare i messaggi e-mail. Il contenuto può essere:

* Un file HTML con un foglio di stile incorporato

* Un file .zip che include un file HTML, il foglio di stile (.css) e le immagini

>[!NOTE]
>
>La struttura del file .zip non è soggetta a vincoli. Tuttavia, i riferimenti devono essere relativi e adattarsi alla struttura ad albero della cartella .zip.

1. Nella pagina Progetta modello, seleziona **Importa HTML**.

   SCHERMATA

1. Trascina e rilascia il file HTML o .zip desiderato e fai clic su **Importa**.

   SCHERMATA

>[!NOTE]
>
>Quando il contenuto di HTML viene caricato, il contenuto sarà in modalità di compatibilità. In questa modalità, puoi solo personalizzare il testo, aggiungere collegamenti o aggiungere risorse al contenuto.

Puoi apportare le modifiche desiderate al contenuto importato utilizzando gli [strumenti dell&#39;editor di posta elettronica visivo](#add-structure-and-content).

### Scegli un modello {#choose-a-template}

È possibile scegliere tra due tipi di modelli.

* Modelli di esempio: il Marketo Engage offre quattro modelli e-mail predefiniti.

* Modelli salvati: si tratta di modelli creati da zero utilizzando il menu Modelli o di un messaggio e-mail creato e scelto di salvare come modello.

>[!BEGINTABS]

>[!TAB Modelli di esempio]

Scegli uno dei nostri modelli predefiniti per iniziare subito a utilizzare la progettazione delle e-mail.

1. Nella pagina Crea e-mail, seleziona **Modelli di esempio**.

   SCHERMATA

1. Seleziona il modello desiderato.

   SCHERMATA

1. Viene visualizzata un&#39;anteprima. Per confermare la selezione, fai clic su **Usa questo modello**.

   SCHERMATA

>[!TAB Modelli salvati]

Scegli uno dei modelli creati in precedenza.

1. Nella pagina Crea e-mail, seleziona **Modelli salvati**.

   SCHERMATA

1. Seleziona il modello desiderato.

   SCHERMATA

1. Viene visualizzata un&#39;anteprima. Per confermare la selezione, fai clic su **Usa questo modello**.

   SCHERMATA

>[!ENDTABS]

## Aggiungere struttura e contenuto {#add-structure-and-content}

1. Per iniziare a creare o modificare il contenuto, trascina un elemento da Strutture nell’area di lavoro. Modificane le impostazioni nel riquadro a destra.

   >[!TIP]
   >
   >Seleziona il componente colonna n:n per definire il numero di colonne desiderato (tra tre e 10). Puoi anche definire la larghezza di ciascuna colonna spostando le frecce sotto di essa.

   SCHERMATA

   >[!NOTE]
   >
   >Le dimensioni di ogni colonna non possono essere inferiori al 10% della larghezza totale del componente struttura. È possibile rimuovere solo colonne vuote.

1. Dalla sezione Sommario, trascina gli elementi desiderati e rilasciali in uno o più componenti della struttura.

   SCHERMATA

1. Ogni componente può essere personalizzato tramite le schede Impostazioni o Stile. Modificare il carattere, lo stile del testo, il margine e altro ancora.

SCHERMATA

### Aggiungi Assets {#add-assets}

```
ADD ASSETS OR ADD IMAGES? WHAT OTHER ASSETS CAN YOU ADD?
```

```
Access assets stored in the Assets library. IMAGES AND FILES ONLY?
```

1. Per accedere alle immagini, fai clic sull’icona del selettore delle risorse.

   SCHERMATA

1. Trascina e rilascia l’immagine desiderata in un componente struttura.

   SCHERMATA

   >[!NOTE]
   >
   >Per sostituire un&#39;immagine esistente, selezionala, quindi fai clic su **Seleziona una risorsa** nella scheda Impostazioni a destra.

Fai clic su Abilita contenuto condizione per aggiungere contenuto dinamico e adattare il contenuto ai profili target in base a regole condizionali.



Se necessario, puoi personalizzare ulteriormente l’e-mail facendo clic su Passa all’editor di codice dal menu avanzato. Questo consente di modificare il codice sorgente dell’e-mail, ad esempio per aggiungere tag di tracciamento o HTML personalizzati.

ATTENZIONE
Dopo il passaggio all’editor di codice, non puoi tornare al designer visivo per questo messaggio e-mail.

Una volta che il contenuto è pronto, fai clic sul pulsante Simula contenuto per verificare il rendering. È possibile scegliere la visualizzazione desktop o mobile.

Al termine, fai clic su Salva.

### Livelli, impostazioni e stili {#layers-settings-styles}

```
ARE THEY CALLED LAYERS OR COMPONENTS
```

Apri la struttura di navigazione per accedere a strutture specifiche e alle relative colonne/componenti per una modifica più granulare.

1. Per accedere a, fai clic sull’icona della struttura di navigazione.

SCHERMATA




### Personalizzare il contenuto {#personalize-content}

I token funzionano nel nuovo editor nello stesso modo in cui funzionano nel vecchio, ma l’icona ha un aspetto diverso.

1. Seleziona il componente testo e fai clic sull&#39;icona **Aggiungi personalizzazione**.

   SCHERMATA

1. Fai clic sul tipo di [token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} desiderato.

   SCHERMATA

1. Fai clic su + o ... per aggiungere un token allo spazio vuoto.

   SCHERMATA

   >[!NOTE]
   >
   >&quot;Testo di fallback&quot; è il nuovo termine dell’editor per il valore predefinito. Esempio: ``{{lead.First Name:default=Friend}}``

1. Al termine, fai clic su **Salva**.

### Modifica tracciamento URL {#edit-url-tracking}

A volte è meglio non abilitare l’URL di tracciamento di Marketo su un collegamento all’interno di un’e-mail. Questa funzione è utile quando la pagina di destinazione non supporta i parametri URL e può causare il mancato funzionamento del collegamento.

1. Fai clic sull’icona Collegamenti per visualizzare tutti gli URL nel messaggio e-mail.

   SCHERMATA

1. Fai clic sull’icona a forma di matita per modificare il tracciamento di eventuali collegamenti desiderati.

   SCHERMATA

   ```
   LABEL?
   
   TAGS?
   ```

   <table><tbody>
     <tr>
       <td><b>Traccia senza markt_tok</b></td>
       <td>definizione</td>
     </tr>
     <tr>
       <td><b>Traccia con mkt_tok</b></td>
       <td>definizione</td>
     </tr>
     <tr>
       <td><b>Non tracciare</b></td>
       <td>definizione</td>
     </tr>
   </tbody>
   </table>

1. Al termine, fai clic su **Salva**.

## Controlla avvisi {#check-alerts}

Durante la progettazione del contenuto, gli avvisi vengono visualizzati in alto a destra dello schermo quando mancano le impostazioni chiave.

Esistono due tipi di avvisi:

**Avvisi**

Le avvertenze si riferiscono a consigli e best practice, ad esempio:

* **Il collegamento di rinuncia non è presente nel corpo dell&#39;e-mail**: sebbene i collegamenti di annullamento dell&#39;iscrizione siano un requisito, è consigliabile aggiungerli al corpo dell&#39;e-mail.

>[!NOTE]
>
>L&#39;aggiunta di un&#39;opzione di annullamento dell&#39;abbonamento non è richiesta per [e-mail operative](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md) (non di marketing).

* **La versione di testo di HTML è vuota**: è necessario definire una versione di testo del corpo dell&#39;e-mail per i casi in cui non è possibile visualizzare il contenuto di HTML.

* **Nel corpo dell&#39;e-mail è presente un collegamento vuoto**: verifica che tutti i collegamenti presenti nell&#39;e-mail siano corretti.

* **La dimensione dell&#39;e-mail ha superato il limite di 100 KB**: per una consegna ottimale, assicurati che la dimensione dell&#39;e-mail non superi i 100 KB.

**Errori**

Gli errori impediscono l’invio o il test dell’e-mail finché non vengono risolti:

* **Riga dell&#39;oggetto mancante**: è necessaria una riga dell&#39;oggetto dell&#39;e-mail.

* **La versione e-mail del messaggio è vuota**: questo errore si verifica quando il contenuto dell&#39;e-mail non è stato configurato.

## Verifica l’e-mail

Una volta definito il contenuto del messaggio, puoi utilizzare i profili di test per visualizzarne l’anteprima, inviare bozze e controllare il rendering nei client desktop, mobili e basati su Web più diffusi. Se hai inserito contenuti personalizzati, puoi controllarne la modalità di visualizzazione nel messaggio utilizzando i dati del profilo di test.

Per visualizzare l&#39;anteprima del contenuto dell&#39;e-mail, fai clic su **Simula contenuto**, quindi aggiungi un profilo di test per verificare il messaggio utilizzando i dati del profilo di test.

SCHERMATA

## Fai riferimento a un’e-mail {#reference-an-email}

Dopo aver creato un’e-mail nel nuovo editor, puoi farvi riferimento in Campagne avanzate e/o Elenchi avanzati come faresti con qualsiasi altra e-mail.

* Per farvi riferimento in un elenco avanzato, [segui i soliti passaggi](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md).

* Per farvi riferimento in una campagna avanzata, [segui i soliti passaggi](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

>[!NOTE]
>
>È possibile fare riferimento solo alle e-mail salvate. Nel nuovo editor e-mail non è presente lo stato &quot;approvato&quot;.

>[!MORELIKETHIS]
>
>[Modelli e-mail](/help/marketo/product-docs/email-marketing/general/beta-new-email-editor/email-templates.md){target="_blank"}: scopri come creare, progettare e accedere a un modello e-mail nel nuovo editor.
