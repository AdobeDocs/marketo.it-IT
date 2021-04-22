---
unique-page-id: 1147091
description: Informazioni sull’appartenenza al programma - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sull’appartenenza al programma
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Informazioni sull&#39;appartenenza al programma {#understanding-program-membership}

>[!NOTE]
>
>Marketo sta standardizzando la lingua per tutte le sottoscrizioni, pertanto potresti visualizzare lead/lead nell’abbonamento e persona/persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori informazioni](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md).

>[!NOTE]
>
>**Definizione:** un membro è una persona che ha uno stato in un programma.

## Come le persone diventano membri di un programma {#how-people-become-members-of-a-program}

1. Una persona compila un modulo [su una pagina di destinazione](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) nel programma.

   1. La persona avrà automaticamente il primo stato nella progressione.

1. Importare i membri [nel programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md) da un file CSV.

   1. La persona avrà automaticamente il primo stato nella progressione.

1. Utilizza il passaggio di flusso [cambia lo stato del programma](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md) .
1. Una persona registra o partecipa a un webinar [sincronizzato con un programma di eventi](/help/marketo/product-docs/demand-generation/events/understanding-events/launchpoint-event-partners.md).
1. Una persona viene [creata utilizzando l&#39;applicazione di check-in Marketo iPad](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md).
1. Una persona viene aggiunta a una campagna SFDC, che è [sincronizzata con il programma](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md).

>[!NOTE]
>
>Per un programma e-mail, una persona viene aggiunta all’iscrizione solo quando l’e-mail viene inviata.

## Stati del programma {#program-statuses}

Gli stati del programma sono i passaggi che le persone attraversano in un programma (ad esempio, Invitato, RSVP-d, Partecipato, No Show). Questi passaggi sono definiti dal [canale](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>Una persona non può tornare a uno stato precedente del programma. La progressione dello stato è solo unidirezionale.

## Stati di successo {#success-statuses}

Lo scopo di un programma è quello di creare un&#39;interazione significativa con la persona o il potenziale cliente. Il successo viene contrassegnato quando una persona raggiunge lo stato che raggiunge tale obiettivo.

>[!NOTE]
>
>Per un webinar, la registrazione non è un&#39;interazione significativa se non guarda il webinar. Partecipare è un successo in questo caso.

## Programma di acquisizione {#acquisition-program}

Quando un nuovo nome entra nel sistema come membro del programma, Marketo lo imposta automaticamente come &quot;acquisizione&quot;. Questo stabilisce il merito per l’attribuzione [Primo contatto](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

>[!MORELIKETHIS]
>
>* [Utilizzare i tag in un programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags/use-tags-in-a-program.md)
>* [Creare un rapporto sulle prestazioni del programma](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md)

