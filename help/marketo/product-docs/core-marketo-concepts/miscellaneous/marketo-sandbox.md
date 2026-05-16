---
unique-page-id: 11386358
description: Scopri la sandbox Marketo Engage da testare prima della produzione. Utilizza un’istanza sandbox per eseguire il test senza influire sulla produzione.
title: Sandbox Marketo
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
TQID: https://experienceleague.adobe.com/Cb1H0PKG-G0c4FkIcjI-erNzR0dwRtj7TwfqtwhFFMI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 306
ht-degree: 3%

---

# Sandbox Marketo {#marketo-sandbox}

Una sandbox di Marketo Engage è un’ulteriore istanza utilizzata a scopo di test prima dell’implementazione nell’ambiente di produzione.

>[!AVAILABILITY]
>
>Non tutti hanno acquistato questa funzione. Per informazioni, contatta il team dell’account di Adobe (il tuo Account Manager).

Non è possibile sincronizzare una sandbox di Marketo con il CRM regolare se è già sincronizzata con l’istanza di produzione. Utilizza la sandbox del tuo CRM per la sincronizzazione e segui tutti gli stessi passaggi della sincronizzazione originale.

## Aspetti da considerare sulle sandbox {#things-to-know-about-sandboxes}

* Se si desidera aggiungere utenti, il processo è uguale a [aggiungere utenti in produzione](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md#add-a-user). Anche in questo caso, se dispongono già di un accesso a Marketo, devono utilizzare un indirizzo e-mail diverso.
* La sandbox di Marketo inizierà a essere vuota, ma dispone delle stesse funzioni dell’istanza di produzione.
* Se crei un programma nella sandbox e vuoi spostarlo in produzione, puoi eseguire un&#39;[importazione di programmi](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* Le sandbox sono limitate, pertanto gli ambienti di test non influiscono negativamente sulle istanze di produzione. Puoi inviare fino a 20 e-mail per campagna.

>[!CAUTION]
>
>L&#39;aggiornamento della sandbox per Marketo Dynamics _o_ Salesforce Sync non è al momento supportato. Se devi aggiornare la sandbox CRM, è necessaria una nuova sandbox Marketo. Per informazioni, contatta il team dell’account di Adobe (il tuo Account Manager).

## Copia istanza {#instance-copy}

Puoi inviare un caso di supporto richiedendo una copia dell’istanza una tantum per riempire la sandbox. La copia dell&#39;istanza non riporterà _tutto_. Contattare il [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support) per ulteriori dettagli.

>[!NOTE]
>
>Se stai modificando il CRM nativo, sarebbe necessaria una nuova istanza di Marketo e non sarebbe possibile effettuare una copia dell’istanza nella nuova istanza di Marketo. In alternativa, è possibile utilizzare il supporto tecnico di Marketo per esplorare le funzionalità di importazione del programma.
