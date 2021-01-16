---
unique-page-id: 2953132
description: Campagne intelligenti per batch e trigger - Documenti Marketo - Documentazione prodotto
title: Informazioni sulle campagne in batch e di attivazione
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Campagne avanzate in batch e trigger {#understanding-batch-and-trigger-smart-campaigns}

Esistono due tipi di campagne intelligenti: Batch e Trigger.

## Batch Smart Campaign {#batch-smart-campaign}

>[!NOTE]
>
>**Definizione**
>
>Una campagna batch viene avviata in un momento specifico e interessa un set specifico di persone tutte contemporaneamente. Un esempio potrebbe essere l&#39;invio di un&#39;e-mail a tutte le persone in California.

Le campagne smart in batch includeranno solo filtri nella sezione degli elenchi smart (ovvero, nessun trigger).

![](assets/batch-filter.png)

Facendo clic sulla scheda **Schedule** (Pianificazione), verrà confermato che la campagna smart è impostata su &quot;Batch&quot;.

![](assets/batch-c4.png)

**Campagne intelligenti in batch**

* Può essere pianificato per le ricorrenze, ad esempio giornaliere, settimanali e mensili. Potete anche farli correre una sola volta.
* Sono visibili nella [vista programmazione programma](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). Tutto ciò che segue un passaggio &quot;Wait&quot; all&#39;interno della campagna intelligente non verrà incluso nella vista.

<br> 

## Trigger Smart Campaign {#trigger-smart-campaign}

>[!NOTE]
>
>**Definizione**
>
>Una campagna intelligente di attivazione interessa una persona alla volta in base a un evento attivato. Un esempio di attivatore potrebbe consistere nel fare clic su un collegamento in un messaggio e-mail.

Se una campagna intelligente utilizza almeno un trigger all&#39;interno della sezione dell&#39;elenco smart, la modalità verrà automaticamente attivata.

![](assets/trigger.png)

Facendo clic sulla scheda **Schedule** (Pianificazione), verrà confermato che la campagna smart è impostata su &quot;Triggered&quot; (Attivazione).

![](assets/trigger2.png)

**Attiva campagne intelligenti**

* Impossibile pianificare le ricorrenze. Possono essere impostati solo su attivi o inattivi.
* È possibile impostare più attivatori. Tuttavia, se viene attivato un attivatore, le azioni della campagna verranno eseguite.

>[!TIP]
>
>Utilizzate il [registro attività](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) per vedere cosa si è verificato passo dopo passo all&#39;interno delle campagne intelligenti. Potete trovare il registro attività nell&#39;ultima scheda della pagina dei dettagli di una persona.
