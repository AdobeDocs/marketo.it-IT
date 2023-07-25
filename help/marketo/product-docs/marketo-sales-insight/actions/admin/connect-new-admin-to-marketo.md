---
description: Collegare il nuovo amministratore a Marketo - Documentazione di Marketo - Documentazione del prodotto
title: Connetti nuovo amministratore a Marketo
exl-id: ef405bca-a29a-40fc-9efa-eccff5f45956
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Connetti nuovo amministratore a Marketo {#connect-new-admin-to-marketo}

Se l’altro amministratore è già connesso a Marketo, deve eseguire solo il passaggio 1.

Se il secondo amministratore non è connesso a Marketo come amministratore...

1. L’amministratore principale deve disconnettere il secondo amministratore da Marketo da Impostazioni > Marketo > Accesso utente.

1. L’amministratore secondario accede al proprio account MSC, passa a Impostazioni > Marketo e fa clic su **Connetti**.

1. Ora l’utente secondario è connesso a Marketo come amministratore.

1. L’amministratore principale ora può effettuare l’accesso e disconnettersi da Marketo.

>[!NOTE]
>
>Gli altri utenti rimarranno connessi finché l’utente B sarà connesso come amministratore prima che l’utente A si disconnetta.

## Aggiornare la connessione Marketo {#update-your-marketo-connection}

Se decidi di rimuovere l’Amministratore che ha configurato l’integrazione di Marketo, consulta questo articolo per scoprire come.

L’integrazione Marketo sarà associata a un utente amministratore di Sales Connect/Actions. In genere, si tratta dell’amministratore che ha fatto clic per primo sul pulsante &quot;Connetti&quot; nella pagina di connessione di Marketo e ha stabilito la connessione.

Per rimuovere l’amministratore che ha stabilito la connessione a Marketo, è necessario prima stabilire una nuova connessione da un altro utente amministratore. Abbiamo elencato le attività seguenti che dovranno essere completate per farlo.

Per semplificare le istruzioni, consulta l’Amministratore attualmente connesso come Amministratore A e l’Amministratore che desideri stabilire una nuova connessione a Marketo con come Amministratore B:

1. L’Amministratore A (Amministratore attualmente connesso) dovrà rimuovere l’accesso all’integrazione con Marketo dall’Amministratore B (nuovo Amministratore).

1. Chiedi all&#39;amministratore B (nuovo amministratore) di stabilire una nuova connessione a Marketo.

1. Disconnetti Admin A (originariamente connesso Admin).

>[!NOTE]
>
>L’amministratore originale responsabile dell’integrazione di Marketo visualizzerà un’opzione &quot;Disconnetti&quot; selezionabile quando si passa alla pagina di integrazione di Marketo. Altri amministratori (che non hanno stabilito una connessione) non lo faranno. Inoltre, gli amministratori a cui è stato concesso l’accesso all’integrazione Marketo non potranno fare clic su Connetti, per questo motivo è necessario seguire i passaggi per rimuovere prima l’accesso all’integrazione.

**Rimuovi accesso a Marketo dall&#39;amministratore B**

L’Amministratore A (originariamente responsabile della connessione) deve seguire la procedura riportata di seguito.

1. Nell’applicazione web, fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

1. Clic **Marketo**.

1. Clic **Accesso utente**.

1. Cerca l’Amministratore per il quale vuoi stabilire la nuova connessione Marketo.

1. Rimuovi l&#39;accesso.

**Stabilisci nuova connessione per l’amministratore B**

Questi passaggi devono essere seguiti da Amministratore B (nuovo Amministratore)

1. Nell’applicazione web, fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

1. Clic **Marketo**.

1. Clic **Disconnetti**.

**Disconnettere l’integrazione di Marketo per l’amministratore A**

Questi passaggi devono essere seguiti dall’Amministratore A (Amministratore originariamente connesso).

1. Nell’applicazione web, fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

1. Clic **Marketo**.

1. Clic **Disconnetti**.

Ora che un nuovo amministratore ha stabilito una connessione a Marketo e l’amministratore originale è stato disconnesso, l’amministratore originariamente connesso può essere rimosso in modo sicuro dall’istanza Sales Connect/Actions.
