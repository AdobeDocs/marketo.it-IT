---
description: Connetti nuovo amministratore a Marketo - Documentazione Marketo - Documentazione del prodotto
title: Connetti nuovo amministratore a Marketo
hide: true
hidefromtoc: true
source-git-commit: 0ed5981470998dadd5f42384cd2e9572fec94ef6
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Connetti nuovo amministratore a Marketo {#connect-new-admin-to-marketo}

Se l’altro amministratore è già connesso a Marketo, deve solo eseguire il passaggio 1.

Se il secondo amministratore non è connesso a Marketo come amministratore..

1. L’amministratore principale deve disconnettere il secondo amministratore da Marketo da Impostazioni > Marketo > Accesso utente

1. L’amministratore secondario accede al proprio account MSC, passa a Impostazioni > Marketo e fa clic **Connetti**.

1. Ora l’utente secondario è connesso a Marketo come amministratore.

1. L&#39;amministratore principale può ora effettuare l&#39;accesso e disconnettersi da Marketo.

>[!NOTE]
>
>Gli altri utenti rimarranno connessi finché l&#39;utente B sarà connesso come amministratore prima che l&#39;utente A si disconnette.

## Aggiorna la tua connessione Marketo {#update-your-marketo-connection}

Se decidi di voler rimuovere l&#39;amministratore che ha impostato l&#39;integrazione di Marketo, consulta questo articolo per scoprire come.

L’integrazione di Marketo sarà legata a un utente amministratore di Sales Connect/Actions. In genere, si tratta dell’amministratore che ha fatto clic sul pulsante &quot;Connect&quot; nella pagina di connessione di Marketo e ha stabilito la connessione.

Per rimuovere l’amministratore che ha stabilito la connessione Marketo, un nuovo collegamento deve prima essere stabilito da un altro utente amministratore. Abbiamo elencato le attività riportate di seguito che dovranno essere completate per eseguire questa operazione.

Al fine di semplificare le istruzioni, ci riferiremo all’amministratore attualmente connesso come amministratore A e all’amministratore che desideri stabilire una nuova connessione a Marketo con come amministratore B:

1. L&#39;amministratore A (amministratore attualmente connesso) dovrà rimuovere l&#39;accesso all&#39;integrazione con Marketo dall&#39;amministratore B (nuovo amministratore).

1. Chiedi all’amministratore B (nuovo amministratore) di stabilire una nuova connessione a Marketo.

1. Disconnetti amministratore A (amministratore connesso in origine).

>[!NOTE]
>
>L’amministratore originale responsabile dell’integrazione di Marketo vedrà un’opzione &quot;Disconnetti&quot; su cui è possibile fare clic quando si passa alla pagina di integrazione di Marketo. Gli altri amministratori (che non hanno stabilito una connessione) non lo faranno. Inoltre, gli amministratori a cui è stato concesso l’accesso all’integrazione Marketo non potranno fare clic su Connetti. Per questo motivo è necessario seguire prima i passaggi per rimuovere l’accesso all’integrazione.

**Rimuovere l&#39;accesso Marketo dall&#39;amministratore B**

L’amministratore A (amministratore originariamente responsabile della connessione) deve seguire questi passaggi.

1. Passa alle impostazioni .

1. Fai clic su **Marketo**.

1. Fai clic su **Accesso utente**.

1. Cerca l’amministratore per il quale desideri stabilire la nuova connessione Marketo.

1. Rimuovi l&#39;accesso.

**Stabilire una nuova connessione per l&#39;amministratore B**

Questi passaggi devono essere seguiti dall&#39;amministratore B (nuovo amministratore)

1. Passa alle impostazioni .

1. Fai clic su **Marketo**.

1. Fai clic su **Disconnetti**.

**Disconnettere l&#39;integrazione Marketo per l&#39;amministratore A**

Questi passaggi devono essere seguiti dall&#39;amministratore A (amministratore originariamente connesso)

1. Passa alle impostazioni .

1. Fai clic su **Marketo**.

1. Fai clic su **Disconnetti**.

Ora che un nuovo amministratore ha stabilito una connessione a Marketo e l&#39;amministratore originale è stato disconnesso, l&#39;amministratore originariamente connesso può essere rimosso in tutta sicurezza dall&#39;istanza Sales Connect/Actions.
