---
unique-page-id: 1147108
description: Importare un programma - Documentazione Marketo - Documentazione del prodotto
title: Importare un programma
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
source-git-commit: a64c499f6972e94adfecbe164d86f7db1b1447aa
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# Importare un programma {#import-a-program}

Un programma può essere importato da un abbonamento Marketo a un altro. Ad esempio, puoi creare un programma in una sandbox e importarlo nell’abbonamento live. È inoltre possibile importare un programma predefinito dalla libreria dei programmi Marketo.

## Importare un programma {#import-a-program-1}

1. Vai a **Attività di marketing.**

   ![](assets/ma.png)

1. Fai clic su **Nuovo** a discesa. Seleziona **Programma di importazione**.

   ![](assets/image2014-9-17-12-3a15-3a4.png)

   >[!NOTE]
   >
   >Importazione programma è disponibile solo per gli utenti per i quali è abilitata l’autorizzazione Importa programma. Ulteriori informazioni [gestione di ruoli e autorizzazioni utente](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >Per collegare un account sandbox al tuo abbonamento live, contatta [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Selezionare un Marketo **Abbonamento** e un programma da importare. Fai clic su **Successivo**.

   ![](assets/image2014-9-17-12-3a20-3a13.png)

1. Specifica una **Cartella campagna** per il programma importato. Fai clic su **Avanti.**

   ![](assets/image2014-9-17-12-3a20-3a44.png)

   >[!NOTE]
   >
   >Assicurati **Usa conflitto predefinito** regole selezionate. Le regole di conflitto sono necessarie quando si importano programmi in un’istanza con risorse dello stesso nome.

1. Anteprima dettagli e **Importa** il programma.

   ![](assets/image2014-9-17-12-3a21-3a36.png)

   Viene visualizzata una finestra di dialogo per l’avanzamento dell’importazione del programma.

   ![](assets/image2014-9-17-12-3a21-3a51.png)

Al termine dell’importazione riceverai un messaggio e-mail di conferma.

>[!NOTE]
>
>Sarà necessario riprogrammare le campagne batch importate e attivare le campagne di attivazione. Il sistema disattiva automaticamente le pianificazioni delle campagne e attiva le campagne nel programma importato.

## Identificare i programmi predefiniti nella libreria dei programmi Marketo {#identify-pre-built-programs-in-the-marketo-program-library}

La libreria dei programmi Marketo contiene programmi precompilati e testati che puoi importare nell’abbonamento. I programmi disponibili includono:

1. **Cura Di Base.** Invia una serie di e-mail separate da passaggi di attesa.
1. **Gestione dei dati.** Mantiene l’integrità dei dati tramite campagne intelligenti.
1. **Invia e-mail con pagina di destinazione.** Invia un’e-mail iniziale con un’offerta, ad esempio &quot;scarica questo white paper&quot;. Segue un messaggio e-mail di conferma o di promemoria. Include una pagina di destinazione con un modulo.
1. **E-mail con stato progressivo** Invia un&#39;esplosione di posta con un link tracciabile per la persona da fare clic. Aggiorna lo stato di avanzamento per ogni persona: Inviata, Aperta, Cliccata, ecc.
1. **Momenti Interessanti.** Crea momenti interessanti per il tuo team di vendita per tenerli aggiornati.
1. **Pagina di destinazione con autoresponder.** Utilizza i contenuti scaricabili per ottenere nuove persone e nutrirle. Include pagine di destinazione e moduli.
1. **Ciclo di vita 2.** Utilizza il punteggio per spostare una persona da nuova a qualificata per il marketing.
1. **Modello E-Mail Mobile.** Un modello e-mail reattivo è stato testato su iPhone e Android. Alcune versioni di Android, MS Outlook, Exchange e applicazioni di terze parti come Gmail e Yahoo! Le app mobile di posta non supportano il CSS richiesto per i modelli reattivi. È consigliabile eseguire il test prima di inviare le e-mail.
1. **Programma Importazione Sweepstakes.** Programma Sweepstakes per quelli che provano la Biblioteca Programma! È sufficiente approvare le e-mail e la pagina di destinazione e attivare la campagna avanzata. Quindi visualizza la pagina di destinazione approvata, compila il modulo e immetti!
1. **Campagne disponibili per le vendite.** Fornisce ai tuoi rappresentanti commerciali un modo per eseguire campagne avanzate Marketo da un dashboard nel tuo CRM.
1. **Punteggio - Spark Edition.** Punteggio demografico e comportamentale acquisito in un singolo campo di punteggio. Include più di due dozzine di campagne relative al punteggio.
1. **Punteggio - Standard e Seleziona edizioni.** Punteggio demografico e comportamentale acquisito in campi di punteggio separati. Include più di due dozzine di campagne relative al punteggio.
1. **Sincronizza nuove persone con CRM.** La campagna che sincronizza nuove persone nel tuo sistema CRM. Assegna uno stato di persona in modo che venga riconosciuto come non pronto per le vendite.
1. **Webinar con adattatore evento.** Un set completo di e-mail, ad esempio inviti e promemoria, oltre a pagine di destinazione con moduli e campagne per lo spostamento delle persone all’interno del programma. Questo programma ottiene aggiornamenti su registrazione, frequenza, ecc. da provider di eventi online come WebEx.
1. **Webinar senza adattatore evento.** Come sopra, ma con i processi manuali per la registrazione, la frequenza, ecc.
1. **Programma di valutazione delle decisioni siriane**. Questo programma è progettato per supportare il modello standard di valutazione delle decisioni di Sirius, incluse le regole di valutazione implicite ed esplicite e l&#39;assegnazione di persone con corrispondenza.

>[!CAUTION]
>
>È necessario creare due campi personalizzati (&quot;Punteggio demografico&quot; e &quot;Punteggio comportamentale&quot;) prima di importare il programma Punteggio - Standard &amp; Select Editions.

## Impatto sulle attività esterne durante le importazioni del programma {#impact-on-external-assets-during-program-imports}

I programmi utilizzano risorse esterne come modelli e-mail, modelli di pagina di destinazione, immagini, moduli, token e tag di programma. È possibile configurare la modalità di gestione dei modelli di pagina di destinazione e dei tag di programma e Marketo gestisce automaticamente il resto.

**Modelli di pagina di destinazione/e-mail:** I modelli e-mail/pagina di destinazione vengono importati in Design Studio. È possibile utilizzare regole di conflitto per configurare il comportamento quando esiste un modello con lo stesso nome. Utilizzando la regola predefinita, a un modello verrà aggiunto un numero se ne esiste uno con lo stesso nome. Ad esempio, se disponi già di un modello denominato &quot;Modello standard&quot;, il nuovo verrà denominato &quot;Modello standard - 1&quot;.

**Pagine di destinazione/Forms:** Se in Design Studio esiste un modulo o una pagina di destinazione con lo stesso nome, verranno comunque importati, ma con un numero aggiunto al nome (ad esempio: Pagina di destinazione - 1).

**Immagini:** Le immagini utilizzate dalle pagine di destinazione vengono importate nello studio di progettazione, a meno che non ne esista una con lo stesso nome.

**Token:** I token che risiedono al di fuori di un programma verranno convertiti in token locali durante il processo di importazione.

>[!CAUTION]
>
>I token di tipo immagine non sono supportati per le importazioni di programmi. Se viene importato un programma con tipo immagine, i miei token **no** passeranno dei token.

**Tag del programma:** È possibile utilizzare regole di conflitto per controllare il modo in cui verranno trattati i tag di programma non esistenti nell&#39;account di destinazione. Utilizzando la regola predefinita verranno creati i tag del programma oppure è possibile scegliere di ignorarli.

>[!CAUTION]
>
>Durante l’importazione di un programma, invia e-mail/pagine di destinazione che contengono [contenuto dinamico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) verranno saltate.
