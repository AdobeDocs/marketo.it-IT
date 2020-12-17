---
unique-page-id: 7512524
description: Best practice per Smart List - Marketo Docs - Documentazione prodotto
title: Best practice per gli elenchi avanzati
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---


# Best practice per gli elenchi smart {#best-practices-for-smart-lists}

Gli elenchi intelligenti sono lo strumento di query più potente nell&#39;universo di marketing. Trovano le persone che state cercando con la velocità magica e la facilità.

Per semplificare l&#39;utilizzo e ottimizzare le prestazioni, abbiamo creato un elenco di buone pratiche. Divertiti!

>[!NOTE]
>
>**Ogni cliente è diverso.** Più grande è il database, maggiore è l&#39;elaborazione. Più attività sono memorizzate, più tempo è necessario per le ricerche.
>
>Se si verifica un rallentamento, provare i suggerimenti riportati di seguito. Se il problema persiste, contattare Marketo [Supporto](http://support.marketo.com).

1. **Cronologia limite - **Filtri storia (anche noti come Filtri attività) sono tra le operazioni che richiedono più tempo e risorse. Se devi utilizzarli, prova a limitare l’intervallo di date al più breve possibile, riducendo così il set di dati ricercabili.
1. **Limita elenchi smart nidificati - **Durante la creazione di un nuovo elenco smart, limitare la quantità di filtri &quot;Member of Smart List&quot; utilizzati. Questa operazione è denominata nidificazione di elenchi avanzati e ogni elenco smart a cui viene fatto riferimento aumenta il tempo di elaborazione. Al contrario, potete fare riferimento a elenchi statici o utilizzare [segmentazione](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).
1. **Utilizzare operatori positivi rispetto a quelli negativi - **I filtri &quot;non&quot; sono disponibili, devono cercare l&#39;intero set di dati nell&#39;istanza, che può essere estremamente lungo. I filtri &quot;is&quot; positivi sono in grado di sfruttare algoritmi di ricerca più efficaci.
1. **Evitare &quot;contains&quot; -** Se hai solo dati parziali, &quot;inizia con&quot; qualificatori darà risultati molto più veloci di &quot;contiene&quot;. &quot;Is&quot; sarà ancora più veloce. evitare di utilizzare &quot;contains&quot; con più valori; i due insieme possono rallentare ulteriormente una campagna.
1. **Utilizzare il campione casuale da solo - **Il campione casuale è un filtro speciale. Utilizzatelo da solo per inserire le persone in elenchi precompilati. Quindi basta utilizzare &quot;Member of List&quot; per rendere la vostra lista intelligente super veloce. Esempio casuale: **NOT** funziona con gli elenchi avanzati nidificati. Il filtro Esempio casuale non funziona se si tratta dell’Elenco avanzato a cui viene fatto riferimento per il filtro &quot;Membro di Elenco avanzato&quot;.
1. **Essere parsimoniosi con i filtri di inattività - **Filtri come &quot;Forma non riempita&quot; possono essere molto utili, ma richiedono molta più potenza di elaborazione.
1. **Essere parsimonioso con incollare in più valori - **Multi-select è progettato per incollare in dozzine o forse centinaia di valori. Mettetene troppi, ma rallenta.
1. **Sii prudente quando aggiungi vincoli - **Questi sono i piccoli dettagli di una regola e i relativi valori. Maggiore è il numero di vincoli aggiunti, minore sarà il tempo di elaborazione.
1. **Semplificare le campagne - **100+ regole indipendenti (l&#39;abbiamo visto!) ovviamente ci vorrà un po&#39; di tempo per l&#39;elaborazione. Tenetelo semplice e noterete i guadagni di velocità - più sarà più facile da capire per voi.
1. **Includere il simbolo @ prima del nome del dominio quando si utilizza il filtro** **Indirizzo e-mail -** Questo consente di utilizzare una query più veloce. Esempio: Invece di utilizzare *email contains &#39;somedomain.com*&#39;, utilizzare *email contains &#39;@somedomain.com*&#39;. Se utilizzi più indirizzi e-mail con &quot;contains&quot;, TUTTI questi devono iniziare con &quot;@&quot;.

>[!TIP]
>
>Marketo può essere utilizzato in molti modi e alcune tecniche sono migliori per voi e la vostra azienda. Considerare i servizi professionali [Marketo](http://pages2.marketo.com/72-hour-survival-guide.html) per rendere il vostro investimento brillante.

