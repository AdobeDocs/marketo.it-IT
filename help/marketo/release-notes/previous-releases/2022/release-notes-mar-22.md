---
description: Note sulla versione - Marzo 2022 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione - Marzo 2022
exl-id: 91826d56-a38e-44af-b798-17bfc016c311
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 4%

---

# Note sulla versione - Marzo 2022 {#release-notes-mar-22}

Le seguenti funzioni sono incluse nella versione di marzo 2022. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità inizieranno a essere rilasciate il **11 marzo 2022**, con un rollout graduale di ogni funzionalità nelle settimane successive (se non specificato diversamente).

## Orchestrazione cross-channel {#cross-channel-orchestration}

* **[!DNL Dynamic Chat]**: massimizza ogni opportunità sul tuo sito web eseguendo il targeting sia dei lead che degli account con conversazioni proattive, coinvolgenti e 1:1 personalizzate. [Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} consente agli utenti di Marketo Engage di iniziare a sfruttare le chat come parte chiave delle esperienze cross-channel integrate per i casi di utilizzo di marketing e vendite B2B. Le caratteristiche includono: la possibilità di prenotare le riunioni direttamente all&#39;interno della chat, l&#39;indirizzamento dei lead, modelli di avvio, creazione di conversazioni con trascinamento e molto altro. Dynamic Chat è incluso in tutti i pacchetti Marketo Engage e verrà introdotto quest’anno per tutti gli utenti di Marketo Engage.

* **Miglioramento del filtro dell&#39;attività bot e-mail**: come miglioramento della funzione [Filtro dell&#39;attività bot e-mail](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"} rilasciata in precedenza, ora puoi dare il consenso per la registrazione delle attività identificate come bot. Puoi quindi filtrare e attivare le azioni in base alle attività identificate come eseguite dai bot.

## Esperienza di nuova generazione {#modern-ux}

* **Screens aggiornato nell&#39;esperienza di nuova generazione**: verranno forniti schermi aggiuntivi e aggiornati nell&#39;esperienza di nuova generazione che offrono una progettazione aggiornata e miglioramenti a livello di usabilità accessibili tramite l&#39;interruttore:

   * Visualizzazione elenco moduli in [!UICONTROL Design Studio] (incluse nuove azioni in blocco)

* **Aggiornamento del flusso di lavoro del programma di importazione**: il flusso di lavoro del programma di importazione viene consegnato nell&#39;esperienza di nuova generazione con una progettazione aggiornata e miglioramenti a livello di usabilità. Si tratta di una modifica automatica senza interruttore.

* **Controllo amministratore per l&#39;interruttore di attivazione dell&#39;esperienza di nuova generazione**: gestisce il rollout dell&#39;esperienza di nuova generazione in modo che funzioni per gli utenti, consentendo agli amministratori di selezionare i tipi di utenti che possono accedere all&#39;interruttore di attivazione.

## Automazione dell’esperienza {#experience-automation}

* **Passaggi di flusso self-service (Beta)**: espandi la connettività tra Marketo Engage e il resto dello stack con la possibilità di creare passaggi di flusso personalizzati da utilizzare nelle campagne avanzate. Sia gli utenti che i partner di Marketo possono sfruttare questa funzionalità per consentire l’utilizzo di servizi web esterni in campagne batch ed eseguibili, a differenza dei webhook, che possono essere utilizzati solo in campagne trigger.

* **Scadenza risorsa**: mantieni il controllo delle risorse e delle campagne sensibili al tempo con la possibilità di pianificare la loro disattivazione automatica a una data e un&#39;ora specificate nell&#39;esperienza utente classica.

* **Sostituzione priorità campagna avanzata**: assicurati che le campagne avanzate attivino l&#39;alta priorità il prima possibile, con la possibilità di ignorare la classificazione di priorità della campagna standard. È inoltre possibile ridurre la priorità delle campagne intelligenti con trigger a bassa priorità per liberare risorse di elaborazione per altre attività ad alta priorità.

## Miglioramenti API {#api-enhancements}

* **Restituisci lo stato di tracciamento delle e-mail aperte**: consente la lettura dello stato di tracciamento delle e-mail aperte tramite API
* **Recupera righe oggetto contenuto dinamico da e-mail**: consente agli addetti al marketing di eseguire analisi delle righe oggetto dinamiche negli strumenti di business intelligence
* **Campi personalizzati membro del programma CRUD**: consente agli addetti al marketing di creare in modo programmatico campi personalizzati membro del programma
* **Esportazione oggetti personalizzati in blocco aggiornataAl filtro**: consente agli addetti al marketing di sincronizzare in modo programmatico gli oggetti personalizzati
* **Impostazione di avvio automatico esposizione per i programmi e-mail**: consente agli addetti al marketing di configurare programmi e-mail con avvio automatico tramite API
* **Aggiornamento selettivo dei tag del programma**: consente agli addetti al marketing di inviare aggiornamenti selettivi dei tag senza spingere tutti i tag contemporaneamente
* **Campo actionResult estrazione attività in blocco**: consente agli addetti al marketing di identificare le attività ignorate o non riuscite

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## [!DNL Bizible] {#bizible}

![(stella)](assets/yellow-star.png)

* **Modelli BI**: [!DNL Bizible] fornirà gli artefatti di report fondamentali e scaricabili e i report di esempio per Tableau e Power BI per consentire lo sviluppo rapido di report personalizzati adatti alle tue esigenze aziendali specifiche.

## [!DNL Sales Connect] {#sales-connect}

![(stella)](assets/yellow-star.png)

* **Limitazione della connessione e-mail (GA)**: la limitazione della connessione e-mail consente agli amministratori di [!DNL Sales Connect] di configurare la frequenza di invio delle e-mail quando si utilizza Gmail o [!DNL Exchange] come canale di consegna, in modo che la frequenza con cui le e-mail vengono consegnate al provider del canale di consegna non superi i limiti imposti.

## Annunci {#announcements}

* **Deprecazione di Marketo Sky**: a marzo, Marketo Sky non sarà più disponibile, in quanto le nostre risorse saranno concentrate sulla distribuzione dell&#39;esperienza utente di nuova generazione. Nel tentativo di mantenere l’accesso a funzionalità esclusive di Marketo Sky, ora con Asset Expiration e Smart Campaign Priority Override vengono introdotte nell’esperienza classica. [Fai clic qui](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) per ulteriori informazioni.

**_Webinar sulla versione del prodotto_**

[Webinar sulla versione di Marketo Engage di marzo e maggio 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
