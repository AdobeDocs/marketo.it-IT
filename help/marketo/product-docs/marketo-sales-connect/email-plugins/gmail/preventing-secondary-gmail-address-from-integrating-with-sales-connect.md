---
unique-page-id: 14352546
description: Impedire l'integrazione dell'indirizzo Gmail secondario con Sales Connect - Documenti Marketo - Documentazione del prodotto
title: Impedire l'integrazione dell'indirizzo Gmail secondario con Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Impedire l&#39;integrazione dell&#39;indirizzo Gmail secondario con [!DNL Sales Connect] {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Integrazione Gmail interrotta (perché il mio Gmail personale invia e-mail) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Il motivo più comune per una connessione Gmail interrotta è un’integrazione accidentale con l’account personale di un utente. Ciò può verificarsi quando un utente fa clic su &quot;Connetti&quot; o quando tenta di inviare un’e-mail dal proprio account personale. Potrebbe essere molto interessante, perché l&#39;opzione esiste quando si accede al proprio account Gmail nella stessa istanza di [!DNL Chrome] dell&#39;e-mail aziendale.

## Perché [!DNL Sales Connect] tenta persino di integrarsi con il mio Gmail personale? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

[!DNL Sales Connect] si integra con Gmail tramite un&#39;estensione installata nel browser [!DNL Chrome]. Ogni volta che l’estensione rileva un’istanza di Gmail aperta, offre un’opzione per integrarla. Per evitare un’integrazione con il tuo account Gmail personale, ti consigliamo una delle tre cose seguenti:

Accedi Come Altro [!DNL Chrome] Utente (Consigliato)

Fai clic su [questo collegamento](https://support.google.com/chrome/answer/2364824?hl=en) per leggere come creare un altro [!DNL Chrome]profilo.

**Pro**: l&#39;accesso come altro utente aprirà una nuova istanza di [!DNL Chrome]. Questa istanza è una nuova finestra di [!DNL Chrome] e nessuna delle vecchie estensioni esisterà in questa. Inoltre, conserva i cookie in modo da non dover accedere al tuo Gmail ogni volta.

**Contro**: devono essere aperte due finestre di [!DNL Chrome].

Usa un altro browser

**Pro:** l&#39;utilizzo di un altro browser Internet (IE o Firefox) in cui non è installata l&#39;estensione impedirà che ciò accada.

**Contro**: l&#39;utilizzo di più browser può essere fastidioso.

Utilizzare Una Finestra In Incognito

**Pro:** Una finestra in incognito è simile all&#39;apertura di una versione nuda di [!DNL Chrome]. Ciò significa che non avrà installato nessuna delle tue estensioni e [!DNL Sales Connect] non sarà presente per connettersi.

**Contro**: dovrai accedere a Gmail ogni volta che inizi la tua giornata e di nuovo se chiudi accidentalmente la finestra.
