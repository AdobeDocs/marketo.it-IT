---
unique-page-id: 8159286
description: Filtri e attivatori per le opportunità - Documenti Marketo - Documentazione del prodotto
title: Filtri e attivatori per le opportunità
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Filtri e attivatori opportunità {#opportunity-filters-and-triggers}

I filtri e gli attivatori delle opportunità ti consentono di tenere traccia degli eventi delle opportunità da Salesforce. Sono un po&#39; diversi rispetto ad altri filtri e trigger.

## Filtri per le opportunità {#opportunity-filters}

I filtri delle opportunità ti consentono di analizzare in profondità i lead Salesforce che hanno opportunità. È possibile trovarli nella cartella Opportunità della palette quando si modifica un elenco avanzato. Vengono in qualche gusto.

* Numero di oggetti
* Importo totale dell&#39;opzione
* Ricavi previsti per l&#39;Opty totale
* Ha opportunità
* È stata aggiunta l’opportunità
* Opportunità rimossa
* Opportunità aggiornata

Se cerchi i campi Opportunità (personalizzati o standard), utilizza il filtro **Con opportunità** o **L&#39;opportunità era`[Added/Removed/Updated]`** filtri o trigger.

**Numero di opzioni, Importo totale dell&#39;opzione, Ricavi totali previsti dell&#39;opzione**

Con questi filtri, puoi trovare i lead in base al numero totale, alla quantità o ai ricavi previsti di tutte le loro opportunità.

![](assets/image2015-6-11-12-3a29-3a34.png)

**Ha un&#39;opportunità, è stata aggiunta all&#39;opportunità, è stata rimossa dall&#39;opportunità**

Se cerchi lead che hanno opportunità in base a una combinazione di criteri, utilizza il filtro **Con opportunità**, **È stato aggiunto a Opportunity** o **È stato rimosso da Opportunity** . Vi dicono:

* **Ha opportunità**: Se questo lead ha al momento qualche opportunità di corrispondenza
* **È stato aggiunto a Opportunità**: Se questo lead è stato aggiunto a un’opportunità corrispondente
* **È stato rimosso dall&#39;opportunità**: Se questo lead è stato rimosso da un’opportunità corrispondente

Aggiungi i criteri di ricerca come **Vincoli** sul filtro. I vincoli includono i campi di opportunità standard e personalizzati:

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Ad esempio, supponiamo di voler trovare i lead che hanno opportunità aperte di almeno 5.000 $. Trascina il filtro **Ha opportunità** e utilizza i vincoli **È chiuso** e **Importo**:

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>Quando utilizzi più filtri Opportunità, potresti ricevere risposte errate. Se hai creato l’esempio precedente con due filtri Opportunità, otterrai un elenco di lead che hanno un’opportunità di almeno 5.000 $ e qualsiasi opportunità che viene chiusa, anche se si tratta di opportunità separate.

**Opportunità aggiornata**

Il filtro **Opportunità è stata aggiornata** cerca qualsiasi opportunità quando un campo opportunità specifico è stato aggiornato. Scegli il campo da controllare con il menu a discesa Attributo trigger, quindi utilizza i vincoli per limitare il set di modifiche.

Ad esempio, questo filtro mostrerà a tutti i lead che hanno subito modifiche alla data di chiusura negli ultimi 30 giorni:

![](assets/image2015-6-11-12-3a33-3a7.png)

## Trigger opportunità {#opportunity-triggers}

Sono disponibili i seguenti trigger di opportunità. Funzionano come i filtri corrispondenti (descritti in precedenza), ma possono attivare le campagne subito quando si verifica l’evento:

* Opportunità aggiornata
* Aggiunto a Opportunità
* Rimosso dall&#39;opportunità

Ad esempio, puoi utilizzare questo Smart List per attivarsi quando viene aggiunto un lead a qualsiasi opportunità. Nel flusso, puoi aggiungerli all’elenco Marketing Suspended (Sospendi marketing) o inviare loro un’e-mail con targeting.

![](assets/image2015-6-11-12-3a33-3a48.png)

Per disattivare i campi personalizzati delle opportunità, utilizza l&#39;attivatore **Opportunity is Updated** (Opportunità aggiornata) e scegli il campo nel menu a discesa:

![](assets/image2015-6-11-12-3a33-3a34.png)
