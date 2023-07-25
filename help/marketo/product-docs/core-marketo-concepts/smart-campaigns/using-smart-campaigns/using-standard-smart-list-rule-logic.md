---
unique-page-id: 1147001
description: Utilizzo della logica standard per la regola dell’elenco avanzato - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo della logica standard per le regole di elenchi avanzati
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Utilizzo della logica standard per le regole di elenchi avanzati {#using-standard-smart-list-rule-logic}

Potresti aver notato l’opzione &quot;Usa filtri&quot; durante la creazione degli elenchi avanzati delle campagne. Questa impostazione consente di decidere se i filtri devono essere valutati con un operatore AND o OR.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>La modifica della logica della regola dell’elenco avanzato si applica solo ai filtri, **non** trigger.

Gli attivatori vengono sempre valutati come OR anche se l’impostazione precedente è impostata su ALL.  Ecco un esempio:

![](assets/image2014-9-22-14-3a12-3a57.png)

L’elenco avanzato di cui sopra in parole:

```box
IF person fills out My Form
OR
IF person visits My Page 
AND 
Industry is Marketing 
AND 
Country is USA 
THEN follow the campaign's flow step(s)
```

Quindi, se una persona compila il modulo **o** visita la pagina, la campagna valuterà quindi tale persona in base a **tutto** o **qualsiasi** dei filtri successivi, a seconda dell’impostazione utilizzata.

>[!MORELIKETHIS]
>
>[Utilizzo della logica avanzata della regola di elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
