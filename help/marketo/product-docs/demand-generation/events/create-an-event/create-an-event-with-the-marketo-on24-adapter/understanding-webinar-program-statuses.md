---
unique-page-id: 10096681
description: Informazioni sugli stati del programma Webinar - Documenti Marketo - Documentazione del prodotto
title: Informazioni sugli stati del programma webinar
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# Informazioni sugli stati del programma webinar {#understanding-webinar-program-statuses}

>[!IMPORTANT]
>
>A partire da agosto 2022, ON24 non supporta più nuove integrazioni Marketo. Le informazioni contenute in questo articolo si applicano solo agli utenti esistenti.

Gli stati del programma rappresentano i diversi stati dell’evento che una persona compie come membro dell’evento. Sono associati a un tipo di canale. Marketo ha un tipo di canale integrato denominato **Webinar**. Gli stati possono essere utilizzati sia nelle campagne batch che nelle campagne di attivazione.

Le persone si spostano attraverso lo stato del programma in modo lineare e non tornano indietro nello stato. Ad esempio, una persona con uno stato di **Partecipato** impossibile tornare a **Registrato**.

Ecco una breve descrizione degli stati del programma associati al canale del webinar.

>[!TIP]
>
>Per aggiornare manualmente gli stati, fai clic su  **Aggiorna da Webinar Provider** in **Azioni evento** a discesa.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Non in programma** - Utilizzare questo stato per rimuovere le persone dall&#39;evento.

**Invitato** - Utilizzare questo stato per aggiungere persone all&#39;evento.

**Approvazione in sospeso** - Utilizza questo stato per interrompere l’invio di un’e-mail di conferma alle tue persone. Consulta &quot;Approvazione manuale degli utenti registrati&quot; in [Aggiornamenti alla registrazione degli eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md) per ulteriori informazioni.

**Wait Listed** - Utilizzare questo stato per mantenere alcune persone in attesa di ulteriori posti disponibili.

**Rifiutato** - Utilizzare questo stato per rifiutare la registrazione di una persona all&#39;Evento.

**Registrato** - Questo stato spinge le persone su ON24 quando si utilizza l&#39;integrazione ON24. Lo stato della persona viene aggiornato quando ON24 risponde che la persona è stata registrata correttamente.

**Errore di registrazione** - Questo stato indica che l&#39;utente ha rilevato un errore durante il tentativo di registrazione per l&#39;evento.

>[!NOTE]
>
>Se si verifica un errore di registrazione, è possibile ottenere informazioni aggiuntive per tale persona guardando la colonna Motivo stato nella scheda Membri del programma. Una volta corretto l’errore, puoi modificare manualmente lo stato del programma dell’utente in Registrato in Marketo.

**Partecipato** - Al termine del webinar, ON24 restituisce un elenco di persone che hanno partecipato. Questo stato viene estratto automaticamente in Marketo.

**Atteso on-demand** - Le persone che hanno partecipato alla versione archiviata del webinar ricevono questo stato.

**Nessuna visualizzazione** - Al termine del webinar e dopo aver estratto i dati di presenza da ON24, lo stato delle persone che si sono registrate ma non hanno partecipato viene aggiornato a No Show. L&#39;ON24 può richiedere da 30 minuti a 3 ore per preparare le informazioni sulla presenza finale e renderle disponibili in Marketo.

>[!NOTE]
>
>Affinché Marketo possa ottenere lo stato No Show, le persone devono essere state registrate *in Marketo*. Non è possibile acquisire No Show proveniente dal feed di dati On24.

>[!MORELIKETHIS]
>
>[Informazioni sugli eventi dell&#39;adattatore Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
