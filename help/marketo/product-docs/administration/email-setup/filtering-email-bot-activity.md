---
description: Filtrare l’attività del bot e-mail - Documenti Marketo - Documentazione del prodotto
title: Filtrare l’attività del bot e-mail
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: a64c499f6972e94adfecbe164d86f7db1b1447aa
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Filtrare l’attività del bot e-mail {#filtering-email-bot-activity}

A volte, l’attività di bot e-mail può gonfiare erroneamente i dati di apertura e clic delle e-mail. Ecco come ripararlo.

>[!NOTE]
>
>Utilizzo della [Lista di ragni e bot internazionali IAB/ABC](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/), tutte le attività di apertura/clic con un IP o un agente utente che corrispondono a qualsiasi elemento di tale elenco verranno identificate come attività bot e non verranno registrate in Marketo.

1. Fai clic su **Amministratore**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Fai clic su **E-mail**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Fai clic sul pulsante **Attività bot** scheda .

   ![](assets/filtering-email-bot-activity-3.png)

1. Fai clic sul cursore per abilitare **Attività bot filtro**.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Puoi scegliere separatamente se registrare o meno l’attività bot. Se scegli di non farlo, potresti visualizzare un calo delle aperture delle e-mail e dei clic mentre i numeri falsi vengono filtrati.

**PASSAGGIO OPZIONALE**: Per disattivare la funzione, deselezionare il dispositivo di scorrimento. Se disattivi, i dati &quot;Attività bot negli ultimi 90 giorni&quot; sì **not** reimpostare.

>[!TIP]
>
>Utilizza i dati delle attività bot negli elenchi avanzati tramite &quot;Is Bot Activity&quot; booleano (sì/no) o nei vincoli di filtro/trigger applicabili.
