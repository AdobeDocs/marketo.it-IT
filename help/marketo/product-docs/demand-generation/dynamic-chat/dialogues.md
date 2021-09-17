---
description: Finestre di dialogo - Documenti Marketo - Documentazione del prodotto
title: Finestre di dialogo
hide: true
hidefromtoc: true
source-git-commit: c46902686f1d5af63a51f5eaae2dc0e6afe99629
workflow-type: tm+mt
source-wordcount: '273'
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

Ci sono diversi attributi tra cui scegliere. In questo esempio scegliamo Stato lead _è_ California e la dimensione dell&#39;azienda _è maggiore di_ 50.

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
>L&#39;utilizzo di un asterisco funge da jolly catch-all. Quindi `https://*.website.com` inserirebbe la finestra di dialogo su ogni pagina del sito, inclusi i sottodomini (ad esempio: support.website.com). E `https://website.com/folder/*` inseriva la finestra di dialogo in ogni pagina HTML della cartella successiva (ad esempio: in questo caso diciamo che la cartella è &quot;sport&quot;, quindi: website.com/sports/baseball.html, website.com/sports/football.html, ecc.).
