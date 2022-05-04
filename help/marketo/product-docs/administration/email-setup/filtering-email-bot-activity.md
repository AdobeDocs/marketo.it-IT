---
description: Filtrare l’attività del bot e-mail - Documenti Marketo - Documentazione del prodotto
title: Filtrare l’attività del bot e-mail
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: 2ef4b0b2a541c8b6a67bd654fda45956601661bd
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Filtrare l’attività del bot e-mail {#filtering-email-bot-activity}

A volte, l’attività di bot e-mail può gonfiare erroneamente i dati di apertura e clic delle e-mail. Segui i passaggi seguenti per risolvere il problema.

Utilizziamo tre metodi distinti per confermare l’attività di bot:

* Corrispondenza con [Elenco bot di Interactive Advertising Bureau](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target=&quot;_blank&quot;}: Le attività che corrispondono a qualsiasi elemento nell’elenco UA/IP (User Agent/IP address) IAB saranno contrassegnate come bot.
* Corrispondenza con gli UA/IP del collegamento nascosto: Aggiungiamo un collegamento nascosto a tutte le e-mail e acquisiamo i clic UA/IP provenienti da esse. Le attività che corrispondono a questi UA/IP saranno contrassegnate come bot.
* Corrispondenza con il pattern di prossimità: Quando più di due attività si verificano contemporaneamente (in meno di due secondi), vengono identificate come bot.

In corrispondenza dell’attività di selezione dei collegamenti e-mail e apertura delle e-mail, i nuovi attributi verranno compilati con i valori seguenti:

* Le attività identificate come bot avranno &quot;Attività bot&quot; come &quot;True&quot; e &quot;Pattern attività bot&quot; come pattern/metodo identificato
* Le attività identificate come non bot avranno &quot;Attività bot&quot; come &quot;False&quot; e &quot;Pattern attività bot&quot; come &quot;N/A&quot;
* Le attività che sono successe prima dell’introduzione di questi attributi avranno &quot;Attività bot&quot; come &quot; (vuoto) e &quot;Pattern attività bot&quot; come &quot; (vuoto)

1. Fai clic su **Amministratore**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Fai clic su **E-mail**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Fai clic sul pulsante **Attività bot** scheda .

   ![](assets/filtering-email-bot-activity-3.png)

1. Fai clic sul pulsante **Abilita identificazione attività bot** cursore da attivare.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Puoi scegliere separatamente se registrare o meno l’attività bot. Se scegli di non farlo, potresti visualizzare un calo delle aperture delle e-mail e dei clic mentre i numeri falsi vengono filtrati.

**PASSAGGIO OPZIONALE**: Per disattivare la funzione, deselezionare il dispositivo di scorrimento. Se disattivi, i dati sì **not** reimpostare.

>[!TIP]
>
>Sfrutta i dati delle attività bot negli elenchi avanzati tramite &quot;Is Bot Activity&quot; booleano (sì/no) e &quot;Bot Activity Pattern&quot; nei filtri &quot;Click Link in Email&quot; e &quot;Open Email&quot;, e gli attivatori &quot;Click Link in Email&quot; e &quot;Open Email&quot;.
