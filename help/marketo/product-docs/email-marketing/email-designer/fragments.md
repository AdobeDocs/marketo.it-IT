---
solution: Marketo Engage
product: marketo
title: Frammenti
description: Scopri come creare e utilizzare frammenti di contenuto visivo come componenti riutilizzabili per e-mail e modelli e-mail.
level: Beginner, Intermediate
exl-id: abc065a0-cd2f-4f0f-a5f2-228b833b99a8
source-git-commit: 76d854176c3c462596596689b43d3567517fee63
workflow-type: tm+mt
source-wordcount: '1909'
ht-degree: 0%

---

# Frammenti

Un frammento è un componente riutilizzabile a cui è possibile fare riferimento in uno o più modelli e-mail e e-mail. In genere si tratta di un blocco di contenuto (testo, immagine o entrambi) che può essere inserito rapidamente nel progetto. Con questa funzionalità, puoi precreare più blocchi di contenuto personalizzati per assemblare il contenuto delle e-mail e migliorare così il processo di progettazione. I casi d’uso comuni includono blocchi di contenuto di intestazione/piè di pagina per e-mail, banner di invito di eventi, messaggi stagionali e altro ancora.

Per utilizzare al meglio i frammenti nei flussi di lavoro:

* _Crea frammenti_ - Crea frammenti visivi da zero o salvando il contenuto come frammento dall&#39;editor di contenuti visivi.
* _Riutilizza frammenti_ - Puoi utilizzarli nel contenuto per il numero di volte necessario.

## Frammenti visivi {#visual-fragments}

I frammenti visivi sono blocchi visivi predefiniti creati (utilizzando l’editor di contenuto visivo) che puoi riutilizzare in più e-mail o modelli e-mail.

## Accedere e gestire i frammenti {#access-and-manage-fragments}

Per accedere ai frammenti visivi, vai a **Design Studio** in Marketo Engage. Nell&#39;albero a sinistra fare clic su **[!UICONTROL Frammenti (nuovi)]**.

![Frammenti di accesso](assets/access-and-manage-fragments-1.png){width="600" zoomable="yes"}

Per impostazione predefinita, la tabella è ordinata in base alla colonna _[!UICONTROL Modificato]_. Fare clic sui titoli di altre colonne per modificare l&#39;ordinamento della tabella. Fai di nuovo clic sullo stesso titolo per passare da crescente a decrescente.

### Trova e filtra

Utilizza la barra di ricerca per trovare un frammento in base al nome. Fai clic sull&#39;icona _Filtro_ ( ![Icona Filtro](assets/icon-filter.svg) ) per visualizzare le opzioni di filtro disponibili e scegliere le impostazioni desiderate.

![Filtra i frammenti visualizzati](assets/access-and-manage-fragments-2.png){width="700" zoomable="yes"}

### Personalizzare le colonne {#customize-the-column-display}

Personalizza le colonne da visualizzare nella tabella facendo clic sull&#39;icona _Personalizza tabella_ ( ![Personalizza icona tabella](assets/icon-column-settings.svg) ) in alto a destra.

Selezionare le colonne desiderate e fare clic su **[!UICONTROL Applica]**.

![Personalizza tabella modale](assets/access-and-manage-fragments-3.png){width="400" zoomable="yes"}

### Stato del frammento {#fragment-status}

Lo stato del frammento determina la sua disponibilità per l’utilizzo in un’e-mail o in un modello e-mail e le modifiche che puoi apportare.

<table>
<tbody>
  <tr>
    <td width="25%"><b>Bozza</b></td>
    <td width="75%">Quando crei un frammento, questo si trova nello stato Bozza. La bozza rimane tale fino a quando non la pubblichi per l’utilizzo in un messaggio e-mail o in un modello e-mail.
    <p>Azioni disponibili:
    <li>Modifica tutti i dettagli</li>
    <li>Modifica in designer visivo</li>
    <li>Pubblica</li>
    <li>Duplica</li>
    <li>Elimina</li>
  </td>
  <tr>
    <td><b>Pubblicato</b></td>
    <td>Quando pubblichi un frammento, questo diventa disponibile per l’utilizzo in un’e-mail o in un modello e-mail. Il contenuto del frammento pubblicato non può essere modificato nella finestra di progettazione visiva.
    <p>Azioni disponibili:
    <li>Modifica descrizione</li>
    <li>Aggiungi a un messaggio e-mail o a un modello</li>
    <li>Crea bozza di versione</li>
    <li>Duplica</li>
    <li>Elimina (se non in uso)</li>
    </td>
  </tr>
  <tr>
    <td style="width:25%"><b>Pubblicato con bozza</b></td>
    <td style="width:75%">Quando crei una bozza da un frammento pubblicato, la versione pubblicata rimane disponibile per l’utilizzo in un modello e-mail o e-mail e il contenuto della bozza può essere modificato nella finestra di progettazione visiva. Se si pubblica la bozza della versione, questa sostituirà la versione pubblicata corrente e il contenuto verrà aggiornato in <i>tutti</i> i modelli e-mail e le e-mail in cui è in uso. 
    <p>Azioni disponibili:
    <li>Modifica descrizione</li>
    <li>Aggiungi a un messaggio e-mail o a un modello</li>
    <li>Modifica versione bozza in Progettazione visiva</li>
    <li>Pubblica versione bozza</li>
    <li>Duplica</li>
    <li>Elimina (se non in uso)</li>
    </td>
  </tr>
</tbody>
</table>

## Creare i frammenti {#create-fragments}

1. Per creare un nuovo frammento visivo, fare clic su **[!UICONTROL Crea frammento]** in alto a destra nella pagina dell&#39;elenco dei frammenti.

   ![Pulsante Crea frammento](assets/create-fragments-1.png){width="700" zoomable="yes"}

1. Assegna al frammento un **[!UICONTROL Nome]** e una **[!UICONTROL Descrizione]** facoltativa.

   _Requisiti del frammento_

   * Nome: massimo 100 caratteri, deve essere univoco, senza distinzione tra maiuscole e minuscole
   * Descrizione: massimo 300 caratteri
   * Caratteri: i caratteri alfa, numerici e speciali sono ammessi
   * I caratteri riservati sono **_non consentiti_**: `\ / : * ? " < > |`

   ![Crea frammento modale](assets/create-fragments-2.png){width="400" zoomable="yes"}

1. Fai clic su **[!UICONTROL Crea]**.

   ![Crea frammento modale](assets/create-fragments-3.png){width="400" zoomable="yes"}

   >[!NOTE]
   >
   >Impossibile modificare il tipo **Type** di un frammento in questo momento.

   La finestra di progettazione visiva viene aperta con un&#39;area di lavoro vuota.

1. Utilizza gli [strumenti di progettazione del contenuto](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#add-structure-and-content){target="_blank"} per creare il contenuto del frammento visivo.

1. Fai clic su **[!UICONTROL Salva]** in qualsiasi momento per salvare la bozza del frammento.

1. Quando sei pronto a rendere il frammento disponibile per l&#39;utilizzo in un messaggio e-mail o in un modello e-mail, fai clic su **[!UICONTROL Pubblica]**.

## Visualizza dettagli frammento {#view-fragment-details}

Fai clic sul nome di un frammento nella pagina dell’elenco per aprire la pagina dei dettagli del frammento. Puoi scegliere di modificare il frammento, rinominarlo o aggiornarne la descrizione. Effettuare gli aggiornamenti e fare clic all&#39;esterno del campo del nome o della descrizione per salvare le modifiche.

>[!NOTE]
>
>Se un frammento pubblicato è utilizzato da un’e-mail o da un modello e-mail, non puoi modificarne il nome o il contenuto. Puoi creare una versione bozza se desideri apportare modifiche al frammento.

![Visualizza dettagli per un frammento pubblicato](assets/view-fragment-details-1.png){width="600" zoomable="yes"}

Fai clic su **[!UICONTROL Modifica frammento]** per aprire il frammento nell&#39;editor di contenuti visivi.

Uscire dalla visualizzazione in qualsiasi momento facendo clic sulla freccia _Indietro_ in alto a sinistra, per tornare alla pagina dell&#39;elenco _Frammenti_.

## Visualizza frammento utilizzato da riferimenti {#view-fragment-used-by-references}

Nella pagina dei dettagli del frammento, fai clic sulla scheda **[!UICONTROL Usato da]** per visualizzare i dettagli sulla posizione in cui il frammento viene utilizzato in Marketo Engage.

>[!IMPORTANT]
>
>Non è possibile eliminare un frammento attualmente utilizzato da un’e-mail o da un modello e-mail.

![Utilizzato dai riferimenti per il frammento](assets/view-fragment-used-by-1.png){width="600" zoomable="yes"}

Fai clic sul collegamento per aprire l’e-mail o il modello e-mail corrispondente in cui viene utilizzato il frammento.

## Elimina frammenti {#delete-fragments}

Poiché non è possibile eliminare un frammento attualmente utilizzato da un messaggio e-mail o da un modello e-mail, controlla i riferimenti _used-by_ prima di avviare la rimozione di un frammento. Inoltre, una rimozione non può essere annullata, pertanto controlla prima di avviare un’azione di eliminazione.

Puoi eliminare un frammento utilizzando uno dei seguenti metodi:

* Dai dettagli del frammento a destra, fai clic su **[!UICONTROL Elimina]**.
* Nella pagina dell&#39;elenco _[!UICONTROL Frammenti]_, fare clic sui puntini di sospensione accanto al frammento e scegliere **[!UICONTROL Elimina]**.

Questa azione apre una finestra di dialogo di conferma. È possibile interrompere il processo facendo clic su **[!UICONTROL Annulla]** oppure su **[!UICONTROL Elimina]** per confermare l&#39;eliminazione.

![Finestra di dialogo Elimina frammento](assets/fragment-delete-dialog.png){width="400"}

## Modificare i frammenti {#edit-fragments}

Le modifiche apportate a un frammento dipendono dal suo stato corrente:

* Quando un frammento è nello stato _Bozza_, puoi modificarne i dettagli e il contenuto visivo.
* Quando un frammento è nello stato _Pubblicato_, puoi modificare la descrizione del frammento, ma non il nome. Non è possibile modificare il contenuto visivo.
* Quando un frammento è in stato _Pubblicato con bozza_, la modifica dei dettagli è limitata alla descrizione. Puoi anche modificare il contenuto visivo della versione bozza.

>[!BEGINTABS]

>[!TAB Bozza]

1. Nella pagina dell&#39;elenco _[!UICONTROL Frammenti]_ fare clic sul nome del frammento per aprirlo.

   Viene visualizzata un’anteprima del contenuto visivo, con i dettagli del frammento a destra.

1. Apportare le modifiche desiderate.

   ![Dettagli per frammento con stato Bozza](assets/fragment-draft-details.png){width="600" zoomable="yes"}

1. Per apportare modifiche al contenuto nella finestra di progettazione visiva, fare clic su **[!UICONTROL Modifica frammento]**. Al termine, fai clic su **Salva**.

1. Fai clic su **[!UICONTROL Salva]** o **[!UICONTROL Salva e chiudi]** per tornare ai dettagli del frammento.

1. Se desideri rendere il frammento disponibile per l&#39;utilizzo in un messaggio e-mail o in un modello e-mail, fai clic su **[!UICONTROL Pubblica]**.

>[!TAB Pubblicato]

1. Nella pagina dell&#39;elenco _[!UICONTROL Frammenti]_ fare clic sul nome del frammento per aprirlo.

   Viene visualizzata un’anteprima del contenuto visivo, con i dettagli del frammento a destra.

1. Se necessario, modifica la descrizione.

   Per un frammento pubblicato, non è possibile modificare tutti gli altri dettagli.

1. Se desideri aggiornare il contenuto, fai clic su **[!UICONTROL Crea versione bozza]** in alto a destra.

   Fare clic su **[!UICONTROL OK]** nella finestra di dialogo per aprire la versione bozza nella finestra di progettazione visiva. Se necessario, è possibile modificare `image source` KG - LINK HERE.

   ![Finestra di dialogo Crea bozza versione](assets/fragments-create-draft-version.png){width="300"}

1. Fai clic su **[!UICONTROL Salva]** o **[!UICONTROL Salva e chiudi]** per tornare ai dettagli del frammento.

1. Se desideri rendere il frammento disponibile per l&#39;utilizzo in un messaggio e-mail o in un modello e-mail, fai clic su **[!UICONTROL Pubblica]**.

>[!NOTE]
>
>Quando pubblichi la versione bozza, questa sostituisce la versione pubblicata corrente e il contenuto viene aggiornato nelle e-mail e nei modelli e-mail in cui è già in uso.

>[!TAB Pubblicato con bozza]

Esistono due modi per aprire la versione bozza per la modifica dalla pagina di elenco _[!UICONTROL Frammenti]_:

* Fai clic sull&#39;icona _Altro_ (**...**) accanto al nome del frammento e scegli **[!UICONTROL Apri versione bozza]**.

  ![Apri versione bozza](assets/fragments-create-draft-version.png){width="300"}

* Fai clic sul nome del frammento per aprirlo. Quindi, fai clic su **[!UICONTROL Apri versione bozza]** in alto a destra.

Viene visualizzata un’anteprima del contenuto visivo per la versione bozza, con i dettagli del frammento a destra.

Per aggiornare il contenuto:

1. Fai clic su **[!UICONTROL Modifica frammento]** in alto a destra. Al termine, fai clic su **Salva**.

1. Fai clic su **[!UICONTROL Salva]** o **[!UICONTROL Salva e chiudi]** per tornare ai dettagli del frammento.

1. Se desideri rendere il frammento disponibile per l&#39;utilizzo in un messaggio e-mail o in un modello e-mail, fai clic su **[!UICONTROL Pubblica]**.

>[!NOTE]
>
>Quando pubblichi la versione bozza, questa sostituisce la versione pubblicata corrente e il contenuto viene aggiornato nelle e-mail e nei modelli e-mail in cui è già in uso.

>[!ENDTABS]

## Frammenti duplicati {#duplicate-fragments}

Puoi duplicare un frammento utilizzando uno dei seguenti metodi:

* Dalla pagina dell&#39;elenco _[!UICONTROL Frammenti]_, fai clic sull&#39;icona _Altro_ (**...**) accanto al nome del frammento e scegli **[!UICONTROL Duplica]**.
* Nella parte superiore destra della pagina dei dettagli del frammento, fare clic su **[!UICONTROL ... Altro]** e scegli **[!UICONTROL Duplicato]**.

![Duplica il frammento](assets/fragment-details-duplicate.png){width="600" zoomable="yes"}

Nella finestra di dialogo, inserisci un nome univoco e una descrizione facoltativa. Fai clic su **[!UICONTROL Duplica]**.

![Immettere un nome e una descrizione per il frammento duplicato](assets/fragment-duplicate-dialog.png){width="400"}

Il frammento duplicato viene quindi visualizzato nell&#39;elenco _Frammenti_.

## Salvare un nuovo frammento da e-mail o contenuto del modello {#save-a-new-fragment-from-email-or-template-content}

Quando crei/modifichi un modello e-mail o e-mail nell’editor di contenuto visivo, puoi salvare tutto o parte del contenuto come frammento per riutilizzarlo.

1. Per salvare il contenuto come frammento, fare clic su **[!UICONTROL Altro]** e scegliere **[!UICONTROL Salva come frammento]**.

1. Seleziona i diversi elementi da includere nel frammento.

   Selezionare più strutture tenendo premuto il pulsante Maiusc o Ctrl.

   È possibile selezionare solo strutture adiacenti.

1. Con il contenuto selezionato, fai clic su **[!UICONTROL Crea]** in alto a destra.

1. Nella finestra di dialogo, immetti un nome e una descrizione facoltativa per il frammento e fai clic su **[!UICONTROL Crea]**.

Il frammento viene quindi visualizzato nella pagina di elenco _Frammenti_ ed è disponibile per l&#39;utilizzo nelle e-mail e nei modelli e-mail.

## Aggiungere frammenti visivi all’e-mail o al contenuto del modello {#add-visual-fragments-to-your-email-or-template-content}

I frammenti sono progettati per essere riutilizzati. Puoi aggiungerne fino a 30 in un e-mail o modello e-mail e nidificarli fino a un solo livello.

* [Aggiungere un frammento a un messaggio e-mail](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#add-fragments)

* [Aggiungere un frammento a un modello e-mail](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#add-fragments)

Il contenuto del frammento viene aggiornato dinamicamente all’interno della struttura per eseguire il rendering di un’immagine del modo in cui il contenuto viene visualizzato nell’e-mail.

>[!TIP]
>
>Se desideri che il frammento occupi l&#39;intero layout orizzontale all&#39;interno del messaggio e-mail, aggiungi una struttura di [!UICONTROL 1:1 colonna], quindi trascina e rilascia il frammento al suo interno.

Dopo il salvataggio, il modello e-mail/e-mail viene visualizzato nella pagina dei dettagli del frammento quando viene selezionata la scheda _[!UICONTROL Usato da]_. I frammenti aggiunti non sono modificabili nell’e-mail o nel modello, il frammento di origine pubblicato definisce il contenuto.

## Azioni sui frammenti durante l’authoring di e-mail e modelli {#fragment-actions-during-email-and-template-authoring}

Quando un frammento viene aggiunto a un e-mail o a un modello e-mail, il relativo contenuto non può essere modificato all’interno dell’e-mail o del modello. Tuttavia, puoi applicare le seguenti azioni:

* **[!UICONTROL Elimina]** - Rimuove il frammento dal contenuto del modello e-mail o e-mail corrente (l&#39;origine del frammento non è interessata).
* **[!UICONTROL Aggiorna]** - Aggiorna il contenuto del frammento nel modello e-mail o e-mail corrente. L’aggiornamento è utile quando desideri riflettere eventuali modifiche recenti apportate al frammento dopo l’aggiunta all’e-mail o al modello e-mail.
* **[!UICONTROL Duplicato]** - Questo duplica il frammento nello stesso modello e-mail o e-mail all&#39;interno dell&#39;editor. Il frammento duplicato viene aggiunto immediatamente sotto l’originale.
* **[!UICONTROL Apri frammento]** - Verrà aperta una nuova scheda del browser con la pagina e i dettagli dell&#39;editor frammenti.
* **[!UICONTROL Interrompi ereditarietà]** - Interrompe l&#39;ereditarietà del frammento (e delle relative modifiche) dall&#39;origine. Utilizza questa azione per rendere il contenuto del frammento disponibile come contenuto indipendente e modificabile all’interno del modello e-mail o e-mail. Questa azione rimuove anche il modello e-mail o e-mail dal riferimento _Usato da_ per il frammento originale.

Quando selezioni il frammento nella pagina dell’editor, queste azioni sono disponibili nella barra degli strumenti contestuale e nel pannello delle proprietà a destra.

![Applica azioni al frammento selezionato](assets/fragment-actions-email-authoring.png){width="600" zoomable="yes"}
