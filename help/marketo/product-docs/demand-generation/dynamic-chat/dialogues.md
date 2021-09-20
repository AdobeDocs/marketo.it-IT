---
description: Finestre di dialogo - Documenti Marketo - Documentazione del prodotto
title: Finestre di dialogo
hide: true
hidefromtoc: true
source-git-commit: c6713c972603ab9528a66e908e47e4c187b86c0c
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# Finestre di dialogo {#dialogues}

Le finestre di dialogo sono le conversazioni di chat specifiche impostate. Possono essere personalizzati per look, così come quello che si dice e chi lo vede.

## Creare una nuova finestra di dialogo {#create-a-new-dialogue}

1. Fare clic su **Finestre di dialogo**.

PICC

1. Fare clic sul pulsante **Crea nuovo**.

PICC

1. Immetti un nome (la descrizione è facoltativa), imposta il livello di priorità e fai clic su **Salva**.

PICC

>[!NOTE]
>
>SPIEGA IL LIVELLO DI PRIORITÀ

## Criteri del pubblico {#audience-criteria}

Analogamente agli elenchi avanzati di Marketo, gli attributi dei criteri per il pubblico consentono di definire il pubblico di destinazione.

Ci sono diversi attributi tra cui scegliere. In questo esempio, puntiamo tutti i lead noti in California che lavorano in un&#39;azienda con più di 50 dipendenti.

1. Acquisite l’attributo Stato lead e trascinatelo a destra.

PICC

1. __ Isis impostato per impostazione predefinita. Nel campo Seleziona valori digitare CA (è inoltre possibile fare clic sul menu a discesa e selezionare dall’elenco).

PICC

1. Prendi l&#39;attributo Dimensione società e trascinalo a destra.

PICC

1. Fai clic sull’elenco a discesa dell’operatore e seleziona Maggiore di.

PICC

1. Digitare 50 e fare clic in un altro punto dello schermo per salvare.

PICC

COME CATTURARE ANON LEAD

NOTA - forse accennato a come lavori dedotti/mostra caso d’uso, l’e-mail lead è vuota

## Aggiungi gruppi {#add-groups}

Hai anche la possibilità di raggruppare gli attributi, nel caso in cui desideri avere tutti gli attributi insieme a &quot;qualsiasi&quot; di un altro.

FINISCI QUESTO

## Target {#target}

In questo punto immetti gli URL specifici su cui desideri visualizzare una finestra di dialogo specifica.

Formati accettabili:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>L&#39;utilizzo di un asterisco funge da jolly catch-all. Quindi `https://*.website.com` inserirebbe la finestra di dialogo su ogni pagina del sito, inclusi i sottodomini (ad esempio: `support.website.com`). E `https://website.com/folder/*` inseriva la finestra di dialogo in ogni pagina HTML della cartella successiva (ad esempio: in questo caso diciamo che la cartella è &quot;sport&quot;, quindi: website.com/sports/baseball.html, website.com/sports/football.html, ecc.).

## Progettazione flussi {#stream-designer}

Il designer del flusso contiene diverse schede che è possibile aggiungere per modellare la conversazione di chat.

TABELLA

Messaggio: Utilizzare quando si desidera eseguire un&#39;istruzione senza alcuna risposta necessaria (ad esempio: &quot;Ciao! Oggi tutti gli articoli sono con uno sconto del 25% con codice SAVE25.&quot;)

Domanda: Utilizzare quando si desidera porre una domanda a scelta multipla, di cui fornire le risposte disponibili (ad esempio: A che tipo di veicolo ti interessa? Risposte = SUV, compatto, camion, ecc.)

Acquisizione delle informazioni: Utilizza quando desideri raccogliere informazioni. I tre campi tra cui scegliere sono Indirizzo e-mail, Numero di telefono e Testo (che consente al visitatore di scrivere il proprio messaggio).

Utilità di pianificazione degli appuntamenti: Fornisce al visitatore un calendario delle date disponibili per pianificare un follow-up. La disponibilità del calendario riflette [l&#39;agente successivo in riga](help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing).

Obiettivo: Questa è l&#39;unica carta che i visitatori non vedranno. Sta a te determinare a quale punto un obiettivo viene raggiunto all&#39;interno della chat specifica (es: se la raccolta dell&#39;e-mail del visitatore è l&#39;obiettivo, posiziona la scheda Obiettivo dopo l&#39;acquisizione delle informazioni nello streaming.)

POSSIBILE SEZIONE PROPRIA

MOSTRA GLI ESEMPI SEGUENTI