---
unique-page-id: 2953132
description: Campagne intelligenti per batch e trigger - Documenti Marketo - Documentazione prodotto
title: Informazioni sulle campagne in batch e di attivazione
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---


# Informazioni sulle campagne in batch e di attivazione {#understanding-batch-and-trigger-smart-campaigns}

Esistono due tipi di campagne intelligenti: Batch e Trigger.

>[!NOTE]
>
>**FYI**
>
>Marketo sta ora standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che l&#39;iscrizione contenga lead/lead e la persona/persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

## Batch Smart Campaign {#batch-smart-campaign}

>[!NOTE]
>
>**Definizione**
>
>Una campagna batch viene avviata in un momento specifico e interessa un set specifico di persone tutte contemporaneamente. Un esempio potrebbe essere l&#39;invio di un&#39;e-mail a tutte le persone in California.

Le campagne smart in batch includeranno solo filtri nella sezione degli elenchi smart (ovvero, nessun trigger).

![](assets/batch-filter.png)

Facendo clic sulla scheda **Schedule (Pianificazione** ), verrà confermato che la campagna smart è impostata su &quot;Batch&quot;.

![](assets/batch-c4.png)

**Campagne intelligenti in batch**

* Può essere pianificato per le ricorrenze, ad esempio giornaliere, settimanali e mensili. Potete anche farli correre una sola volta.
* Sono visibili nella vista [Pianificazione](../../../../product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md)programma.\
   *Si noti che qualsiasi cosa dopo un passaggio &quot;Wait&quot; all&#39;interno della campagna intelligente non sarà incluso nella vista.

<br> 

## Attivate Smart Campaign {#trigger-smart-campaign}

>[!NOTE]
>
>**Definizione**
>
>Una campagna intelligente di attivazione interessa una persona alla volta in base a un evento attivato. Un esempio di attivatore potrebbe consistere nel fare clic su un collegamento in un messaggio e-mail.

Se una campagna intelligente utilizza almeno un trigger all&#39;interno della sezione dell&#39;elenco smart, la modalità verrà automaticamente attivata.

![](assets/trigger.png)

Facendo clic sulla scheda **Pianificazione** , si confermerà che la campagna intelligente è impostata su &quot;Attivato&quot;.

![](assets/trigger2.png)

**Attiva campagne intelligenti**

* Impossibile pianificare le ricorrenze. Possono essere impostati solo su attivi o inattivi.
* È possibile impostare più attivatori. Tuttavia, se viene attivato un attivatore, le azioni della campagna verranno eseguite.

## Video sulla creazione di campagne e-mail attivate {#watch-a-video-on-creating-triggered-email-campaigns}

`<iframe width="630" height="470" src="//play.vidyard.com/6zNazwTgt2LNeCjPAt3W9K.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

>[!TIP]
>
>Utilizzate il registro [delle](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) attività per vedere cosa si è verificato passo dopo passo all&#39;interno delle campagne intelligenti. Potete trovare il registro attività nell&#39;ultima scheda della pagina dei dettagli di una persona.

