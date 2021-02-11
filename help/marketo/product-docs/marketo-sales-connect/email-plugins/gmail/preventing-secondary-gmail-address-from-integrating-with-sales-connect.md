---
unique-page-id: 14352546
description: Impedire l'integrazione dell'indirizzo di posta elettronica secondario con Sales Connect - Marketo Docs - Documentazione del prodotto
title: Impedire l'integrazione dell'indirizzo e-mail secondario con Sales Connect
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# Impedire l&#39;integrazione dell&#39;indirizzo di posta elettronica secondario con il servizio di vendita {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Integrazione Gmail interrotta (perché il mio personale Gmail invia email) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

Il motivo più comune per una connessione Gmail interrotta è un&#39;integrazione accidentale con l&#39;account personale di un utente. Ciò può accadere quando un utente fa clic su &quot;Connect&quot; o quando tenta di inviare un&#39;e-mail dal proprio account personale. Questo può essere molto invitante a fare perché l&#39;opzione esisterà quando accedete al vostro account Gmail nella stessa istanza di Chrome del vostro lavoro e-mail.

## Perché Sales Connect tenta persino di effettuare l&#39;integrazione con il mio Gmail personale? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect si integra con Gmail tramite un&#39;estensione installata nel browser Chrome. Ogni volta che l&#39;estensione percepisce un&#39;istanza di Gmail aperta, offre un&#39;opzione per integrarsi con esso. Per impedire l&#39;integrazione con il tuo account Gmail personale, ti consigliamo una delle tre cose...

Accesso Come Altro Utente Chrome (Consigliato)

Fare clic su [questo collegamento](https://support.google.com/chrome/answer/2364824?hl=en) per leggere come creare un altro profilo Chrome.

**Pros**: L&#39;accesso come un altro utente aprirà una nuova istanza di Chrome. Questa istanza è una nuovissima finestra di Chrome, e nessuna delle vostre vecchie estensioni esisterà in questo. Inoltre tiene i cookie in modo da non dover accedere sempre al Gmail.

**Cons**: Devono essere aperte due finestre di Chrome.

Usa un altro browser

**Pros:** L&#39;utilizzo di un altro browser Internet (IE o Firefox) che non dispone dell&#39;estensione installata impedirà che ciò si verifichi.

**Cons**: L&#39;utilizzo di più browser può essere fastidioso.

Utilizzare Una Finestra In Incognito

**Pros:** Una finestra incognito è come aprire una versione nuda di Chrome. Ciò significa che non sarà installata alcuna delle vostre estensioni e che i servizi di vendita Connect non saranno presenti per connettersi.

**Cons**: Dovrai accedere a Gmail ogni volta che inizi la tua giornata, e di nuovo se chiudi accidentalmente la finestra.
