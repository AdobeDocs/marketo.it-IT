---
unique-page-id: 1147001
description: Scopri come utilizzare la logica standard della regola di elenco avanzato in una campagna avanzata. Combina i filtri con la logica AND per la qualifica.
title: Utilizzare la logica standard per le regole di elenchi avanzati
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/hRPdzjEUOeC2PZK2YlO1IPZOPoPOfo7CHJu2yUtU0qc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
ht-degree: 10%

---

# Utilizzare la logica standard per le regole di elenchi avanzati {#using-standard-smart-list-rule-logic}

Potresti aver notato l’opzione &quot;Usa filtri&quot; durante la creazione degli elenchi avanzati delle campagne. Questa impostazione consente di decidere se i filtri devono essere valutati con un operatore AND o OR.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>La modifica della logica della regola dell&#39;elenco smart si applica solo ai filtri, _not_ trigger.

Gli attivatori vengono sempre valutati come OR anche se l’impostazione precedente è impostata su ALL. Ad esempio:

![](assets/using-standard-smart-list-rule-logic-2.png)

L’elenco avanzato di cui sopra in parole:

```box
IF person fills out Great Form
OR
IF person visits Keith's Landing Page
AND
Industry is Energy
AND
Country is US
THEN follow the campaign's flow step(s)
```

Pertanto, se una persona compila il modulo _o_ visita la pagina, la campagna valuterà tale persona in base a _all_ o _any_ dei filtri successivi, a seconda dell&#39;impostazione utilizzata.

>[!MORELIKETHIS]
>
>[Utilizzo della logica avanzata dell&#39;elenco smart](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}
