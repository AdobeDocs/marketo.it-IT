---
description: Una guida dettagliata per la creazione di una campagna e-mail in CX Enterprise Collaborator, dalla scrittura delle richieste alla revisione e all’esportazione della campagna.
title: Creare e generare campagne e-mail
source-git-commit: b58edb707bf68aeed9f1b5eba8328c54a95c5a2f
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Creare e generare campagne e-mail {#build-and-generate-email-campaigns}

Scopri come creare e rivedere in pochi minuti campagne e-mail complete.

## Prima di iniziare

Assicurati di avere:

* Un account CX Enterprise Worker attivo ([registratevi qui](https://coworker-essentials.experience.adobe.com/), se non lo avete già fatto).

* Il tuo marchio è configurato in **La tua roba** > **Marchi**.

* (Facoltativo ma consigliato) Un modello e-mail di HTML caricato in **Le tue cose** > **Modelli e-mail**.

* Un CSV di pubblico pronto per il caricamento.

* Un’idea chiara dell’obiettivo della campagna (ad esempio, &quot;riconquistare clienti inattivi&quot;, &quot;invitare utenti di prova a un webinar&quot;).

>[!TIP]
>
>Se non hai ancora scritto i prompt per le campagne di marketing, impiega due minuti per ignorare _Richiedere a CX Enterprise Collaborator: best practice_ prima di iniziare.

## Passaggio 1: avviare una nuova chat

Dalla pagina Home puoi iniziare in tre modi:

* Digitate un prompt nella barra centrale dei prompt.
* Seleziona un modello di campagna pronto dalla sezione modelli sotto la barra dei prompt.
* Utilizzare un&#39;opzione &quot;Help me prompt&quot; dal menu a discesa nella barra dei prompt per fare in modo che CX Enterprise Worker ti guidi durante la scrittura del prompt.

[SCHERMATA: Home page con barra dei prompt, riga del modello e opzione &quot;Help me prompt&quot; evidenziata]

[PER KEITH: Breve descrizione di ciascuna opzione e quando usarla. Suggerisci modelli per i nuovi utenti, richieste in formato libero per gli addetti al marketing che sanno cosa desiderano e &quot;Chiedi assistenza&quot; per chiunque nel periodo compreso tra.]

## Passaggio 2: scrivi la richiesta

Un forte prompt di CX Enterprise Workker include:

* L’obiettivo della campagna (cosa stai cercando di raggiungere).
* Il pubblico (per chi o da dove provengono i dati del pubblico).
* Formato e struttura (numero di e-mail, cadenza, tono).
* Indicazioni sul marchio o sul contesto (riferimenti al marchio, al prodotto o alla campagna).

Esempio:

```
"Create a win-back email series for customers who bought last year but haven't returned. Use the CSV I uploaded. Include 2–3 emails that feel seasonal and remind them to shop again."
```

[PER KEITH: può aggiungere altri 2-3 esempi di prompt che si estendono su B2B e B2C per dare varietà. Estrai i casi d&#39;uso dal documento della raccolta per coerenza.]

[SCHERMATA: barra di richiesta con il prompt di esempio digitato in]

## Passaggio 3: caricare il pubblico

[PER KEITH: procedura dettagliata per il caricamento CSV. Copertina: - Posizione del pulsante Carica nell’interfaccia utente. : colonne obbligatorie e aspettative relative al formato. - Campi di personalizzazione che CX Enterprise Collaborator può utilizzare (nome, data dell&#39;ultimo ordine, categoria del prodotto, ecc.). : collegamento al file CSV di esempio. - Cosa succede se i dati sono disordinati o se mancano dei campi.]

[SCHERMATA: flusso di caricamento CSV]

>[!TIP]
>
>Escludi eventuali contatti che non desideri inviare tramite e-mail (utenti non abbonati, indirizzi interni, account di test) prima di caricarli. Anche se attiveremo progressivamente la funzionalità per &quot;escludere&quot; utenti specifici o &quot;aggiungere attributi&quot; durante il corso della prova, non sarà immediatamente disponibile dalla data di lancio.

## Passaggio 4: aggiungere una breve descrizione e materiale di riferimento

&lbrack;FOR KEITH: Spiega come allegare una breve documentazione di riferimento sul brand o altro contesto. Copertina: - Tipi di file supportati. - il modo in cui CX Enterprise Collaborator utilizza queste informazioni (estratte nel contesto del prompt, applicate alla generazione di contenuti, ecc.). - Limiti di dimensione del file, se presenti

Ecco un approfondimento della mia sessione al summit dove affronto questo tema: https://business.adobe.com/it/summit/2026/sessions/3-2-1-launch-project-halo-revealed-s232.html\
Limitazioni - Posso collegarvi con l&#39;engg - Neha Pullabhotla, che sarà in grado di aiutarci su specifiche qui. &rbrack;

[SCHERMATA: breve/riferimento allegato interfaccia utente]

## Passaggio 5: generare la campagna

Fai clic su **Genera campagna**. CX Enterprise Collaborator:

* Genera un piano di campagna strutturato.
* Chiedi il pubblico di destinazione, che verrà utilizzato anche per la personalizzazione dei contenuti.
* Crea contenuti e-mail personalizzati per ogni passaggio.
* Costruire dinamicamente il percorso lungo il percorso.
* Assemblalo tutto su una singola bacheca della campagna.

[PER KEITH: descrizione dell&#39;aspetto e dei contenuti della bacheca della campagna. Coprire la vista piano, la vista percorso e la vista contenuto. Tieni presente quanto può durare in genere la generazione, che dipende dal numero di punti di contatto nel loro percorso. Chiama che quando aprono un editor per il flusso di lavoro o per l’e-mail, sono conversazione li mostrerà in modo che siano nel contesto del componente specifico, come l’editor e-mail è un editor e-mail point &amp; click con la limitazione che non è destinato ad essere un designer a tutti gli effetti, gli utenti possono modificare le immagini in Adobe Express o anche connettersi a Google Drive o AEM Assets utilizzando Adobe Express, Tutte le loro risorse di immagini sono memorizzate in Express, rigenerare le immagini all’interno del nostro editor e-mail con Firefly in linea, o sostituirle con un’immagine locale dal loro computer. Possono cambiare il modello di HTML e rigenerare il contenuto, e infine inviarsi un&#39;e-mail di prova per convalidare ciò che il cliente finale riceverà]

[SCHERMATA: scheda Campaign generata con piano, percorso e contenuto visibili]

## Passaggio 6: rivedere e perfezionare

L’interfaccia conversazionale consente un perfezionamento semplice. Per apportare modifiche, contattare CX Enterprise Collaborator:

* &quot;Rendi più urgente l’oggetto dell’e-mail 2.&quot;
* &quot;Abbrevia la copia del corpo in tutte le e-mail.&quot;
* &quot;Scambia il pubblico con i clienti solo della regione occidentale.&quot;
* &quot;Aggiungi una quarta e-mail con un CTA più forte.&quot;
* &quot;Cambia l’attesa da 3 giorni a 5 giorni.&quot;

[PER KEITH: scopri come apportare modifiche sia tramite chat che tramite modifica diretta. Spiega in che modo gli artefatti vengono aggiornati. Non esiste alcuna possibilità di aggiungere altri nodi al flusso di lavoro tramite l’editor, né attualmente esiste il controllo delle versioni. Per ottenere i migliori risultati, li invitiamo anche a richiedere qualsiasi modifica per il flusso di lavoro complessivo all&#39;inizio della creazione del piano]

[SCHERMATA: ottimizzazione conversazionale in azione — mostra un prima e dopo di un&#39;e-mail dopo una richiesta di chat]

## Passaggio 7: inviare un’e-mail di bozza

Prima del lancio, invia la campagna a te stesso o a un membro del tuo team per la revisione in una vera e propria casella in entrata.

[PER KEITH: passaggi per l&#39;invio di una bozza. Copertina: - Dove si trova il pulsante bozza. - Chi può ricevere le bozze (attualmente solo l’utente connesso - Indica se vengono inviate tutte le e-mail del percorso o solo una alla volta (attualmente solo 1 alla volta, a meno che l’utente non dica &quot;bozza questa serie&quot; nella chat. - Cosa verificare nella bozza (rendering, collegamenti, token di personalizzazione, piè di pagina per annullare l&#39;abbonamento).]

[SCHERMATA: invia flusso bozza]

## Passaggio 8: avviare o esportare

Quando sei soddisfatto della campagna, hai alcune opzioni:

>[!NOTE]
>Launch non è attualmente disponibile al momento del rilascio, ma verrà abilitato entro due settimane dalla versione iniziale, in attesa dell’autorizzazione legale.

* Avvia la campagna.
* Esporta singole e-mail come HTML.
* Esporta l’intera campagna come documento Word o PDF per la revisione del team.

[PER KEITH: Dettagli su ciascuna opzione ed eventuali controlli pre-avvio eseguiti da CX Enterprise Collaborator (conformità, collegamenti interrotti, campi di personalizzazione mancanti, ecc.).]

[SCHERMATA: opzioni di avvio/esportazione]

## Domande comuni

&lbrack;PER KEITH: Domande frequenti 4-6 basate sul feedback ricevuto dagli utenti in anticipo. Suggerimenti per iniziare - per discutere con il nostro team Eng:
* &quot;Perché la prima risposta richiede così tanto tempo?
* &quot;E se l&#39;output di CX Enterprise Collaborator non fosse corretto?&quot;
* &quot;Posso modificare le e-mail direttamente o solo tramite chat?&quot;
* &quot;Come posso salvare una campagna senza avviarla?&quot;
* &quot;Cosa succede se il file CSV del mio pubblico contiene errori?&quot;
* &quot;Posso duplicare o eseguire il remix di una campagna?&quot;
* &quot;Come posso condividere una bozza di campagna con un compagno di squadra per la revisione?&quot;&rbrack;
