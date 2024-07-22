---
unique-page-id: 1147001
description: Utilizzo della logica standard per la regola dell’elenco avanzato - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo della logica standard per le regole di elenchi avanzati
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Utilizzo della logica standard per le regole di elenchi avanzati {#using-standard-smart-list-rule-logic}

Potresti aver notato l’opzione &quot;Usa filtri&quot; durante la creazione degli elenchi avanzati delle campagne. Questa impostazione consente di decidere se i filtri devono essere valutati con un operatore AND o OR.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>La modifica della logica della regola dell&#39;elenco smart si applica solo ai filtri, _not_ trigger.

Gli attivatori vengono sempre valutati come OR anche se l’impostazione precedente è impostata su ALL. Ecco un esempio:

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
