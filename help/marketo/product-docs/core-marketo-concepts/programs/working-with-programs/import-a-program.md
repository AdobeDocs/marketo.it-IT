---
unique-page-id: 1147108
description: Importa un programma - Documenti Marketo - Documentazione prodotto
title: Importare un programma
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 0%

---


# Importa un programma {#import-a-program}

Un programma può essere importato da un’iscrizione a Marketo a un’altra. Ad esempio, potete creare un programma in una sandbox e importarlo nell&#39;abbonamento live. È inoltre possibile importare un programma pregenerato dalla libreria dei programmi Marketo.

## Importa un programma {#import-a-program-1}

1. Vai a **Attività di marketing.**

   ![](assets/ma.png)

1. Fare clic **Nuovo **a discesa. Selezionare **Importa programma**.

   ![](assets/image2014-9-17-12-3a15-3a4.png)

   >[!NOTE]
   >
   >Importazione programma è disponibile solo per gli utenti che hanno attivato i ruoli con l&#39;autorizzazione Importa programma. Ulteriori informazioni sulla [gestione di ruoli utente e autorizzazioni](../../../../product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >
   >Per collegare un account sandbox al tuo abbonamento live, contatta il [Supporto marketing](http://www.marketo.com/services/support/).

1. Selezionare un&#39;iscrizione **Marketing** e un programma da importare. Fare clic su **Next**.

   ![](assets/image2014-9-17-12-3a20-3a13.png)

1. Specificate una **cartella campagna** per il programma importato. Fare clic su **Avanti.**

   ![](assets/image2014-9-17-12-3a20-3a44.png)

   >[!NOTE]
   >
   >Assicurarsi che** ****Usa regole di conflitto predefinite** sia selezionato. Le regole di conflitto sono necessarie quando si importano programmi in un&#39;istanza con risorse dello stesso nome.

1. Visualizza in anteprima i dettagli e **Importa** il programma.

   ![](assets/image2014-9-17-12-3a21-3a36.png)

   Viene visualizzata una finestra di dialogo con l’avanzamento dell’importazione del programma.

   ![](assets/image2014-9-17-12-3a21-3a51.png)

Al termine dell’importazione, riceverete un messaggio e-mail di conferma.

>[!NOTE]
>
>Sarà necessario riprogrammare le campagne batch importate e attivare le campagne di attivazione. Il sistema disattiva automaticamente i programmi delle campagne e attiva le campagne nel programma importato.

## Identificare i programmi pregenerati nella libreria dei programmi di Marketo {#identify-pre-built-programs-in-the-marketo-program-library}

La libreria del programma Marketo contiene programmi preconfigurati e testati che puoi importare nell&#39;abbonamento. I programmi disponibili includono:

1. **Nurture di base.** Invia una serie di e-mail separate da passaggi di attesa.
1. **Gestione dei dati.** Mantiene l&#39;integrità dei dati mediante campagne intelligenti.
1. **E-mail con pagina di destinazione.** Invia un messaggio e-mail iniziale con un&#39;offerta, ad esempio &quot;scarica il white paper&quot;. Segue un messaggio e-mail di conferma o promemoria. Include una pagina di destinazione con un modulo.
1. **E-mail con stato progressione.** Invia un messaggio di posta elettronica con un collegamento tracciabile per la persona su cui fare clic. Aggiorna lo stato di progressione per ogni persona - Inviata, Aperta, Cliccata, ecc.
1. **Momenti Interessanti.** Crea momenti interessanti per il tuo team di vendita per mantenerli aggiornati.
1. **Pagina di destinazione con autoresponder.** Utilizzate contenuti scaricabili per ottenere nuove persone e svilupparle. Include pagine di destinazione e moduli.
1. **Ciclo di vita 2.** Utilizza il punteggio per spostare una persona da nuova a qualificata per il marketing.
1. **Modello e-mail per dispositivi mobili.** Un modello e-mail reattivo è stato testato su iPhone e Android. Alcune versioni di app Android, MS Outlook, Exchange e di terze parti come Gmail e Yahoo! Le app mobili di posta non supportano il CSS richiesto per i modelli reattivi. È consigliabile eseguire il test prima di inviare le e-mail.
1. **Programma Import Sweepstakes.** Programma Sweepstakes per chi prova la Biblioteca dei Programmi! È sufficiente approvare le e-mail e la pagina di destinazione e attivare la campagna intelligente. Visualizzate la pagina di destinazione approvata, compilate il modulo e immettete il testo.
1. **Campagne di vendita disponibili.** Offre ai tuoi agenti di vendita un modo per eseguire campagne smart Marketo da un dashboard in CRM.
1. **Punteggio - Spark Edition.** Punteggio demografico e comportamentale acquisito in un singolo campo di punteggio. Include più di due dozzine di campagne relative al punteggio.
1. **Punteggio - Standard &amp; Select Editions.** Punteggio demografico e comportamentale acquisito in campi di punteggio separati. Include più di due dozzine di campagne relative al punteggio.
1. **Sincronizza nuove persone con CRM.** La campagna che sincronizza nuove persone con il sistema CRM. Assegna uno stato a una persona in modo che venga riconosciuta come non pronta per le vendite.
1. **Webinar con adattatore evento.** Una serie completa di e-mail, ad esempio inviti e promemoria, oltre a pagine di destinazione con moduli e campagne per l&#39;indirizzamento delle persone attraverso il programma. Questo programma ottiene aggiornamenti su registrazione, partecipazione, ecc. da provider di eventi online come WebEx.
1. **Webinar senza adattatore evento.** Come sopra, ma con processi manuali per la registrazione, la partecipazione, ecc.
1. **Programma** di Punteggio Decisioni Sirius. Questo programma è costruito per supportare il modello standard di valutazione delle decisioni di Sirius, incluse le regole di punteggio implicite ed esplicite e l&#39;assegnazione di persona matrixed. Per ulteriori informazioni, vedere [questo PDF](http://docs.marketo.com/display/docs/assets/sirius-decisions-scoring-program-overview.pdf).

>[!CAUTION]
>
>È necessario creare due campi personalizzati (&quot;Punteggio demografico&quot; e &quot;Punteggio comportamentale&quot;) prima di importare il programma Scoring - Standard &amp; Select Editions.

## Impatto sulle risorse esterne durante le importazioni del programma {#impact-on-external-assets-during-program-imports}

I programmi utilizzano risorse esterne come i modelli e-mail, i modelli delle pagine di destinazione, le immagini, i moduli, i token e i tag dei programmi. È possibile configurare il modo in cui vengono gestiti i modelli e i tag dei programmi delle pagine di destinazione e Marketo gestisce automaticamente gli altri.

**Modelli e-mail: **I modelli e-mail vengono importati automaticamente e creati a meno che non ne esista uno con lo stesso nome.

**Modelli pagina di destinazione: **I modelli delle pagine di destinazione vengono importati nello studio di progettazione. Potete utilizzare le regole di conflitto per configurare il comportamento quando esiste un modello con lo stesso nome. Utilizzando la regola predefinita, un numero viene aggiunto a un modello di pagina di destinazione se ne esiste uno con lo stesso nome. Ad esempio, se esiste un modello di pagina di destinazione denominato Standard Template 1, verrà creato un modello di pagina di destinazione denominato Standard Template 1.

**Immagini: **Le immagini utilizzate dalle pagine di destinazione vengono importate nello studio di progettazione a meno che non ne esista una con lo stesso nome.

**Token: **I token che vivono al di fuori di un programma saranno convertiti in token locali durante il processo di importazione.

>[!CAUTION]
>
>Tipo di immagine I miei token non sono supportati per le importazioni di programmi. Se viene importato un programma che ha un tipo di immagine, i token **no **i verranno utilizzati.

**Tag programma: **È possibile utilizzare regole di conflitto per controllare come verranno trattati i tag di programma che non esistono nell&#39;account di destinazione. Utilizzando la regola predefinita verranno creati i tag dei programmi, oppure sarà possibile scegliere di ignorare i tag.  **Forms: **I moduli esterni vengono importati automaticamente nello studio di progettazione, a meno che non ne esista uno con lo stesso nome.

>[!CAUTION]
>
>Durante l&#39;importazione di un programma, le pagine/e-mail di destinazione contenenti [contenuto dinamico](http://docs.marketo.com/x/yRAt) verranno ignorate.

## Guarda il video {#watch-a-video}

`<iframe width="630" height="470" src="//play.vidyard.com/KgvZssZ9WRkZgDsY1yZfms.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`