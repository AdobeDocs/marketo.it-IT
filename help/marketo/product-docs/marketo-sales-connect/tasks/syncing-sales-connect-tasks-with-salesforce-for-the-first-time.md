---
unique-page-id: 14352541
description: Sincronizzazione delle attività di vendita con Salesforce per la prima volta - Marketo Docs - Documentazione del prodotto
title: Sincronizzazione delle attività di vendita con Salesforce per la prima volta
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Sincronizzazione delle attività di vendita con Salesforce per la prima volta {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Quando attivi per la prima volta la sincronizzazione tra le attività di Sales Connect e Salesforce, importiamo le attività di Salesforce. Lo faremo **not** sovrascrivi tutte le attività correnti in Sales Connect to Salesforce. Per ridurre il disordine e i duplicati, le uniche attività che vengono sincronizzate da Sales Connect in Salesforce sono le attività create *dopo* è possibile sincronizzare Sales Connect con SFDC.

Ecco cosa succede quando si sincronizzano le attività di Sales Connect e SFDC:

- Non appena fai clic su salva nella sincronizzazione delle attività, queste iniziano a sincronizzarsi. Inizialmente ci vorrà un po&#39; di tempo.

- Eventuali promemoria aggiornati o creati nelle ultime 24 ore verranno inviati da SFDC a Sales Connect. La sincronizzazione è basata sulla data di scadenza e tutte le attività verranno sincronizzate sul back-end, ma in Command Center verranno visualizzate solo le attività scadute oggi e domani.

- Se la sincronizzazione è stata attivata in precedenza ed elimini eventuali attività in SFDC, tutto ciò che è stato eliminato negli ultimi 15 giorni verrà eliminato dal Centro comandi.

- Le attività verranno sincronizzate costantemente tra Sales Connect e SFDC purché la sincronizzazione sia abilitata.

Dopo la sincronizzazione iniziale, tutte le attività create, modificate, completate o eliminate in Sales Connect verranno sincronizzate nell&#39;elenco delle attività in Salesforce. E qualsiasi cosa creata, modificata, completata o eliminata in Salesforce aggiornerà l&#39;elenco delle attività in Sales Connect.

Per attivare questa sincronizzazione, controlla la casella di sincronizzazione nel tuo [Pagina Impostazioni](https://toutapp.com/login) nell&#39;applicazione web.
