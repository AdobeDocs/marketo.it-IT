---
solution: Marketo Engage
product: marketo
title: TITOLO
description: Scopri come creare e gestire le linee guida per il brand.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: e0e739054c6389e0a3ab638097491e6c24f5e30c
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 9%

---

# Creare e gestire i brand personali {#brands}

>[!AVAILABILITY]
>
>Prima di poter utilizzare l&#39;Assistente di intelligenza artificiale in Adobe Marketo Engage, devi accettare il [contratto utente](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"}. Per ulteriori informazioni, contatta il team account di Adobe (il tuo account manager).

Le linee guida per il marchio sono un set dettagliato di regole e standard che stabiliscono l’identità visiva e verbale di un marchio. Essi fungono da riferimento per mantenere una rappresentazione coerente del marchio su tutte le piattaforme di marketing e comunicazione.

In [!DNL Marketo Engage], ora puoi inserire e organizzare manualmente i dettagli del tuo marchio o caricare documenti di linee guida per l&#39;estrazione automatica delle informazioni.

## Accedere ai brand {#generative-access}

Per accedere al menu **[!UICONTROL Brands]** in [!DNL Adobe Marketo Engage], è necessario concedere agli utenti le autorizzazioni **[!UICONTROL Manage brand kit]** o **[!UICONTROL Enable AI assistant]**. COLLEGAMENTO ULTERIORI INFORMAZIONI

+++  Scopri come assegnare le autorizzazioni relative al brand

Per assegnare le autorizzazioni per i brand, effettua le seguenti operazioni:

1. Nel prodotto **Autorizzazioni**, passa alla scheda **Ruoli** e seleziona il **Ruolo** desiderato.

1. Fai clic su **Modifica** per modificare le autorizzazioni.

1. Aggiungi la risorsa **Assistente AI**, quindi seleziona **Gestisci brand kit** o **[!UICONTROL Enable Ai assistant]** dal menu a discesa.

   Si noti che l&#39;autorizzazione **[!UICONTROL Enable Ai assistant]** fornisce accesso in sola lettura al menu **[!UICONTROL Brands]**.

   SCHERMATA

1. Fai clic su **Salva** per applicare le modifiche.

   Le autorizzazioni degli utenti già assegnati a questo ruolo verranno aggiornate automaticamente.

1. Per assegnare questo ruolo a nuovi utenti, passa alla scheda **Utenti** nella dashboard **Ruoli** e fai clic su **Aggiungi utente**.

1. Immetti il nome o l’indirizzo e-mail dell’utente o sceglilo dall’elenco e fai clic su **Salva**.

1. Se l’utente non è già stato creato in precedenza, consulta [questa documentazione](https://experienceleague.adobe.com/it/docs/experience-platform/access-control/abac/permissions-ui/users).

+++

## Creazione e gestione del brand {#create-brand-kit}

Per creare e gestire la linea guida del brand, puoi inserire i dettagli personalmente o caricare il documento di linee guida del brand per estrarre automaticamente le informazioni:

1. Nel menu **[!UICONTROL Brands]**, fare clic su **[!UICONTROL Create brand]**.

   SCHERMATA

1. Immetti **[!UICONTROL Name]** per il tuo marchio.

1. Trascina e rilascia o seleziona il file per caricare le linee guida per il brand ed estrarre automaticamente le informazioni rilevanti per il brand. Fai clic su **[!UICONTROL Create brand]**.

   Il processo di estrazione delle informazioni ora inizia. Il completamento potrebbe richiedere alcuni minuti.

   SCHERMATA

1. I contenuti e gli standard di creazione visiva vengono ora compilati automaticamente. Sfoglia le diverse schede per adattare le informazioni in base alle esigenze. [Ulteriori informazioni](#personalize)

1. Dal menu avanzato di ogni sezione o categoria, puoi aggiungere riferimenti per estrarre automaticamente le informazioni rilevanti sul brand.

   Per rimuovere il contenuto esistente, utilizzare le opzioni **[!UICONTROL Clear section]** o **[!UICONTROL Clear category]**.

   SCHERMATA

1. Una volta configurata, fai clic su **[!UICONTROL Save]**, quindi su **[!UICONTROL Publish]** per rendere disponibile la linea guida del brand in AI Assistant.

1. Per apportare modifiche al tuo marchio pubblicato, fai clic su **[!UICONTROL Edit brand]**.

   >[!NOTE]
   >
   >In questo modo viene creata una copia temporanea in modalità di modifica, che sostituisce la versione live pubblicata.

   SCHERMATA

1. Dal dashboard **[!UICONTROL Brands]**, apri il menu avanzato facendo clic sull&#39;icona BLANK per:

   * Visualizza marchio
   * Modifica
   * Duplica
   * Pubblica
   * Annulla pubblicazione
   * Elimina

   SCHERMATA

Le linee guida del tuo marchio sono ora accessibili dal menu a discesa **[!UICONTROL Brand]** di AI Assistant, che consente di generare contenuti e risorse in linea con le tue specifiche. Ulteriori informazioni su AI Assistant - COLLEGAMENTO

SCHERMATA

### Imposta un marchio predefinito {#default-brand}

Puoi designare un marchio predefinito da applicare automaticamente durante la generazione del contenuto e il calcolo dei punteggi di allineamento durante la creazione della campagna.

Per impostare un marchio predefinito, vai al tuo dashboard **[!UICONTROL Brands]**. Aprire il menu avanzato facendo clic sull&#39;icona ![](assets/do-not-localize/Smock_More_18_N.svg) e selezionare **[!UICONTROL Mark as default brand]**.

SCHERMATA

## Personalizzare il brand {#personalize}

### Informazioni sul brand {#about-brand}

Utilizza la scheda **[!UICONTROL About the brand]** per stabilire l&#39;identità di base del tuo marchio, delineandone lo scopo, la personalità, la tagline e altri attributi di definizione.

1. Per iniziare, compila le informazioni fondamentali per il tuo marchio nella categoria **[!UICONTROL Key details]**:

   * **[!UICONTROL Brand Kit Name]**: immettere il nome del kit del marchio.

   * **[!UICONTROL When to Use]**: specificare scenari o contesti in cui applicare il kit del brand.

   * **[!UICONTROL Brand Name]**: immettere il nome ufficiale del marchio.

   * **[!UICONTROL Brand Description]**: fornire una panoramica di ciò che questo brand rappresenta.

   * **[!UICONTROL Default Tagline]**: aggiungi la tagline principale associata al brand.

   SCHERMATA

1. Nella categoria **[!UICONTROL Guiding principles]**, chiarisci la direzione e la filosofia di base del tuo marchio:

   * **[!UICONTROL Mission]**: descrive in dettaglio lo scopo del tuo marchio.

   * **[!UICONTROL Vision]**: Descrivere l&#39;obiettivo a lungo termine o lo stato futuro desiderato.

   * **[!UICONTROL Market Positioning]**: Spiega in che modo il tuo marchio è posizionato sul mercato.

   SCHERMATA

1. Dalla categoria **[!UICONTROL Core brand values]**, fai clic su &quot;Aggiungi icona&quot; per aggiungere i valori principali del brand e inserire i dettagli:

   * **[!UICONTROL Value]**: assegna un nome al valore del marchio principale.

   * **[!UICONTROL Description]**: Spiega cosa significa questo valore per il tuo marchio.

   * **[!UICONTROL Behaviors]**: delineare le azioni o gli atteggiamenti che riflettono questo valore nella pratica.

   * **[!UICONTROL Manifestations]**: fornisci esempi di come questo valore è espresso nel branding reale.

   SCHERMATA

1. Se necessario, fai clic sull’icona &quot;Modifica&quot; per aggiornare o eliminare uno dei valori del brand di base.

   SCHERMATA

Ora puoi personalizzare ulteriormente il tuo marchio o [pubblicare il tuo marchio](#create-brand-kit).

### Stile di scrittura {#writing-style}

La sezione **[!UICONTROL Writing style]** illustra gli standard per la scrittura dei contenuti, specificando in che modo il linguaggio, la formattazione e la struttura devono essere utilizzati per mantenere la chiarezza, la coerenza e la coerenza in tutti i materiali.

+++ Categoria ed esempi disponibili

<table>
  <thead>
    <tr>
      <th>Categoria</th>
      <th>Sottocategoria</th>
      <th>Esempio di linee guida</th>
      <th>Esempio di esclusioni</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="4">Standard per la creazione di contenuti</td>
      <td>Standard di messaggistica del marchio</td>
      <td>Innovazione e messaggistica personalizzata.</td>
      <td>Non esagerare con le funzionalità dei prodotti.</td>
    </tr>
    <tr>
      <td>Utilizzo tag</td>
      <td>Posiziona la tagline sotto il logo su tutte le risorse di marketing digitale.</td>
      <td>Non modificare o tradurre la tagline.</td>
    </tr>
    <tr>
      <td>Messaggistica di base</td>
      <td>Enfatizzare la dichiarazione dei principali vantaggi, ad esempio una maggiore produttività.</td>
      <td>Non utilizzare proposte di valore non correlate.</td>
    </tr>
    <tr>
      <td>Standard di denominazione</td>
      <td>Utilizza nomi semplici e descrittivi come "ProScheduler".</td>
      <td>Non utilizzare termini complessi o caratteri speciali.</td>
    </tr>
    <tr>
      <td rowspan="5">Stile di comunicazione del marchio</td>
      <td>Caratteristiche di brand personality</td>
      <td>Amichevole e accessibile.</td>
      <td>Non essere disfattista.</td>
    </tr>
    <tr>
      <td>Meccanica di scrittura</td>
      <td>Mantieni le frasi brevi e di impatto.</td>
      <td>Non usare un gergo eccessivo.</td>
    </tr>
    <tr>
      <td>Tono situazionale</td>
      <td>Mantenere un tono professionale nelle comunicazioni di crisi.</td>
      <td>Non essere sprezzante nelle comunicazioni di supporto.</td>
    </tr>
    <tr>
      <td>Linee guida per la scelta di Word</td>
      <td>Usa parole come "innovativo" e "intelligente".</td>
      <td>Evita parole come "economico" o "hack".</td>
    </tr>
    <tr>
      <td>Standard linguistici</td>
      <td>Segui le convenzioni inglesi americane.</td>
      <td>Non mescolare ortografia britannica con quella americana.</td>
    </tr>
    <tr>
      <td rowspan="3">Standard di conformità legale</td>
      <td>Norme sui marchi</td>
      <td>Utilizza sempre il simbolo ™ o ®.</td>
      <td>Non omettere i simboli legali quando necessario.</td>
    </tr>
    <tr>
      <td>Standard di copyright</td>
      <td>Includi avvisi di copyright sul materiale di marketing.</td>
      <td>Non utilizzare contenuti di terze parti senza autorizzazione.</td>
    </tr>
    <tr>
      <td>Standard disclaimer</td>
      <td>Visualizzare le liberatorie in modo leggibile sulle risorse digitali.</td>
      <td>Non nascondere le liberatoria in aree non visibili.</td>
    </tr>
</table>

+++

</br>

Per personalizzare **[!UICONTROL Writing Style]**:

1. Dalla scheda **[!UICONTROL Writing Style]**, fare clic su ![](assets/do-not-localize/Smock_Add_18_N.svg) per aggiungere una linea guida, un&#39;eccezione o un&#39;esclusione.

1. Immettere la linea guida, l&#39;eccezione o l&#39;esclusione e fare clic su **[!UICONTROL Add]**.

   SCHERMATA

1. Seleziona una linea guida o un’esclusione da aggiornare o eliminare.

1. Fai clic su Modifica per modificare l’esempio o sull’icona Elimina per eliminarlo.

   SCHERMATA

Ora puoi personalizzare ulteriormente il tuo marchio o [pubblicare il tuo marchio](#create-brand-kit).

### Contenuto visivo {#visual-content}

La sezione **[!UICONTROL Visual Content]** definisce gli standard per le immagini e il design, specificando le specifiche necessarie per mantenere un aspetto del marchio unificato e coerente.

+++ Categorie ed esempi disponibili

<table>
  <thead>
    <tr>
      <th>Categoria</th>
      <th>Esempio di linee guida</th>
      <th>Esempio di esclusioni</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Standard per la fotografia</td>
      <td>Utilizza l'illuminazione naturale per le riprese in esterni.</td>
      <td>Evita le immagini eccessivamente modificate o con pixel.</td>
    </tr>
    <tr>
      <td>Standard illustrazione</td>
      <td>Utilizza stili puliti e minimalisti.</td>
      <td>Evita di essere troppo complessi.</td>
    </tr>
    <tr>
      <td>Icona standard</td>
      <td>Utilizza un sistema di griglia a 24 px coerente.</td>
      <td>Non combinare le dimensioni delle icone, non utilizzare pesi di traccia incoerenti o non discostarsi dalle regole della griglia.</td>
    </tr>
    <tr>
      <td>Linee guida sull’utilizzo</td>
      <td>Scegliete uno stile di vita che rifletta i clienti reali che usano il prodotto in ambienti professionali.</td>
      <td>Non utilizzare immagini che contraddicono il tono del marchio o che appaiono fuori contesto.</td>
    </tr>
</table>

+++

</br>

Per personalizzare **[!UICONTROL Visual content]**:

1. Dalla scheda **[!UICONTROL Visual content]**, fare clic su VUOTO per aggiungere una linea guida, un&#39;esclusione o un esempio.

1. Immettere la linea guida, l&#39;esclusione o l&#39;esempio e fare clic su **[!UICONTROL Add]**.

   SCHERMATA

1. Per aggiungere un&#39;immagine che mostra l&#39;utilizzo corretto, selezionare **[!UICONTROL Example]** e fare clic su **[!UICONTROL Select image]**. È inoltre possibile aggiungere un’immagine che mostra un utilizzo errato come esempio di esclusione.

   SCHERMATA

1. Seleziona una linea guida o un’esclusione da aggiornare o eliminare.

1. Seleziona una linea guida o un’esclusione per aggiornarla. Fai clic sull’icona &quot;Elimina&quot; per eliminarla.

   SCHERMATA

Ora puoi personalizzare ulteriormente il tuo marchio o [pubblicare il tuo marchio](#create-brand-kit).
