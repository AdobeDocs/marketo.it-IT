---
unique-page-id: 10096681
description: Informazioni sugli stati dei programmi del webinar - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sugli stati dei programmi di webinar
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Informazioni sugli stati dei programmi di webinar {#understanding-webinar-program-statuses}

Gli stati del programma rappresentano i diversi stati dell’evento che una persona sviluppa come membro dell’evento. Sono associati a un tipo di canale. Marketo ha un tipo di canale integrato denominato **Webinar**. Gli stati possono essere utilizzati sia nelle campagne batch che in quelle attivate.

Le persone passano da uno stato all’altro del programma in modo lineare e non tornano indietro nello stato. Ad esempio, una persona con lo stato **Partecipazione avvenuta** impossibile tornare a **Registrato**.

Segue una breve descrizione degli stati del programma associati al canale del webinar.

>[!TIP]
>
>Per aggiornare manualmente gli stati, fai clic su  **Aggiorna dal provider del webinar** nel **Azioni evento** a discesa.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Non nel programma** : utilizza questo stato per rimuovere le persone dall’evento.

**Invitato** : utilizza questo stato per aggiungere persone all’evento.

**In attesa di approvazione** - Utilizza questo stato per rimandare l’invio di un’e-mail di conferma al tuo popolo. Consulta &quot;Approvazione manuale dei dichiaranti&quot; in [Aggiornamenti alla registrazione dell&#39;evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"} per ulteriori informazioni.

**In lista d’attesa** - Utilizzare questo stato per mantenere alcune persone in attesa fino a quando non saranno disponibili posti aggiuntivi.

**Rifiutato** - Utilizzare questo stato per rifiutare la registrazione di una persona all&#39;evento.

**Registrato** - Questo stato spinge le persone su ON24 quando si utilizza l&#39;integrazione ON24. Lo stato della persona viene aggiornato quando ON24 risponde che la persona è stata registrata correttamente.

**Errore di registrazione** - Questo stato indica che l’utente ha riscontrato un errore durante il tentativo di registrazione all’evento.

>[!NOTE]
>
>Se si verifica un errore di registrazione, è possibile ottenere ulteriori informazioni per tale persona osservando la colonna Motivo stato nella scheda Membri del programma. Una volta corretto l’errore, puoi cambiare manualmente lo stato del programma dell’utente in Registrato in Marketo.

**Partecipazione avvenuta** - Al termine del webinar, ON24 restituisce un elenco di persone che hanno partecipato. Questo stato viene richiamato automaticamente in Marketo.

**Partecipazione on-demand** - Le persone che hanno partecipato alla versione archiviata del webinar ricevono questo stato.

**Nessuno spettacolo** - Al termine del webinar e dopo aver estratto i dati di partecipazione da ON24, lo stato delle persone che si sono registrate ma non hanno partecipato viene aggiornato a No Show (Nessuno spettacolo). Il servizio ON24 può richiedere da 30 minuti a 3 ore per preparare le informazioni finali sulla partecipazione e renderle disponibili in Marketo.

>[!NOTE]
>
>Affinché Marketo possa richiamare lo stato No Show (No Show), le persone devono essere state registrate *in Marketo*. Non è possibile acquisire alcun programma proveniente dal feed di dati On24.

>[!MORELIKETHIS]
>
>[Informazioni sugli eventi delle schede di rete Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
