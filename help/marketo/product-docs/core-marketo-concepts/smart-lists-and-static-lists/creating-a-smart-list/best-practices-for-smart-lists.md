---
unique-page-id: 7512524
description: Best practice per elenchi avanzati - Documentazione di Marketo - Documentazione del prodotto
title: Best practice per gli elenchi avanzati
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
feature: Smart Lists
source-git-commit: b6628cee17799801815f5b84c424399538eaf5ee
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Best practice per gli elenchi avanzati {#best-practices-for-smart-lists}

Gli elenchi avanzati sono lo strumento di query più potente nell’universo del marketing. Trovano le persone che stai cercando con velocità e facilità magiche.

Per semplificarne l&#39;utilizzo e ottimizzare le prestazioni, è stato creato un elenco di buone pratiche. Buon lavoro!

>[!NOTE]
>
>**Ogni cliente è diverso.** Maggiore è la dimensione del database, maggiore sarà l&#39;elaborazione. Maggiore è il numero di attività memorizzate, maggiore sarà il tempo necessario per la ricerca.
>
>In caso di rallentamento, provare i suggerimenti riportati di seguito. Se il problema persiste, contattare [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. **Limita cronologia -** I filtri della cronologia, o filtri di attività, sono tra le operazioni che richiedono più tempo e risorse. Se devi utilizzarli, prova a limitare l’intervallo di date al più breve possibile, in modo da ridurre il set di dati ricercabile. Inoltre, gli intervalli di date non sostituiscono i periodi di conservazione. Esempio: se l&#39;attività di cui si sta eseguendo una query ha un periodo di conservazione di 90 giorni e si sceglie &quot;ultimi 100 giorni&quot;, verranno restituiti solo i risultati degli ultimi 90 giorni. Periodi di conservazione delle attività [si trova qui](https://nation.marketo.com/t5/knowledgebase/marketo-activities-data-retention-policy/ta-p/251480){target="_blank"}.
1. **Limita elenchi avanzati nidificati -** Quando crei un nuovo elenco avanzato, limita la quantità di filtri &quot;Membro di elenco avanzato&quot; utilizzati. Questa operazione è denominata nidificazione di elenchi avanzati e ogni elenco avanzato a cui si fa riferimento aumenterà il tempo di elaborazione. Al loro posto, puoi fare riferimento a elenchi statici o utilizzare [segmentazione](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md){target="_blank"}.
1. **Usa operatori positivi su negativi -** Anche se i filtri &quot;non&quot; sono disponibili, devono cercare l’intero set di dati nella tua istanza, il che può richiedere molto tempo. I filtri &quot;is&quot; positivi sono in grado di sfruttare algoritmi di ricerca più efficaci.
1. **Evita &quot;contiene&quot; -** Se disponi solo di dati parziali, i qualificatori &quot;inizia con&quot; produrranno risultati molto più veloci di &quot;contiene&quot;. &quot;Is&quot; funziona ancora più velocemente. Evita di utilizzare &quot;contiene&quot; con più valori; i due insieme possono rallentare ulteriormente una campagna.
1. **Usa solo campione casuale -** Campione casuale è un filtro speciale. Utilizzalo da solo per inserire le tue persone in elenchi predefiniti. Quindi utilizza &quot;Membro dell’elenco&quot; per rendere la tua lista intelligente super veloce. Campione casuale **NOT** utilizzare elenchi avanzati nidificati. Il filtro Campione casuale non funziona se si tratta dell’elenco avanzato a cui si fa riferimento per il filtro &quot;Membro dell’elenco avanzato&quot;.
1. **Essere parsimoniosi con i filtri di inattività -** I filtri come &quot;Modulo non compilato&quot; possono essere molto utili, ma richiedono una potenza di elaborazione molto maggiore.
1. **Essere parsimoniosi con l&#39;incollare in più valori -** La selezione multipla è progettata per incollare decine o forse centinaia di valori. Mettine troppe, però, e rallenterà molto.
1. **Mantenere la parsimonia quando si aggiungono vincoli -** Si tratta dei piccoli dettagli di una regola e dei valori correlati. Maggiore è il numero di vincoli aggiunti, più lento sarà il tempo di elaborazione.
1. **Semplificare le campagne -** Oltre 100 regole indipendenti (ne abbiamo viste!) l&#39;elaborazione richiederà ovviamente un po&#39; di tempo. Semplificalo e noterai i guadagni di velocità - oltre a sarà più facile da capire.
1. **Includi il simbolo @ prima del nome di dominio quando utilizzi il filtro Indirizzo e-mail** **-** In questo modo utilizza una query più veloce. Esempio: anziché utilizzare _l&#39;e-mail contiene &#39;somedomain.com&#39;_, utilizza _l&#39;e-mail contiene &#39;@somedomain.com_.&quot; Se utilizzi più indirizzi e-mail con &quot;contiene&quot;, TUTTI devono iniziare con &quot;@.&quot;

>[!TIP]
>
>Il Marketo Engage può essere utilizzato in molti modi e alcune tecniche sono migliori per te e la tua azienda. Contatta il tuo rappresentante commerciale Adobe Professional Services per ottenere il massimo dal tuo investimento.
