---
unique-page-id: 1147027
description: Sincr. la persona in SFDC - Marketo Docs - Documentazione del prodotto
title: Sincronizza persona con SFDC
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# Sincronizza persona con SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

>[!NOTE]
>
>Disponibile solo se integrato con Salesforce.

## Panoramica {#overview}

Questo passaggio di flusso inserirà le persone create da Marketo come lead in Salesforce CRM.

![](assets/sync-person-to-sfdc.png)

## Utilizzo {#usage}

1. Per impostazione predefinita, questo passaggio di flusso verrà assegnato ai proprietari principali in base alle regole di assegnazione automatica di Salesforce.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce richiede che siano compilati i campi Società e Cognome della persona. In caso contrario, rifiuterà il record lead.

1. Puoi impostare un utente Salesforce specifico o una coda lead come proprietario principale.

   ![](assets/sync-person-to-sfdc-2.png)

   Quando si utilizza questo passaggio di flusso, la persona viene sincronizzata immediatamente come lead Salesforce e non deve attendere la sincronizzazione regolare.

   >[!CAUTION]
   >
   >Salesforce non consente di assegnare &quot;Contatti&quot; alle code principali. In questo caso, Marketo creerà un &quot;Lead&quot; duplicato in Salesforce.

