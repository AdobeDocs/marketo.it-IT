---
unique-page-id: 1147091
description: Iscrizione al programma - Documentazione Marketo - Documentazione del prodotto
title: Informazioni sull’iscrizione al programma
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Informazioni sull’iscrizione al programma {#understanding-program-membership}

>[!NOTE]
>
>Marketo ora sta standardizzando il linguaggio in tutti gli abbonamenti, quindi potresti vedere lead/lead nel tuo abbonamento e persone/persone nei nostri documenti. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori informazioni](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md).

>[!NOTE]
>
>**Definizione:** Un membro è una persona con uno stato in un programma.

## Come le persone diventano membri di un programma {#how-people-become-members-of-a-program}

1. Una persona compila un [modulo in una pagina di destinazione](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) nel programma.

   1. La persona avrà automaticamente il primo stato nella progressione.

1. Tu [importa membri nel programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md) da un file CSV.

   1. La persona avrà automaticamente il primo stato nella progressione.

1. Utilizzi il [cambiare lo stato del programma](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md) passaggio di flusso.
1. Una persona si registra o partecipa a un [webinar sincronizzato con un programma di eventi](/help/marketo/product-docs/demand-generation/events/understanding-events/event-partners.md).
1. Una persona è [creato mediante l&#39;applicazione di archiviazione Marketo iPad](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md).
1. Una persona viene aggiunta a una campagna SFDC, che è [sincronizzato nel programma](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md).

>[!NOTE]
>
>Per un programma e-mail, una persona viene aggiunta all’iscrizione solo quando l’e-mail viene inviata.

## Stati dei programmi {#program-statuses}

Gli stati del programma sono i passaggi che le persone seguono in un programma (ad esempio Invitato, Confermato, Partecipato, No Show). Questi passaggi sono definiti da [channel](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>Una persona non può tornare indietro a uno stato di programma precedente. La progressione dello stato è unidirezionale.

## Stati di successo {#success-statuses}

Lo scopo di un programma è quello di creare un’interazione significativa con la persona o il potenziale cliente. Il successo è contrassegnato quando una persona raggiunge lo stato che raggiunge tale obiettivo.

>[!NOTE]
>
>Per un webinar, la registrazione non è un&#39;interazione significativa se non guardano effettivamente il webinar. In questo caso, partecipare è un successo.

## Programma di acquisizione  {#acquisition-program}

Quando un nuovo nome entra nel sistema come membro del programma, Marketo imposta automaticamente tale programma come &quot;acquisizione&quot;. Questo stabilisce il merito per [Attribuzione del primo contatto](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

>[!MORELIKETHIS]
>
>* [Utilizzare i tag in un programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags/use-tags-in-a-program.md)
>* [Creare un rapporto sulle prestazioni del programma](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md)
