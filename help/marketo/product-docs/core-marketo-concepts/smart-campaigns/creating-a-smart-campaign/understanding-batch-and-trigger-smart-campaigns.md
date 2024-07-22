---
unique-page-id: 2953132
description: Informazioni sulle campagne intelligenti batch e trigger - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulle campagne avanzate batch e trigger
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
feature: Smart Campaigns
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---

# Informazioni sulle campagne avanzate batch e trigger {#understanding-batch-and-trigger-smart-campaigns}

Esistono due tipi di campagne intelligenti: Batch e Trigger.

## Campagna batch {#batch-campaign}

>[!NOTE]
>
>**Definizione**
>
>Una campagna batch viene avviata in un momento specifico e interessa un gruppo specifico di persone tutte contemporaneamente. Un esempio potrebbe essere l&#39;invio di un&#39;e-mail a tutte le persone in California.

Le campagne batch avranno solo filtri all’interno della sezione dell’elenco avanzato (ovvero, nessun trigger).

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

Facendo clic sulla scheda **[!UICONTROL Pianifica]** verrà confermato che Smart Campaign è impostata su &quot;Batch&quot;.

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**Campagne Smart In Batch**

* Può essere programmato per le ricorrenze, ad esempio giornaliere, settimanali e mensili. È inoltre possibile eseguirli una sola volta.
* Sono visibili nella [visualizzazione pianificazione programmi](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md){target="_blank"}. Qualsiasi elemento che risulti dopo un passaggio &quot;Attendi&quot; all’interno di Smart Campaign non verrà incluso nella visualizzazione.

<br> 

## Attiva campagna {#trigger-campaign}

>[!NOTE]
>
>**Definizione**
>
>Una campagna Trigger influisce su una persona alla volta in base a un evento attivato. Ad esempio, un trigger potrebbe fare clic su un collegamento in un messaggio e-mail.

Se una campagna avanzata utilizza almeno un trigger nella sezione Elenco avanzato, la modalità viene impostata automaticamente su Attivato.

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

Facendo clic sulla scheda **[!UICONTROL Pianificazione]**, verrà confermato che Smart Campaign è impostata su &quot;Attivato&quot;.

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**Attiva campagne**

* Impossibile pianificare le ricorrenze. Possono essere impostate solo su attive o inattive.
* È possibile impostare più attivatori. Tuttavia, se viene attivato un trigger, verranno eseguite le azioni della campagna.

>[!TIP]
>
>Utilizza il [registro attività](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"} per vedere cosa è successo passo dopo passo all&#39;interno delle campagne avanzate. Puoi trovare il registro attività nell’ultima scheda della pagina dei dettagli di una persona.
