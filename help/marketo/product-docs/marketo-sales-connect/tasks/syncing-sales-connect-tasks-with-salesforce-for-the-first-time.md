---
unique-page-id: 14352541
description: Sincronizzazione delle attività di vendita con Salesforce per la prima volta - Documentazione di Marketo - Documentazione del prodotto
title: Sincronizzazione delle attività di Sales Connect con Salesforce per la prima volta
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# È in corso la prima sincronizzazione di [!DNL Sales Connect] attività con [!DNL Salesforce] {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Quando si attiva la sincronizzazione tra [!DNL Sales Connect] e [!DNL Salesforce] attività, le attività [!DNL Salesforce] vengono importate. **non** eseguirà il push delle attività correnti in [!DNL Sales Connect] a [!DNL Salesforce]. Per ridurre l&#39;ingombro e i duplicati, le uniche attività sincronizzate da [!DNL Sales Connect] in [!DNL Salesforce] sono le attività create *dopo* la sincronizzazione di [!DNL Sales Connect] con SFDC.

Ecco cosa accade quando si sincronizzano [!DNL Sales Connect] e le attività di SFDC:

- Non appena si fa clic su Salva durante la sincronizzazione delle attività, queste vengono sincronizzate. Inizialmente questo richiederà del tempo.

- Tutti i promemoria aggiornati o creati nelle ultime 24 ore verranno inseriti da SFDC a [!DNL Sales Connect]. La sincronizzazione è basata sulla data di scadenza e tutte queste attività verranno sincronizzate nel back-end, ma in Centro comandi verranno visualizzate solo le attività in scadenza oggi e domani.

- Se la sincronizzazione è stata attivata in precedenza ed è stata eliminata qualsiasi attività in SFDC, qualsiasi elemento eliminato negli ultimi 15 giorni verrà eliminato da Centro comandi.

- Le attività verranno sincronizzate costantemente tra [!DNL Sales Connect] e SFDC, purché la sincronizzazione sia abilitata.

Dopo la sincronizzazione iniziale, tutte le attività create, modificate, completate o eliminate in [!DNL Sales Connect] verranno sincronizzate con l&#39;elenco delle attività in [!DNL Salesforce]. E qualsiasi elemento creato, modificato, completato o eliminato in [!DNL Salesforce] aggiornerà l&#39;elenco delle attività in [!DNL Sales Connect].

Per attivare questa sincronizzazione, seleziona la casella di sincronizzazione nella [pagina Impostazioni](https://toutapp.com/login) dell&#39;applicazione Web.
