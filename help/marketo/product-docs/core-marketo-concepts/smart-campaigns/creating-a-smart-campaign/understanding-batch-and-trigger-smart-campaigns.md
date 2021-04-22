---
unique-page-id: 2953132
description: Campagne avanzate in batch e trigger - Documentazione di Marketo - Documentazione del prodotto
title: Campagne avanzate in batch e trigger
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Campagne avanzate in batch e trigger {#understanding-batch-and-trigger-smart-campaigns}

Esistono due tipi di campagne intelligenti: Batch e Trigger.

## Campagna avanzata in batch {#batch-smart-campaign}

>[!NOTE]
>
>**Definizione**
>
>Una campagna batch viene avviata in un momento specifico e influisce su un set specifico di persone tutte contemporaneamente. Un esempio potrebbe essere l&#39;invio di un&#39;e-mail a tutte le persone in California.

Le campagne smart in batch avranno solo filtri all’interno della sezione dell’elenco avanzato (ovvero, nessun trigger).

![](assets/batch-filter.png)

Facendo clic sulla scheda **Pianificazione** si verifica che la campagna avanzata sia impostata su &quot;Batch&quot;.

![](assets/batch-c4.png)

**Campagne avanzate in batch**

* Può essere pianificato per le ricorrenze, ad esempio giornaliere, settimanali e mensili. Puoi anche farli funzionare una sola volta.
* Sono visibili nella [visualizzazione programmazione programma](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). Qualsiasi elemento dopo un passaggio &quot;Wait&quot; (Attendi) all’interno della campagna intelligente non verrà incluso nella visualizzazione.

<br> 

## Trigger della campagna avanzata {#trigger-smart-campaign}

>[!NOTE]
>
>**Definizione**
>
>Una campagna avanzata di attivazione interessa una persona alla volta in base a un evento attivato. Un esempio di trigger potrebbe essere fare clic su un collegamento in un’e-mail.

Se una campagna intelligente utilizza almeno un trigger all’interno della sezione dell’elenco avanzato, la modalità verrà automaticamente impostata su attivata.

![](assets/trigger.png)

Facendo clic sulla scheda **Schedule** (Pianificazione), la campagna avanzata viene impostata su &quot;Triggered&quot; (Attivato).

![](assets/trigger2.png)

**Attivazione di campagne avanzate**

* Impossibile pianificare le ricorrenze. Possono essere impostati solo su attivo o inattivo.
* È possibile impostare più di un trigger. Tuttavia, se viene attivato un trigger, le azioni della campagna vengono eseguite.

>[!TIP]
>
>Utilizza il [registro attività](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) per vedere cosa si è verificato passo dopo passo all&#39;interno delle campagne intelligenti. Puoi trovare il registro attività nell’ultima scheda della pagina dei dettagli di una persona.
