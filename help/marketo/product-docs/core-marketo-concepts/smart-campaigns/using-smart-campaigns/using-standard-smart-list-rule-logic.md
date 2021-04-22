---
unique-page-id: 1147001
description: Utilizzo della logica delle regole dell’elenco avanzato standard - Documenti Marketo - Documentazione del prodotto
title: Utilizzo della logica delle regole dell’elenco avanzato standard
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Utilizzo della logica delle regole di elenco avanzato standard {#using-standard-smart-list-rule-logic}

È possibile che abbiate notato l’opzione &quot;Use filters&quot; (Usa filtri) durante la creazione di elenchi avanzati di campagne. Questa impostazione consente di decidere se i filtri devono essere valutati con un operatore AND o OR.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>La modifica della logica delle regole dell’elenco smart si applica solo ai filtri, ai trigger **not**.

Gli attivatori vengono sempre valutati come OR anche se l&#39;impostazione precedente è impostata su ALL.  Ecco un esempio:

![](assets/image2014-9-22-14-3a12-3a57.png)

L&#39;elenco smart riportato sopra in parole:

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

Pertanto, se una persona compila il modulo **o** visita la pagina, la campagna valuterà tale persona in base a **all** o **any** dei filtri successivi, a seconda delle impostazioni utilizzate.

>[!MORELIKETHIS]
>
>[Utilizzo della logica avanzata delle regole dell’elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
