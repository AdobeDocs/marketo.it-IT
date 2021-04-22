---
unique-page-id: 7512524
description: Best practice per elenchi avanzati - Documenti Marketo - Documentazione del prodotto
title: Best practice per gli elenchi avanzati
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Best practice per gli elenchi avanzati {#best-practices-for-smart-lists}

Gli elenchi avanzati sono lo strumento di query più potente nell&#39;universo di marketing. Trovano le persone che state cercando con velocità magica e facilità.

Per facilitarne l’utilizzo e ottimizzare le prestazioni, abbiamo creato un elenco di buone pratiche. Godetevi!

>[!NOTE]
>
>**Ogni cliente è diverso.** Più grande è il database, maggiore è l&#39;elaborazione. Più attività sono memorizzate, più tempo è necessario per le ricerche.
>
>Se stai riscontrando una lentezza, prova i suggerimenti qui sotto. Se il problema persiste, contatta il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. **Cronologia limiti:**  i filtri di cronologia (ad esempio i filtri di attività) sono tra le operazioni che richiedono più tempo e risorse. Se devi utilizzarli, prova a limitare l’intervallo di date al più breve possibile, in modo da ridurre il set di dati ricercabili.
1. **Limita gli elenchi smart nidificati:** quando crei un nuovo elenco smart, limita la quantità di filtri utilizzati per i membri dell’elenco avanzato. Questa operazione si chiama nidificazione di elenchi avanzati e ogni elenco smart a cui viene fatto riferimento aumenterà il tempo di elaborazione. È invece possibile fare riferimento a elenchi statici o utilizzare [segmentazione](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).
1. **Usa operatori positivi rispetto a negativi:** anche se i filtri &quot;non&quot; sono disponibili, devono cercare l’intero set di dati nella tua istanza, il che può richiedere molto tempo. I filtri &quot;is&quot; positivi sono in grado di sfruttare algoritmi di ricerca più efficaci.
1. **Evita &quot;contiene&quot;:** se disponi solo di dati parziali, i qualificatori &quot;inizia con&quot; produrranno risultati molto più veloci rispetto a &quot;contiene&quot;. &quot;Is&quot; sarà ancora più veloce. Evita di utilizzare &quot;contiene&quot; con più valori; i due insieme possono rallentare ulteriormente una campagna.
1. **Utilizza il campione casuale da solo:** il campione casuale è un filtro speciale. Utilizzalo da solo per mettere le tue persone in liste pre-fatte. Quindi basta usare &quot;Membro dell&#39;elenco&quot; per rendere la vostra lista intelligente super veloce. Il campione casuale funziona **NOT** con gli elenchi avanzati nidificati. Il filtro Campione casuale non funziona se si tratta del riferimento a Smart List per il filtro &quot;Membro di Smart List&quot;.
1. **Sii utile con i filtri di inattività -** Filtri come &quot;Non compilato modulo&quot; possono essere molto utili, ma richiedono una potenza di elaborazione molto maggiore.
1. **Incollare più valori significa** selezionare più valori. Mettetene troppe, però, e rallenterà molto.
1. **Presta attenzione quando aggiungi vincoli:** questi sono i piccoli dettagli di una regola e dei valori correlati. Più vincoli si aggiungono, più lento sarà il tempo di elaborazione.
1. **Semplifica le tue campagne -** 100+ regole indipendenti (l&#39;abbiamo visto!) ovviamente ci vorrà un po&#39; di tempo per il processo. Mantenere semplice e si noterà i guadagni di velocità - oltre sarà più facile per voi a capire.
1. **Includi il simbolo @ prima del nome di dominio quando utilizzi il filtro** **Indirizzo e-mail -** Questo lo rende più veloce la query. Esempio: Invece di utilizzare _e-mail contiene &#39;somedomain.com&#39;_, utilizza _e-mail contiene &#39;@somedomain.com_&#39;. Se utilizzi più indirizzi e-mail con &quot;contiene&quot;, TUTTI questi devono iniziare con &quot;@.&quot;

>[!TIP]
>
>Marketo può essere utilizzato in molti modi e alcune tecniche sono migliori per voi e la vostra azienda. Considera [i servizi professionali Marketo](https://pages2.marketo.com/72-hour-survival-guide.html) per rendere il tuo investimento brillante.
