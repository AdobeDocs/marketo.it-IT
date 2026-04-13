---
unique-page-id: 11386358
description: Scopri la sandbox Marketo Engage da testare prima della produzione. Utilizza un’istanza sandbox per eseguire il test senza influire sulla produzione.
title: Sandbox Marketo
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: 9d8baf635462f287a05955b8563bf7866049d94a
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 1%

---

# Sandbox Marketo {#marketo-sandbox}

Una sandbox di Marketo Engage è un’ulteriore istanza utilizzata a scopo di test prima dell’implementazione nell’ambiente di produzione.

>[!AVAILABILITY]
>
>Non tutti hanno acquistato questa funzione. Per ulteriori informazioni, contatta il team dell’account di Adobe (il tuo Account Manager).

Non è possibile sincronizzare una sandbox di Marketo con il CRM regolare se è già sincronizzata con l’istanza di produzione. Utilizza la sandbox del tuo CRM per la sincronizzazione e segui tutti gli stessi passaggi della sincronizzazione originale.

## Aspetti da considerare sulle sandbox {#things-to-know-about-sandboxes}

* Se si desidera aggiungere utenti, il processo è uguale a [aggiungere utenti in produzione](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md#add-a-user). Anche in questo caso, se dispongono già di un accesso a Marketo, devono utilizzare un indirizzo e-mail diverso.
* La sandbox di Marketo inizierà a essere vuota, ma dispone delle stesse funzioni dell’istanza di produzione.
* Se crei un programma nella sandbox e vuoi spostarlo in produzione, puoi eseguire un&#39;[importazione di programmi](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Le sandbox sono limitate in modo che le istanze di produzione non siano influenzate negativamente dagli ambienti di test. Puoi inviare fino a 20 e-mail per campagna.

>[!CAUTION]
>
>Al momento non è supportato l&#39;aggiornamento della sandbox per Marketo Dynamics _o_ Salesforce Sync. Se devi aggiornare la sandbox CRM, è necessaria una nuova sandbox Marketo. Per ulteriori informazioni, contatta il team dell’account di Adobe (il tuo Account Manager).

## Copia istanza {#instance-copy}

Puoi inviare un caso di supporto richiedendo una copia dell’istanza una tantum per riempire la sandbox. La copia dell&#39;istanza non riporterà _tutto_. Per ulteriori informazioni, consultare [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support).

>[!NOTE]
>
>Se stai modificando il CRM nativo, sarebbe necessaria una nuova istanza di Marketo e non sarebbe possibile effettuare una copia dell’istanza nella nuova istanza di Marketo. In alternativa, è possibile consultare il Supporto tecnico Marketo per esplorare le funzionalità di importazione del programma.
