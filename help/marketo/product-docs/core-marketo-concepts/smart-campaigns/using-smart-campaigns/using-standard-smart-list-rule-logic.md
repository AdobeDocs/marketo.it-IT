---
unique-page-id: 1147001
description: Utilizzo della regola standard per gli elenchi avanzati - Documenti Marketo - Documentazione del prodotto
title: Utilizzo della logica standard delle regole per gli elenchi avanzati
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---


# Utilizzo della logica standard delle regole per gli elenchi avanzati {#using-standard-smart-list-rule-logic}

Potreste aver notato l&#39;opzione &quot;Usa filtri&quot; durante la creazione di elenchi smart delle campagne. Questa impostazione consente di decidere se i filtri devono essere valutati con un operatore AND o OR.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>La modifica della logica della regola dell&#39;elenco smart si applica solo ai filtri, **non** agli attivatori.

Gli attivatori vengono sempre valutati come OR anche se l&#39;impostazione precedente è impostata su ALL.  Esempio:

![](assets/image2014-9-22-14-3a12-3a57.png)

L&#39;elenco avanzato in parole:
`<pre data-theme="Confluence">IF person fills out My Form OR IF person visits My Page AND Industry is Marketing AND Country is USA THEN follow the campaign's flow step(s)</pre>` Quindi, se una persona compila il modulo **** o visita la pagina, la campagna valuterà la persona in base a **all **o **any **any **of the next filter, a seconda dell&#39;impostazione utilizzata.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Utilizzo della logica delle regole avanzate per gli elenchi avanzati](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)

>



