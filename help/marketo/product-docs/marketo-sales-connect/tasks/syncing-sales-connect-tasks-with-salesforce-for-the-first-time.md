---
unique-page-id: 14352541
description: Sincronizzazione delle attività di vendita Connect con Salesforce per la prima volta - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione delle attività di vendita Connect con Salesforce per la prima volta
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Sincronizzazione delle attività di vendita Connect con Salesforce per la prima volta {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

La prima volta che attivi la sincronizzazione tra le attività di Sales Connect e Salesforce, importiamo le attività di Salesforce. **Non** eseguiremo il push delle attività correnti di cui disponete in Sales Connect per Salesforce. Per ridurre il disordine e i duplicati, le uniche attività che vengono sincronizzate da Sales Connect a Salesforce sono le attività create *dopo* la sincronizzazione di Sales Connect con SFDC.

Ecco cosa accade quando si sincronizzano le attività di Sales Connect e SFDC:

- Non appena si fa clic su Salva per sincronizzare le attività, queste iniziano a sincronizzarsi. Inizialmente, questa operazione richiederà un po&#39; di tempo.

- Eventuali promemoria che sono stati aggiornati o creati in `last 24 hours` verranno inseriti da SFDC a Sales Connect. La sincronizzazione è basata su `due date` e tutte queste attività verranno sincronizzate sul back-end, ma nel centro comandi verranno visualizzate solo le attività previste oggi e domani.

- Se la sincronizzazione è stata attivata in precedenza ed è stata eliminata qualsiasi attività in SFDC, tutto ciò che è stato eliminato negli ultimi 15 giorni verrà eliminato dal Centro comandi.

- Le attività verranno sincronizzate costantemente tra Sales Connect e SFDC finché la sincronizzazione sarà abilitata.

Dopo la sincronizzazione iniziale, tutte le attività create, modificate, completate o eliminate in Sales Connect verranno sincronizzate nell&#39;elenco delle attività in Salesforce. Inoltre, qualsiasi cosa creata, modificata, completata o eliminata in Salesforce aggiornerà l&#39;elenco delle attività in Sales Connect.

Per attivare questa sincronizzazione, è sufficiente selezionare la casella di sincronizzazione nella pagina [](http://toutapp.com/next#settings/crm/salesforce/configure) Impostazioni dell&#39;applicazione Web.

