---
title: comprensivo di campagne intelligenti batch e trigger
description: Informazioni sulle campagne in batch e di attivazione
translation-type: tm+mt
source-git-commit: cd1b7e65c73de0b31f20289402f1c0832c382b33
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Informazioni sulle campagne in batch e di attivazione

<br> 

Esistono due tipi di campagne intelligenti: Batch e Trigger.

## Batch Smart Campaign

Una campagna batch viene avviata in un momento specifico e interessa un set specifico di persone tutte contemporaneamente. Un esempio potrebbe essere l&#39;invio di un&#39;e-mail a tutti coloro che vivono in California nel vostro database.

Le campagne smart in batch includeranno solo filtri nella sezione degli elenchi smart (ovvero, nessun trigger).

![Immagine uno](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

Facendo clic sulla scheda [!UICONTROL **Schedule (Pianificazione**] ), la campagna smart viene impostata su &quot;Batch&quot;.

![Immagine due](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**Campagne intelligenti in batch**

* Può essere pianificato per le ricorrenze, ad esempio giornaliere, settimanali e mensili. Potete anche farli correre una sola volta.
* Sono visibili nella vista [Pianificazione](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View)programma.
* Tutto ciò che segue un passaggio &quot;Wait&quot; all&#39;interno della campagna intelligente non verrà incluso nella vista.

## Attivate Smart Campaign

Una campagna intelligente di attivazione interessa una persona alla volta in base a un evento attivato. Un esempio di attivatore potrebbe consistere nel fare clic su un collegamento in un messaggio e-mail.

Se una campagna intelligente utilizza almeno un trigger all&#39;interno della sezione dell&#39;elenco smart, la modalità verrà automaticamente attivata.

![Immagine tre](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

Facendo clic sulla scheda [!UICONTROL **Schedule (Pianificazione**] ), la campagna smart viene impostata su &quot;Trigger&quot; (Attivatore).

![Immagine quattro](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**Attiva campagne intelligenti**

* Impossibile pianificare le ricorrenze. Possono essere impostati solo su attivi o inattivi.
* È possibile impostare più attivatori. Tuttavia, se viene attivato _un qualsiasi_ attivatore, le azioni della campagna verranno eseguite.

>[!TIP]
>
>Utilizzate il registro [delle](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person) attività per vedere cosa si è verificato passo dopo passo all&#39;interno delle campagne intelligenti. Potete trovare il registro attività nell&#39;ultima scheda della pagina dei dettagli di una persona.
