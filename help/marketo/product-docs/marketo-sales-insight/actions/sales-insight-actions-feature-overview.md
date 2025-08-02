---
description: Panoramica delle funzioni Azioni di vendita di Insight - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica sulla funzione Azioni di Insight per le vendite
exl-id: 059de248-d1a2-42cd-a7ec-f10b15d0b526
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1305'
ht-degree: 0%

---

# Panoramica sulla funzione Azioni di Insight per le vendite {#msi-actions-feature-overview}

Accelera le attività di ricerca di potenziali clienti con strumenti di marketing e coinvolgimento riuniti in un unico flusso di lavoro utilizzando le azioni di vendita Insight.

>[!NOTE]
>
>Marketo Sales Insight Actions è un&#39;applicazione basata su Web che si integra esclusivamente con Salesforce CRM tramite il [pacchetto Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. A volte viene chiamato &quot;Vendite Marketo&quot; o semplicemente &quot;Azioni&quot;.

Per una panoramica video delle azioni di Sales Insight, [fai clic qui](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/sales-insight-actions/overview.html){target="_blank"}.

![](assets/sales-insight-actions-feature-overview-1.png)

## Layout lead e layout contatto {#lead-layout-and-contact-layout}

Le seguenti azioni sono disponibili dal menu a discesa &quot;Scegli azioni&quot; nella navigazione superiore:

* Invia e-mail vendite
   * Le e-mail di vendita hanno un monitoraggio di visualizzazione, clic e risposta (quando il canale di consegna è configurato)
   * Include e-mail Personalization, firma personalizzata e allegati
   * Condivisione di modelli e rapporti
   * Condivisione team, e-mail di gruppo e capacità CC/CCN
   * L’attività e-mail di vendita verrà registrata nel record persona di Marketo
   * Filtri e trigger corrispondenti nelle campagne Marketo Smart (dettagli di seguito)

* Aggiungi a campagna di vendita
   * Aggiungi lead ai playbook di vendita, ovvero una sequenza di e-mail e attività
   * Include l’accesso e la condivisione del team, la generazione di attività, il salto dei fine settimana, l’eliminazione delle e-mail fuori sede come risposte e la fine automatica
   * L’attività della campagna verrà registrata nel record persona di Marketo
   * Filtri e trigger corrispondenti nelle campagne Marketo Smart (dettagli di seguito)

* Chiamata di vendita
   * Effettuare chiamate di vendita utilizzando il selettore all&#39;interno del CRM
   * Include presenza locale, preregistrata
   * Registra il risultato della chiamata, la registrazione delle chiamate nel pannello e la cronologia delle attività
   * L’attività di chiamata verrà registrata nel record persona di Marketo
   * Filtri e attivatori nelle campagne Marketo Smart

* Aggiungi attività
   * Crea e-mail, chiamate, InMail e attività personalizzate per i lead
   * Automatizzare la creazione di attività con le campagne di vendita
   * Sincronizza attività con [!DNL Salesforce]
   * Registra le attività nella sezione Cronologia attività [!DNL Salesforce]

Per accedere ai feed live, fai clic sull’icona ((0)) nel menu di navigazione in alto. Include la possibilità di visualizzare aggiornamenti live sulle attività di vendita e funzionalità di ancoraggio dello schermo.

![](assets/sales-insight-actions-feature-overview-2.png)

I seguenti dati sono disponibili nelle schede all’interno del pannello MSI:

* Dashboard approfondimenti
   * La griglia Velocity del coinvolgimento includerà le attività da e-mail di vendita, azioni della campagna di vendita e chiamata di vendita
   * Prossime campagne di vendita: quando un lead fa parte di una campagna in corso, queste informazioni saranno disponibili nella scheda Prossime campagne di vendita
   * Attività future: quando è prevista un’attività relativa a un lead, queste informazioni saranno disponibili nella scheda Attività successive

* Scheda E-mail
   * Tutte le e-mail di vendita inviate verranno registrate qui. Le attività verranno anche registrate nel record persona di Marketo
   * Le colonne includono Oggetto, Apri, Clic, Risposta (disponibile solo per e-mail di vendita con canale di consegna impostato), Mittente, Data
   * Include la scheda di presentazione con dettagli aggiuntivi come Mittente, Modello, Campagna di vendita e Anteprima e-mail

* Scheda Chiamata
   * Tutte le chiamate effettuate utilizzando la funzione di chiamata di vendita verranno registrate qui. Le attività verranno anche registrate nel record persona di Marketo
   * Le colonne includono Nome, Risultato, Note, Chiamata, Durata e collegamento alla registrazione
   * Include una scheda a tendina con dettagli aggiuntivi come Chiamata effettuata da, Chiamata con risposta da, Numero di telefono e Stato

## Layout account e opportunità {#account-and-opportunity-layout}

Nella barra di navigazione superiore sono disponibili le seguenti azioni:

* Invia e-mail di vendita: possibilità di inviare e-mail di gruppo personalizzate o con modelli con visualizzazione, tracciamento dei clic e delle risposte a tutti i contatti associati a un account/opportunità
   * Le e-mail di vendita hanno un monitoraggio di visualizzazione, clic e risposta (quando il canale di consegna è configurato)
   * Include e-mail Personalization, firma personalizzata e allegati
   * Condivisione di modelli e rapporti
   * Condivisione team, e-mail di gruppo e capacità CC/CCN
   * L’attività e-mail di vendita verrà registrata nel record persona di Marketo
   * Filtri e trigger corrispondenti nelle campagne Marketo Smart (dettagli di seguito)

* Aggiungi a campagna di vendita: consente di aggiungere ai playbook di vendita tutti i contatti associati a un account/opportunità, ovvero una sequenza di e-mail e attività.
   * Aggiungi lead ai playbook di vendita, ovvero una sequenza di e-mail e attività
   * Include l’accesso e la condivisione del team, la generazione di attività, il salto dei fine settimana, l’eliminazione delle e-mail fuori sede come risposte e la fine automatica
   * L’attività della campagna verrà registrata nel record persona di Marketo
   * Filtri e trigger corrispondenti nelle campagne Marketo Smart (dettagli di seguito)

Per accedere ai feed live, fai clic sull’icona ((0)) nel menu di navigazione in alto. Include la possibilità di visualizzare aggiornamenti live sulle attività di vendita e funzionalità di ancoraggio dello schermo.

Nelle schede sono disponibili i seguenti dati:

* Dashboard approfondimenti
   * Velocity Grid includerà le attività da e-mail di vendita, azioni della campagna di vendita e la chiamata di vendita
   * Prossime campagne di vendita: quando un contatto dell’account/opportunità fa parte di una campagna in corso, queste informazioni saranno disponibili nella scheda Prossime campagne di vendita
   * Attività future: quando un’attività futura riguarda un contatto dell’account/opportunità, queste informazioni saranno disponibili nella scheda Attività successive

* Scheda E-mail
   * Tutte le e-mail di vendita inviate ai contatti dall’account/opportunità verranno registrate qui. Le attività verranno anche registrate nel record persona di Marketo
   * Le colonne includono Oggetto, Apri, Clic, Risposta (disponibile solo per e-mail di vendita con canale di consegna impostato), Mittente e Data
   * Include la scheda di presentazione con dettagli aggiuntivi come Mittente, Modello, Campagna di vendita e Anteprima e-mail

* Scheda Chiamata
   * Tutte le chiamate effettuate ai contatti dall&#39;account/opportunità utilizzando la funzione di chiamata di vendita verranno registrate qui. Le attività verranno anche registrate nel record persona di Marketo
   * Le colonne includono Nome, Risultato, Note, Chiamata, Durata e collegamento alla registrazione
   * Include una scheda a tendina con dettagli aggiuntivi come Chiamata effettuata da, Chiamata con risposta da, Numero di telefono e Stato

## Visualizzazione elenco contatti e lead (azioni in blocco) {#lead-and-contact-list-view}

* [!UICONTROL Send Sales Email] - Possibilità di inviare e-mail personalizzate o con modelli con visualizzazione, tracciamento dei clic e delle risposte a un elenco di contatti/lead
* [!UICONTROL Add to Sales Campaign] - Aggiungi ai playbook di vendita che è una sequenza di e-mail e attività a un elenco di contatti/lead

## Scheda globale di Marketo {#marketo-global-tab}

Scheda **[!UICONTROL Best Bets]**

![](assets/sales-insight-actions-feature-overview-3.png)

Le seguenti azioni in blocco sono disponibili dal menu a discesa nella scheda [!UICONTROL Best Bets]:

* [!UICONTROL Send Sales Email] - Possibilità di inviare e-mail personalizzate o con modelli tramite visualizzazione, tracciamento dei clic e delle risposte
* [!UICONTROL Add to Sales Campaign] - Aggiungi lead ai playbook di vendita che è una sequenza di e-mail e attività

  ![](assets/sales-insight-actions-feature-overview-4.png)

Nella scheda [!UICONTROL Best Bets] sono disponibili le seguenti azioni in linea per singoli lead/contatti:

* [!UICONTROL Send Sales Email] - Possibilità di inviare e-mail personalizzate o con modelli tramite visualizzazione, tracciamento dei clic e delle risposte
* [!UICONTROL Add to Sales Campaign] - Aggiungi lead ai playbook di vendita che è una sequenza di e-mail e attività
* [!UICONTROL Sales Call] - Effettuare chiamate di vendita utilizzando la composizione nel CRM
* [!UICONTROL Add Task] - Crea attività e-mail, chiamata, cliente o LinkedIn per potenziali lead

  ![](assets/sales-insight-actions-feature-overview-5.png)

**Scheda E-Mail**

* Tutte le e-mail di vendita inviate verranno registrate qui. Le attività verranno anche registrate nel record persona di Marketo
* Le colonne includono Oggetto, Apri, Clic, Risposta (disponibile solo per e-mail di vendita con canale di consegna impostato), Mittente e Data
* Include la scheda di presentazione con dettagli aggiuntivi come Mittente, Modello, Campagna di vendita e Anteprima e-mail

**Scheda Chiamata**

* Tutte le chiamate effettuate utilizzando la funzione di chiamata di vendita verranno registrate qui. Le attività verranno anche registrate nel record persona di Marketo
* Le colonne includono Nome, Risultato, Note, Chiamata, Durata e collegamento alla registrazione
* Include una scheda a tendina con dettagli aggiuntivi come Chiamata effettuata da, Chiamata con risposta da, Numero di telefono e Stato

**Scheda Attività**

* Le attività e-mail, di chiamata, InMail e personalizzate create e completate saranno disponibili per la gestione delle attività in questa scheda. Include la possibilità di aggiungere un&#39;attività
* Automatizzare la creazione di attività con le campagne di vendita
* Sincronizza attività con [!DNL Salesforce]
* Registra le attività nella sezione Cronologia attività [!DNL Salesforce]

  ![](assets/sales-insight-actions-feature-overview-6.png)

**Feed live**

* Possibilità di visualizzare aggiornamenti live sulle attività di vendita e funzionalità di ancoraggio dello schermo
* I pulsanti e-mail, chiamata e cadenza incorporati rendono actionable ogni cliente insight

## Funzioni disponibili in Marketo {#features-available-in-marketo}

Attività di vendita acquisite in Marketo:

* Invia e-mail vendite: l’utente ha inviato un’e-mail di vendita a un lead
* Apri e-mail di vendita - Il lead ha aperto un messaggio e-mail di vendita inviato
* Fai clic su E-mail di vendita: il lead ha fatto clic su un collegamento in un’e-mail di vendita
* E-mail di vendita con risposta - Il lead ha risposto a un&#39;e-mail di vendita
* Ricevi chiamata di vendita: il lead ha ricevuto una chiamata da un venditore che utilizza la chiamata di vendita.
* Aggiungi a campagna di vendita: il lead è stato aggiunto a una campagna di vendita creata
* Rimosso dalla campagna di vendita: il lead è stato rimosso da una campagna di vendita creata

I filtri e i trigger includono:

* [!UICONTROL Is Sent Sales Email]
* [!UICONTROL Opens Sales Email]
* [!UICONTROL Clicks Sales Email]
* [!UICONTROL Replies to Sales Email]
* [!UICONTROL Receives Sales Call]
* [!UICONTROL Added to Sales Campaign]
* [!UICONTROL Removed from Sales Campaign]

  ![](assets/sales-insight-actions-feature-overview-7.png)
