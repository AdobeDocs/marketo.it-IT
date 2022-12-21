---
unique-page-id: 1146950
description: Wait - Marketo Docs - Documentazione del prodotto
title: Wait
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 1%

---

# Wait {#wait}

## Panoramica {#overview}

Mettere in pausa una persona in un flusso di campagna intelligente con la facilità **passaggio di attesa**.

![](assets/wait-overview.png)

Notate come si può digitare in linguaggio naturale come &quot;4 ore&quot;. Do **not**, tuttavia, abbrevia le parole (cioè 4 ore). La campagna intelligente verrebbe comunque eseguita, ma il passaggio di attesa verrebbe ignorato.

>[!CAUTION]
>
>La modifica della durata di un passaggio di attesa non avrà effetto sulle persone che lo hanno già inserito. Ad esempio: si ha un passo di attesa per 5 giorni, una persona vi entra, poi si cambia il passo di attesa a 7 giorni - quella persona aspetterà ancora solo i 5 giorni originali prima di avanzare al passaggio successivo di flusso.

>[!TIP]
>
>Se si dispone di un utente già in un passaggio di attesa e non si desidera che avanzi al termine del periodo di attesa, inserire [rimuovi dal flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) subito dopo il passaggio di attesa. Specificare gli utenti che si desidera rimuovere utilizzando [aggiungi scelta](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) opzione .

## Utilizzo {#usage}

Sono disponibili tre modi principali per utilizzare un passaggio di flusso di attesa:

1. [Utilizzare una durata in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [Utilizzare una data specifica in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [Utilizzare un token di data in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
