---
unique-page-id: 14352541
description: Sincronizzazione delle attività di vendita con Salesforce per la prima volta - Documentazione di Marketo - Documentazione del prodotto
title: Sincronizzazione per la prima volta delle attività Sales Connect con Salesforce
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Sincronizzazione per la prima volta delle attività Sales Connect con Salesforce {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Quando attivi per la prima volta la sincronizzazione tra le attività Sales Connect e Salesforce, le attività Salesforce vengono importate. Lo faremo **non** eseguire il push di tutte le attività correnti disponibili in Sales Connect a Salesforce. Per ridurre il disordine e i duplicati, le uniche attività sincronizzate da Sales Connect a Salesforce sono le attività create *dopo* sincronizzi Sales Connect con SFDC.

Ecco cosa accade quando si sincronizzano le attività Sales Connect e SFDC:

- Non appena si fa clic su Salva durante la sincronizzazione delle attività, queste vengono sincronizzate. Inizialmente questo richiederà del tempo.

- Tutti i promemoria aggiornati o creati nelle ultime 24 ore verranno inseriti da SFDC a Sales Connect. La sincronizzazione è basata sulla data di scadenza e tutte queste attività verranno sincronizzate nel back-end, ma in Centro comandi verranno visualizzate solo le attività in scadenza oggi e domani.

- Se la sincronizzazione è stata attivata in precedenza ed è stata eliminata qualsiasi attività in SFDC, qualsiasi elemento eliminato negli ultimi 15 giorni verrà eliminato da Centro comandi.

- Sincronizzeremo costantemente le attività tra Sales Connect e SFDC, purché la sincronizzazione sia abilitata.

Dopo la sincronizzazione iniziale, tutte le attività create, modificate, completate o eliminate in Sales Connect verranno sincronizzate con l&#39;elenco delle attività in Salesforce. E tutto ciò che viene creato, modificato, completato o eliminato in Salesforce aggiorna l&#39;elenco delle attività in Sales Connect.

Per attivare questa sincronizzazione, seleziona la casella di sincronizzazione nel [Pagina Impostazioni](https://toutapp.com/login) nell’applicazione web.
