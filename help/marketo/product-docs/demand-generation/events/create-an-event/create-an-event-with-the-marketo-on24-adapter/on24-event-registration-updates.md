---
unique-page-id: 10096683
description: Aggiornamenti alla registrazione di eventi ON24 - Documentazione di Marketo - Documentazione del prodotto
title: Aggiornamenti alla registrazione dell'evento ON24
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# Aggiornamenti alla registrazione dell&#39;evento ON24 {#on-event-registration-updates}

## Approvazione manuale dei dichiaranti {#manually-approving-registrants}

Puoi approvare manualmente i tuoi iscritti prima di inviare loro un messaggio e-mail di conferma. A tal fine, dovrai configurare le campagne per gestire questo passaggio aggiuntivo:

1. Per la campagna Trigger registrazione:

   * Nell&#39;elenco avanzato, impostare il trigger su **Compila modulo**.
   * Nel flusso, impostare lo stato in Progressione su **In attesa di approvazione**.

1. Vai all&#39;evento e fai clic sulla scheda **Membri**. In questa scheda vengono visualizzate tutte le persone che hanno compilato il modulo. Il loro stato deve essere impostato su **In attesa di approvazione**.
1. Utilizza il filtro nella parte superiore della griglia per visualizzare solo le persone con uno stato di **In attesa di approvazione**.
1. Selezionare le persone da registrare (Maiusc-clic, Ctrl-clic o Seleziona tutto).
1. Scegliere **Modifica stato** dal menu. Seleziona **Registrato**, **Rifiutato** o qualsiasi altro stato applicabile.

## Gestione delle persone con un errore di registrazione {#handling-people-with-a-registration-error}

Se una persona alla fine non viene registrata, ma piuttosto impostata sullo stato Errore di registrazione, non è troppo tardi per recuperare.

1. Dalla scheda Membri, filtrare l&#39;elenco di persone con lo stato **Errore di registrazione**.
1. Prima di continuare, accertati di aver determinato e risolto il problema con l&#39;integrazione (verifica che non vi siano errori in **Partner evento** in Amministratore).
1. Dopo aver risolto il problema, selezionare tutte le persone con lo stato Errore di registrazione e modificarne lo stato in **Registrato**. Verrà eseguito un nuovo tentativo di registrazione con ON24.

## Aggiornamento dello stato del membro da ON24 {#updating-member-status-from-on}

Marketo richiama automaticamente le informazioni sulla frequenza alle 23:00 circa (Pacifico) di ogni notte. Per aggiornare manualmente le informazioni sulla partecipazione, fare clic su **Aggiorna dal provider webinar** in **Azioni evento**.

>[!MORELIKETHIS]
>
>[Informazioni sugli eventi della scheda di rete Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
