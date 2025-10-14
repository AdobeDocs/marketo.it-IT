---
unique-page-id: 7512524
description: Best practice per elenchi avanzati - Documentazione di Marketo - Documentazione del prodotto
title: Best practice per gli elenchi avanzati
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 1%

---

# Best practice per gli elenchi avanzati {#best-practices-for-smart-lists}

Gli elenchi avanzati sono lo strumento di query più potente nell’universo del marketing. Trovano le persone che stai cercando con velocità e facilità magiche.

Per semplificarne l’utilizzo e ottimizzare le prestazioni, abbiamo creato un elenco di best practice. Buon lavoro!

>[!NOTE]
>
>**Ogni utente di Marketo Engage è diverso.** Più grande è il database, maggiore sarà l&#39;elaborazione. Maggiore è il numero di attività memorizzate, maggiore sarà il tempo necessario per la ricerca.
>
>In caso di rallentamento, provare i suggerimenti riportati di seguito. Se il problema persiste, contattare il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. **Cronologia limite -** I filtri cronologia (ovvero i filtri attività) sono tra le operazioni che richiedono più tempo e risorse. Se devi utilizzarli, prova a limitare l’intervallo di date al più breve possibile, in modo da ridurre il set di dati ricercabile. Inoltre, gli intervalli di date non sostituiscono i periodi di conservazione. Esempio: se l&#39;attività di cui si sta eseguendo una query ha un periodo di conservazione di 90 giorni e si sceglie &quot;ultimi 100 giorni&quot;, verranno restituiti solo i risultati degli ultimi 90 giorni. I periodi di conservazione delle attività [&#x200B; si trovano qui](https://nation.marketo.com/t5/knowledgebase/marketo-activities-data-retention-policy/ta-p/251480){target="_blank"}.
1. **Limita elenchi smart nidificati -** Quando si crea un nuovo elenco smart, limitare la quantità di filtri &quot;Membro di elenco smart&quot; utilizzati. Questa operazione è denominata nidificazione di elenchi avanzati e ogni elenco avanzato a cui si fa riferimento aumenterà il tempo di elaborazione. Fare riferimento a elenchi statici o utilizzare [segmentazione](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md){target="_blank"}.
1. **Utilizzare operatori positivi su negativi -** I filtri &quot;non&quot; sono disponibili, ma devono cercare l&#39;intero set di dati nell&#39;istanza, operazione che può richiedere molto tempo. I filtri &quot;is&quot; positivi sono in grado di sfruttare algoritmi di ricerca più efficaci.
1. **Evita &quot;contiene&quot; -** Se disponi solo di dati parziali, i qualificatori &quot;inizia con&quot; produrranno risultati molto più veloci di &quot;contiene&quot;. &quot;Is&quot; funziona ancora più velocemente. Evita di utilizzare &quot;contiene&quot; con più valori; i due insieme possono rallentare ulteriormente una campagna.
1. **Utilizzare il campione casuale da solo -** Il campione casuale è un filtro speciale. Utilizzalo da solo per inserire le tue persone in elenchi predefiniti. Quindi utilizza &quot;Membro dell’elenco&quot; per rendere il tuo elenco avanzato super veloce. Il campione casuale **NOT** funzionerà con elenchi avanzati nidificati. Il filtro Campione casuale non funziona se si tratta dell’elenco avanzato a cui si fa riferimento per il filtro &quot;Membro dell’elenco avanzato&quot;.
1. **Risparmia con i filtri di inattività -** I filtri come &quot;Modulo non compilato&quot; possono essere molto utili, ma richiedono una potenza di elaborazione molto maggiore.
1. **Risparmia con l&#39;incollare più valori -** La selezione multipla è progettata per incollare decine o forse centinaia di valori. Mettine troppe, però, e rallenterà molto.
1. **Risparmia quando aggiungi vincoli -** Questi sono i piccoli dettagli di una regola e dei valori correlati. Maggiore è il numero di vincoli aggiunti, più lento sarà il tempo di elaborazione.
1. **Semplifica le tue campagne -** Oltre 100 regole indipendenti (ne abbiamo viste!) richiederanno ovviamente un po&#39; di tempo per l&#39;elaborazione. Semplificalo e noterai i guadagni di velocità - oltre a sarà più facile da capire.
1. **Includere il simbolo @ prima del nome di dominio quando si utilizza il filtro Indirizzo e-mail** **-** In questo modo si utilizza una query più veloce. Esempio: invece di utilizzare _email contiene &#39;somedomain.com&#39;_, utilizzare _email contiene &#39;@somedomain.com_.&#39; Se utilizzi più indirizzi e-mail con &quot;contiene&quot;, TUTTI devono iniziare con &quot;@.&quot;

>[!TIP]
>
>Marketo Engage può essere utilizzato in molti modi e alcune tecniche sono migliori per te e la tua azienda. Contatta il tuo rappresentante commerciale Adobe Professional Services per ottenere il massimo dal tuo investimento.
