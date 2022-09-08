---
unique-page-id: 10096683
description: Aggiornamenti alla registrazione degli eventi ON24 - Documenti Marketo - Documentazione del prodotto
title: Aggiornamenti alla registrazione degli eventi ON24
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Aggiornamenti alla registrazione degli eventi ON24 {#on-event-registration-updates}

>[!IMPORTANT]
>
>A partire da agosto 2022, ON24 non supporta più nuove integrazioni Marketo. Le informazioni contenute in questo articolo si applicano solo agli utenti esistenti.

## Approvazione manuale dei dichiaranti {#manually-approving-registrants}

Puoi approvare manualmente i registranti prima di inviare loro un messaggio e-mail di conferma. A questo scopo, dovrai configurare le campagne per gestire questo passaggio aggiuntivo:

1. Per la campagna di attivazione della registrazione:

   * Nell’elenco avanzato, imposta il trigger su **Riempie il modulo**.
   * Nel flusso, imposta lo stato in progressivo su **Approvazione in sospeso**.

1. Vai all’evento e fai clic sul pulsante **Membri** scheda . In questa scheda vengono visualizzate tutte le persone che hanno compilato il modulo. Il loro stato deve essere impostato su **Approvazione in sospeso**.
1. Utilizza il filtro nella parte superiore della griglia per visualizzare solo le persone con uno stato **Approvazione in sospeso**.
1. Selezionare le persone da registrare (MAIUSC+clic, CTRL+clic o Seleziona tutto).
1. Dal menu , fai clic su **Cambia stato**. Seleziona **Registrato**, **Rifiutato** o qualsiasi altro stato applicabile.

## Gestione delle persone con un errore di registrazione {#handling-people-with-a-registration-error}

Se una persona finisce per non essere registrata, ma piuttosto impostato sullo stato Errore di registrazione, non è troppo tardi per recuperare.

1. Dalla scheda Membri , filtra l’elenco delle persone con lo stato **Errore di registrazione**.
1. Prima di continuare, assicurati di aver determinato e risolto il problema relativo all&#39;integrazione (controlla che non ci siano errori in **Partner eventi** in Admin).
1. Una volta risolto il problema, seleziona tutte le persone con lo stato Errore di registrazione e cambia il loro stato in **Registrato**. Si cercherà di registrarli nuovamente con ON24.

## Aggiornamento dello stato membro da ON24 {#updating-member-status-from-on}

Marketo richiama automaticamente le informazioni sulla presenza alle 11 di sera circa nel Pacifico. Per aggiornare manualmente le informazioni sulla presenza, fai clic su **Aggiorna da Webinar Provider** sotto **Azioni evento**.

>[!MORELIKETHIS]
>
>[Informazioni sugli eventi dell&#39;adattatore Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
