---
description: Una guida dettagliata per la creazione di una campagna e-mail in CX Enterprise Collaborator, dalla scrittura delle richieste alla revisione e all’esportazione della campagna.
title: Creare e generare campagne e-mail
source-git-commit: 8750337464744e2684bef91d70caa4abcefdcc8c
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Creare e generare campagne e-mail {#build-and-generate-email-campaigns}

Scopri come creare e rivedere in pochi minuti campagne e-mail complete.

## Prima di iniziare

Assicurati di avere:

* Un account CX Enterprise Worker attivo ([registratevi qui](https://coworker-essentials.experience.adobe.com/){target="_blank"}, se non lo avete già fatto).

* Il tuo marchio è configurato in **La tua roba** > **Marchi**.

* (Facoltativo ma consigliato) Un modello e-mail di HTML caricato in **Le tue cose** > **Modelli e-mail**.

* Un CSV di pubblico pronto per il caricamento.

* Un’idea chiara dell’obiettivo della campagna (ad esempio, &quot;riconquistare clienti inattivi&quot; o &quot;invitare utenti di prova a un webinar&quot;).

## Passaggio 1: avviare una nuova chat

Dalla pagina Home puoi iniziare in tre modi:

**Opzione uno**: digitare un prompt nella barra dei prompt centrale.

_Quando utilizzare: quando si conosce esattamente ciò che si desidera._

Opzione 2: scegli un modello pronto dalla sezione **Modelli campagna** sotto la barra dei prompt.

_Quando utilizzare: quando non si è sicuri di dove iniziare._

Opzione tre: utilizzare l&#39;opzione &quot;Help me prompt&quot; dal menu a discesa nella barra dei prompt per fare in modo che CX Enterprise Collaborator ti guidi durante la scrittura del prompt.

_Quando utilizzare: è possibile avere un&#39;idea di ciò che si desidera, ma si desidera ricevere un piccolo aiuto._

[SCHERMATA: Home page con barra dei prompt, riga del modello e opzione &quot;Help me prompt&quot; evidenziata]

![](assets/generate-email-campaigns-.png)

## Passaggio 2: creare la richiesta

Un forte prompt di CX Enterprise Workker include:

* L’obiettivo della campagna (cosa stai cercando di raggiungere).
* Il pubblico (per chi o da dove provengono i dati del pubblico).
* Formato e struttura (numero di e-mail, cadenza, tono).
* Indicazioni sul marchio o sul contesto (riferimenti al marchio, al prodotto o alla campagna).

Esempio:

<pre style="white-space: pre-wrap;">
"Crea una serie e-mail di riconquista per i clienti che hanno acquistato l’anno scorso ma non sono tornati. Utilizza il file CSV che ho caricato. Includi 2-3 e-mail che sembrano stagionali e ricordano di fare acquisti di nuovo."
</pre>

>[!TIP]
>
>Per ulteriori esempi, consulta l&#39;articolo _Casi d&#39;uso_.

[SCHERMATA: barra di richiesta con il prompt di esempio digitato in]

![](assets/generate-email-campaigns-.png)

## Passaggio 3: caricare il pubblico

[PER KEITH: procedura dettagliata per il caricamento CSV. Copertina: - Posizione del pulsante Carica nell’interfaccia utente. : colonne obbligatorie e aspettative relative al formato. - Campi di personalizzazione che CX Enterprise Collaborator può utilizzare (nome, data dell&#39;ultimo ordine, categoria del prodotto, ecc.). : collegamento al file CSV di esempio. - Cosa succede se i dati sono disordinati o se mancano dei campi.]

[SCHERMATA: flusso di caricamento CSV]

![](assets/generate-email-campaigns-.png)

>[!TIP]
>
>Escludi eventuali contatti che non desideri inviare tramite e-mail (utenti non abbonati, indirizzi interni, account di test) prima di caricarli. Anche se attiveremo progressivamente la funzionalità per &quot;escludere&quot; utenti specifici o &quot;aggiungere attributi&quot; durante il corso della prova, non sarà immediatamente disponibile dalla data di lancio.

## Passaggio 4: aggiungere una breve descrizione e materiale di riferimento

&lbrack;FOR KEITH: Spiega come allegare una breve documentazione di riferimento sul brand o altro contesto. Copertina: - Tipi di file supportati. - il modo in cui CX Enterprise Collaborator utilizza queste informazioni (estratte nel contesto del prompt, applicate alla generazione di contenuti, ecc.). - Limiti di dimensione del file, se presenti

Ecco un approfondimento della mia sessione al summit dove affronto questo tema: https://business.adobe.com/it/summit/2026/sessions/3-2-1-launch-project-halo-revealed-s232.html\
Limitazioni - Posso collegarvi con l&#39;engg - Neha Pullabhotla, che sarà in grado di aiutarci su specifiche qui. &rbrack;

[SCHERMATA: breve/riferimento allegato interfaccia utente]

![](assets/generate-email-campaigns-.png)

## Passaggio 5: generare la campagna

Fai clic su **Genera campagna**. CX Enterprise Collaborator:

* Genera un piano di campagna strutturato.
* Chiedi il pubblico di destinazione, che verrà utilizzato anche per la personalizzazione dei contenuti.
* Crea contenuti e-mail personalizzati per ogni passaggio.
* Costruire dinamicamente il percorso lungo il percorso.
* Assemblalo tutto su una singola bacheca della campagna.

[PER KEITH: descrizione dell&#39;aspetto e dei contenuti della bacheca della campagna. Coprire la vista piano, la vista percorso e la vista contenuto. Tieni presente quanto può durare in genere la generazione, che dipende dal numero di punti di contatto nel loro percorso. Chiama che quando aprono un editor per il flusso di lavoro o per l’e-mail, sono conversazione li mostrerà in modo che siano nel contesto del componente specifico, come l’editor e-mail è un editor e-mail point &amp; click con la limitazione che non è destinato ad essere un designer a tutti gli effetti, gli utenti possono modificare le immagini in Adobe Express o anche connettersi a Google Drive o AEM Assets utilizzando Adobe Express, Tutte le loro risorse di immagini sono memorizzate in Express, rigenerare le immagini all’interno del nostro editor e-mail con Firefly in linea, o sostituirle con un’immagine locale dal loro computer. Possono cambiare il modello di HTML e rigenerare il contenuto, e infine inviarsi un&#39;e-mail di prova per convalidare ciò che il cliente finale riceverà]

[SCHERMATA: scheda Campaign generata con piano, percorso e contenuto visibili]

![](assets/generate-email-campaigns-.png)

## Passaggio 6: rivedere e perfezionare

L’interfaccia conversazionale consente un perfezionamento semplice. Per apportare modifiche, contattare CX Enterprise Collaborator:

* &quot;Rendi più urgente l’oggetto dell’e-mail 2.&quot;
* &quot;Abbrevia la copia del corpo in tutte le e-mail.&quot;
* &quot;Scambia il pubblico con i clienti solo della regione occidentale.&quot;
* &quot;Aggiungi una quarta e-mail con un CTA più forte.&quot;
* &quot;Cambia l’attesa da 3 giorni a 5 giorni.&quot;

[PER KEITH: scopri come apportare modifiche sia tramite chat che tramite modifica diretta. Spiega in che modo gli artefatti vengono aggiornati. Non esiste alcuna possibilità di aggiungere altri nodi al flusso di lavoro tramite l’editor, né attualmente esiste il controllo delle versioni. Per ottenere i migliori risultati, li invitiamo anche a richiedere qualsiasi modifica per il flusso di lavoro complessivo all&#39;inizio della creazione del piano]

[SCHERMATA: ottimizzazione conversazionale in azione - mostra un prima e dopo di un&#39;e-mail dopo una richiesta di chat]

![](assets/generate-email-campaigns-.png)

## Passaggio 7: inviare un’e-mail di bozza

Prima del lancio, invia la campagna a te stesso o a un membro del tuo team per la revisione in una vera e propria casella in entrata.

[PER KEITH: passaggi per l&#39;invio di una bozza. Copertina: - Dove si trova il pulsante bozza. - Chi può ricevere le bozze (attualmente solo l’utente connesso - Indica se vengono inviate tutte le e-mail del percorso o solo una alla volta (attualmente solo 1 alla volta, a meno che l’utente non dica &quot;bozza questa serie&quot; nella chat. - Cosa verificare nella bozza (rendering, collegamenti, token di personalizzazione, piè di pagina per annullare l&#39;abbonamento).]

[SCHERMATA: invia flusso bozza]

![](assets/generate-email-campaigns-.png)

## Passaggio 8: avviare o esportare

Quando sei soddisfatto della campagna, hai alcune opzioni:

>[!AVAILABILITY]
>
>Launch non è disponibile nella versione iniziale, ma l’attivazione è prevista per la fine di giugno. Controlla qui per gli aggiornamenti.

* Avvia la campagna.
* Esporta singole e-mail come HTML.
* Esporta l’intera campagna come documento Word o PDF per la revisione del team.

[PER KEITH: Dettagli su ciascuna opzione ed eventuali controlli pre-avvio eseguiti da CX Enterprise Collaborator (conformità, collegamenti interrotti, campi di personalizzazione mancanti, ecc.).]

[SCHERMATA: opzioni di avvio/esportazione]

![](assets/generate-email-campaigns-.png)

## Domande comuni

&lbrack;PER KEITH: Domande frequenti 4-6 basate sul feedback ricevuto dagli utenti in anticipo. Suggerimenti per iniziare - per discutere con il nostro team Eng:
* &quot;Perché la prima risposta richiede così tanto tempo?
* &quot;E se l&#39;output di CX Enterprise Collaborator non fosse corretto?&quot;
* &quot;Posso modificare le e-mail direttamente o solo tramite chat?&quot;
* &quot;Come posso salvare una campagna senza avviarla?&quot;
* &quot;Cosa succede se il file CSV del mio pubblico contiene errori?&quot;
* &quot;Posso duplicare o eseguire il remix di una campagna?&quot;
* &quot;Come posso condividere una bozza di campagna con un compagno di squadra per la revisione?&quot;&rbrack;
