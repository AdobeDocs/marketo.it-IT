---
unique-page-id: 2953132
description: Campagne avanzate in batch e trigger - Documentazione di Marketo - Documentazione del prodotto
title: Campagne avanzate in batch e trigger
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
source-git-commit: 686530e63cffef89bc7b9cbf6affa862689c0a46
workflow-type: tm+mt
source-wordcount: '272'
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

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

Fai clic sul pulsante **Pianificazione** La scheda confermerà che la campagna intelligente è impostata su &quot;Batch&quot;.

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**Campagne avanzate in batch**

* Può essere pianificato per le ricorrenze, ad esempio giornaliere, settimanali e mensili. Puoi anche farli funzionare una sola volta.
* Sono visibili sul [vista programma](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). Qualsiasi elemento dopo un passaggio &quot;Wait&quot; (Attendi) all’interno della campagna intelligente non verrà incluso nella visualizzazione.

<br> 

## Trigger di una campagna avanzata {#trigger-smart-campaign}

>[!NOTE]
>
>**Definizione**
>
>Una campagna avanzata di attivazione interessa una persona alla volta in base a un evento attivato. Un esempio di trigger potrebbe essere fare clic su un collegamento in un’e-mail.

Se una campagna intelligente utilizza almeno un trigger all’interno della sezione dell’elenco avanzato, la modalità verrà automaticamente impostata su attivata.

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

Fai clic su **Pianificazione** La scheda conferma che la campagna intelligente è impostata su &quot;Attivato&quot;.

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**Attivazione di campagne avanzate**

* Impossibile pianificare le ricorrenze. Possono essere impostati solo su attivo o inattivo.
* È possibile impostare più di un trigger. Tuttavia, se viene attivato un trigger, le azioni della campagna vengono eseguite.

>[!TIP]
>
>Utilizza la [registro attività](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) per vedere cosa si è verificato passo dopo passo all’interno delle campagne intelligenti. Puoi trovare il registro attività nell’ultima scheda della pagina dei dettagli di una persona.
