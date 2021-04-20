---
title: Understanding-batch-and-trigger-smart-campagne
description: Campagne avanzate in batch e trigger
exl-id: 54f38ecc-1b4c-4944-9f42-d8c1190c99d0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Campagne avanzate in batch e trigger

<br> 

Esistono due tipi di campagne intelligenti: Batch e Trigger.

## Campagna avanzata in batch

Una campagna batch viene avviata in un momento specifico e influisce su un set specifico di persone tutte contemporaneamente. Un esempio potrebbe essere l&#39;invio di un&#39;e-mail a tutti coloro che vivono in California nel tuo database.

Le campagne smart in batch avranno solo filtri all’interno della sezione dell’elenco avanzato (ovvero, nessun trigger).

![Immagine uno](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

Facendo clic sulla scheda **[!UICONTROL Schedule]** verrà confermato che la campagna avanzata è impostata su &quot;Batch&quot;.

![Immagine 2](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**Campagne avanzate in batch**

* Può essere pianificato per le ricorrenze, ad esempio giornaliere, settimanali e mensili. Puoi anche farli funzionare una sola volta.
* Sono visibili nella [visualizzazione programmazione programma](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View).
* Qualsiasi elemento dopo un passaggio &quot;Wait&quot; (Attendi) all’interno della campagna intelligente non verrà incluso nella visualizzazione.

## Trigger di una campagna avanzata

Una campagna avanzata di attivazione interessa una persona alla volta in base a un evento attivato. Un esempio di trigger potrebbe essere fare clic su un collegamento in un’e-mail.

Se una campagna intelligente utilizza almeno un trigger all’interno della sezione dell’elenco avanzato, la modalità verrà automaticamente impostata su attivata.

![Immagine tre](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

Fai clic sulla scheda **[!UICONTROL Schedule]** per confermare che la campagna avanzata è impostata su &quot;Attivatore&quot;.

![Immagine quattro](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**Attivazione di campagne avanzate**

* Impossibile pianificare le ricorrenze. Possono essere impostati solo su attivo o inattivo.
* È possibile impostare più di un trigger. Tuttavia, se viene attivato un trigger _qualsiasi_, le azioni della campagna verranno eseguite.

>[!TIP]
>
>Utilizza il [registro attività](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person) per vedere cosa si è verificato passo dopo passo all&#39;interno delle campagne intelligenti. Puoi trovare il registro attività nell’ultima scheda della pagina dei dettagli di una persona.
