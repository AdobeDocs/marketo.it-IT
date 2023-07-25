---
unique-page-id: 8159286
description: Filtri e attivatori dell’opportunità - Documentazione di Marketo - Documentazione del prodotto
title: Filtri e attivatori dell’opportunità
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Filtri e attivatori dell’opportunità {#opportunity-filters-and-triggers}

I filtri e i trigger di opportunità ti consentono di monitorare gli eventi di opportunità da Salesforce. Sono leggermente diversi rispetto ad altri filtri e attivatori.

## Filtri opportunità {#opportunity-filters}

I filtri opportunità ti consentono di analizzare in dettaglio i lead di Salesforce che hanno opportunità. È possibile trovarli nella cartella Opportunità della tavolozza quando si modifica un elenco avanzato. Sono disponibili in alcuni gusti.

* Numero di opzioni
* Importo opzione totale
* Ricavi previsti opzione totale
* Ha un’opportunità
* Opportunità aggiunta
* Opportunità rimossa
* L’opportunità è stata aggiornata

Se cerchi i campi Opportunità (personalizzati o standard), utilizza **Ha un’opportunità** filtro o **L&#39;opportunità è stata`[Added/Removed/Updated]`** filtri o trigger.

**Numero di opzioni, Importo opzione totale, Ricavi previsti opzione totale**

Con questi filtri, puoi trovare i lead in base al numero totale, all’importo o ai ricavi previsti di tutte le loro opportunità.

![](assets/image2015-6-11-12-3a29-3a34.png)

**L’Opportunità Possesso È Stata Aggiunta All’Opportunità Ed È Stata Rimossa Dall’Opportunità**

Se cerchi lead con opportunità basate su una combinazione di criteri, utilizza **Ha un’opportunità**, **È stato aggiunto all’opportunità**, o **È stato rimosso dall’opportunità** filtro. Ti dicono:

* **Ha un’opportunità**: se al momento il lead ha un’opportunità corrispondente
* **È stato aggiunto all’opportunità**: se questo lead è mai stato aggiunto a un’opportunità corrispondente
* **È stato rimosso dall’opportunità**: se questo lead è stato rimosso da un’opportunità corrispondente

Aggiungi i criteri di ricerca come **Vincoli** sul filtro. I vincoli includono lo standard dell’opportunità e i campi personalizzati:

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Ad esempio, supponiamo che tu voglia trovare lead con opportunità aperte di almeno 5.000 dollari. Trascina nella **Ha un’opportunità** filtrare e utilizzare **È chiuso** e **Quantità** vincoli:

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>Quando si utilizzano più filtri opportunità, è possibile che vengano visualizzate risposte non corrette. Se hai creato l’esempio precedente con due filtri di opportunità, otterrai un elenco di lead con opportunità che sono pari ad almeno 5.000 dollari e con qualsiasi opportunità chiusa, anche se si tratta di opportunità separate.

**L’opportunità è stata aggiornata**

Il **L’opportunità è stata aggiornata** Il filtro cerca qualsiasi opportunità quando un campo opportunità specifico è stato aggiornato. Seleziona il campo da controllare con il menu a discesa Attributo trigger, quindi utilizza i vincoli per restringere l’insieme delle modifiche.

Ad esempio, questo filtro mostrerà tutti i lead per i quali è stata modificata la data di chiusura negli ultimi 30 giorni:

![](assets/image2015-6-11-12-3a33-3a7.png)

## Trigger opportunità {#opportunity-triggers}

Sono disponibili i seguenti trigger di opportunità. Funzionano esattamente come i filtri corrispondenti (descritti in precedenza), tranne per il fatto che possono attivare le campagne proprio quando si verifica l’evento:

* L’opportunità è aggiornata
* Aggiunto all’opportunità
* Rimosso dall’opportunità

Ad esempio, puoi utilizzare questo elenco avanzato per attivare quando un lead viene aggiunto a qualsiasi opportunità. Nel flusso, puoi aggiungerli all’elenco Marketing Sospeso o inviare loro un’e-mail mirata.

![](assets/image2015-6-11-12-3a33-3a48.png)

Per attivare i campi personalizzati dell’opportunità, utilizza **L’opportunità è aggiornata** attiva e seleziona il campo nel pulldown:

![](assets/image2015-6-11-12-3a33-3a34.png)
