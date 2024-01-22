---
description: Glossario SMS - Documentazione Marketo - Documentazione del prodotto
title: Glossario SMS
feature: Mobile Marketing
source-git-commit: efaf34e8113fc6364655ff01aa788aa62bdd31af
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Glossario SMS {#sms-glossary}

Di seguito sono riportati alcuni termini comuni che incontrerai quando utilizzi i messaggi SMS Vibes con il Marketo Engage.

<table>
<thead>
  <tr>
    <th>Termine</th>
    <th>Definizione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Campagna di acquisizione</td>
    <td>Campagna per l’acquisizione di nuovi abbonati agli elenchi di abbonamenti. Un abbonato può essere aggiunto a una campagna di acquisizione tramite un modulo web Marketo o scrivendo un messaggio con una parola chiave.</td>
  </tr>
  <tr>
    <td>Gestione campagne</td>
    <td>Nella piattaforma Vibes, Campaign Manager è il luogo in cui puoi impostare un elenco di abbonamenti e una campagna di acquisizione. Gli utenti con una licenza completa per la piattaforma Vibes possono accedere a ulteriori tipi di campagne.</td>
  </tr>
  <tr>
    <td>Chiave società</td>
    <td>Company_key è un identificatore alfanumerico univoco per il tuo account di piattaforma. Se disponi di più account aziendali nella piattaforma Vibes (ad esempio account figlio), potresti disporre di più company_keys. Ogni istanza del Marketo Engage può essere mappata a una sola Vibes company_key.</td>
  </tr>
  <tr>
    <td>CTA (invito all’azione)</td>
    <td>Segnaletica digitale o fisica o script verbale per acquisire gli abbonati in un programma di messaggi di testo ricorrente o in un elenco di abbonamenti. Possono essere inserite online, sui social media, nelle e-mail, nella stampa, ecc.</td>
  </tr>
  <tr>
    <td>Dominio breve personalizzato</td>
    <td>Se utilizzi il abbreviatore di collegamento Vibes, l’URL abbreviato apparirà, per impostazione predefinita, nell’URL breve Vibes: https://vbs.cm/xxxxxx. Un dominio breve personalizzato è un dominio univoco del tuo marchio. <a href="https://developer-platform.vibes.com/docs/creating-a-custom-short-domain">Ulteriori informazioni sui domini brevi personalizzati</a>.<p>
    Questo vale solo per i messaggi inviati dalla piattaforma Vibes, in particolare per i messaggi della campagna di acquisizione e per i messaggi predefiniti con codice breve.<p>
    Si consiglia l’abbreviazione dell’URL di Marketo per poter inserire i dati di clic nel programma Marketo.</td>
  </tr>
  <tr>
    <td>Messaggi predefiniti</td>
    <td>Messaggi obbligatori per il codice breve per rispondere alle richieste HELP, STOP e di messaggi non riconosciuti.</td>
  </tr>
  <tr>
    <td>Disconnetti</td>
    <td>Le disconnessioni sono una forma di rinuncia a causa della rimozione del numero di cellulare da una rete di gestori. I motivi di una disconnessione includono: un account è stato completamente chiuso, un account prepagato ha esaurito i fondi o il numero è stato rimosso dalla rete di gestori per altri motivi sconosciuti. I numeri di cellulare disconnessi e non trasferiti a un altro operatore di telefonia mobile vengono cancellati da tutti gli elenchi di abbonamenti nella piattaforma Vibes.</td>
  </tr>
  <tr>
    <td>Doppio consenso</td>
    <td>Un metodo di acquisizione che richiede a un potenziale abbonato di confermare il proprio consenso all’aggiunta a un elenco di abbonamenti con un comando di risposta, come "Y" o il proprio codice postale. L’utilizzo di un doppio prompt di consenso può aiutarti a rispettare le linee guida di messaggistica di testo statali e federali.</td>
  </tr>
  <tr>
    <td>Evento</td>
    <td>Un evento è un’occorrenza definita che può essere inviata alla piattaforma Vibes e utilizzata per attivare azioni attivate dall’API, inclusi gli invii di messaggi. Ogni evento contiene dati specifici dell’evento, tra cui un event_type, utilizzato per determinare con quale campagna di messaggi attivata da API corrisponde. L’API Evento può essere attivata tramite Webhook nel Marketo Engage. Per saperne di più <a href="https://developer-platform.vibes.com/reference/event-api">Riferimento API evento</a>.</td>
  </tr>
  <tr>
    <td>Parola chiave</td>
    <td>Una parola breve o una stringa alfanumerica inviata dal consumatore al codice breve per avviare un’esperienza mobile.</td>
  </tr>
  <tr>
    <td>Codice lungo (10DLC)</td>
    <td>Un ID mittente da cui vengono inviati messaggi bidirezionali tra il brand e il consumatore. I codici lunghi USA sono composti da 10 cifre numeriche.</td>
  </tr>
  <tr>
    <td>MDN</td>
    <td>Numero di directory mobile o numero di telefono di una persona. I numeri MDN e di telefono cellulare non sono identificatori univoci in Marketo.</td>
  </tr>
  <tr>
    <td>Database mobile</td>
    <td>Il database mobile è il database in cui vengono memorizzati i dati del sottoscrittore. Ogni abbonato ha un "record persona" univoco, in cui vengono compilati il numero di cellulare ed eventuali campi personalizzati associati.</td>
  </tr>
  <tr>
    <td>Partecipante</td>
    <td>Una persona che ha una o più interazioni mobili (ad esempio l’invio di un messaggio di testo) con il programma mobile, ma non si è iscritta a un elenco di iscrizioni.</td>
  </tr>
  <tr>
    <td>Record persona</td>
    <td>Un record persona è una raccolta di dati per un numero di telefono cellulare specifico. A ogni record persona viene inoltre assegnato un valore person_key univoco per l'identificazione. Gli ID Marketo sono collegati a Vibes utilizzando il campo external_person_id. Ulteriori informazioni sui record delle persone in <a href="https://developer-platform.vibes.com/reference/person-api">Documentazione API di Vibes Person</a>.</td>
  </tr>
  <tr>
    <td>Codice breve</td>
    <td>Un ID mittente da cui vengono inviati messaggi bidirezionali tra il brand e il consumatore. I codici brevi statunitensi sono composti da 5-6 cifre numeriche. I codici brevi canadesi sono composti da 4-6 cifre numeriche. L’integrazione di Marketo LaunchPoint con Vibes supporta un codice breve per istanza.</td>
  </tr>
  <tr>
    <td>SMS</td>
    <td>Servizio messaggi brevi. Questo è un messaggio che include solo testo.</td>
  </tr>
  <tr>
    <td>Elenchi di iscrizioni</td>
    <td>Un elenco di numeri di cellulare (e dei corrispondenti record di persona) che hanno fornito il consenso alla ricezione di messaggi ricorrenti dal programma.</td>
  </tr>
  <tr>
    <td>Abbonato</td>
    <td>Un numero di cellulare iscritto a uno o più elenchi di abbonamenti.</td>
  </tr>
  <tr>
    <td>Piattaforma Vibes</td>
    <td>Il sito web a cui accedi per gestire le campagne. Vai a <a href="https://nexus.us.vibes.com/">https://nexus.us.vibes.com/</a> per accedere alla piattaforma Vibes.</td>
  </tr>
</tbody>
</table>
