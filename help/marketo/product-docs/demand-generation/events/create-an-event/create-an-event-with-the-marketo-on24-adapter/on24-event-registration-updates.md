---
unique-page-id: 10096683
description: Aggiornamenti alla registrazione degli eventi ON24 - Documenti Marketo - Documentazione del prodotto
title: Aggiornamenti alla registrazione degli eventi ON24
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---


# Aggiornamenti alla registrazione degli eventi ON24 {#on-event-registration-updates}

## Approvazione manuale degli utenti registrati {#manually-approving-registrants}

Potete approvare manualmente gli utenti registrati prima di inviare loro un messaggio e-mail di conferma. A tal fine, dovrete configurare le campagne per gestire questo passaggio aggiuntivo:

1. Per la campagna di registrazione Trigger:

   * Nell&#39;elenco avanzato, impostare l&#39;attivatore su **Riempi modulo**.
   * In Flusso, imposta lo stato in Progressione su **In attesa di approvazione**.

1. Passate all’evento e fate clic sulla scheda **Membri** . In questa scheda vengono visualizzate tutte le persone che hanno compilato il modulo. Il relativo stato deve essere impostato su **In attesa di approvazione**.
1. Utilizzate il filtro nella parte superiore della griglia per visualizzare solo le persone con lo stato **In attesa di approvazione**.
1. Selezionate le persone da registrare (Maiusc+clic, Ctrl+clic o Seleziona tutto).
1. Dal menu, fate clic su **Modifica stato**. Selezionate **Registrato**, **Rifiutato** o qualsiasi altro stato applicabile.

## Gestione delle persone con un errore di registrazione {#handling-people-with-a-registration-error}

Se una persona finisce per non essere registrata, ma piuttosto impostata sullo stato Errore di registrazione, non è troppo tardi per recuperare.

1. Dalla scheda Membri, filtrate l’elenco delle persone con lo stato Errore **di** registrazione.
1. Prima di continuare, accertatevi di aver determinato e risolto il problema con l&#39;integrazione (verificate che non ci siano errori in Partner **** evento in Amministratore).
1. Una volta risolto il problema, selezionate tutte le persone con lo stato Errore di registrazione e cambiate il loro stato in **Registrato**. Questo tenterà di registrarli nuovamente con ON24.

## Aggiornamento dello stato membro da ON24 {#updating-member-status-from-on}

Marketo raccoglie automaticamente le informazioni di presenza all&#39;incirca alle 11:00 del Pacifico ogni notte. Per aggiornare manualmente le informazioni di partecipazione, fate clic su **Aggiorna dal provider** webinar in Azioni **** evento.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Informazioni sugli eventi dell&#39;adattatore Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



