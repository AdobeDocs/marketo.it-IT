---
unique-page-id: 8159286
description: Filtri e attivatori per le opportunità - Marketo Docs - Documentazione prodotto
title: Filtri e attivatori opportunità
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Filtri e attivatori opportunità {#opportunity-filters-and-triggers}

I filtri e gli attivatori delle opportunità consentono di monitorare gli eventi delle opportunità da Salesforce. Sono un po&#39; diversi rispetto ad altri filtri e trigger.

## Filtri opportunità {#opportunity-filters}

I filtri Opportunità consentono di approfondire i lead Salesforce che dispongono di opportunità. È possibile trovarli nella cartella Opportunità della palette quando si modifica un elenco avanzato. Arrivano in qualche sapore.

* Numero di oggetti
* Importo totale delle opzioni
* Totale ricavi previsti dell&#39;opzione
* Con opportunità
* Opportunità aggiunta
* Opportunità rimossa
* Opportunità aggiornata

Se cercate i campi Opportunità (personalizzati o standard), utilizzate il filtro **Con opportunità** o **Opportunità era`[Added/Removed/Updated]`** filtri o attivatori.

**Numero di opzioni, importo totale dell&#39;opzione, ricavi previsti dell&#39;opzione totale**

Grazie a questi filtri è possibile individuare i lead in base al numero totale, all’importo o alle entrate previste per tutte le opportunità offerte.

![](assets/image2015-6-11-12-3a29-3a34.png)

**Ha un&#39;opportunità, è stata aggiunta all&#39;opportunità, è stata rimossa dall&#39;opportunità**

Se cercate lead con opportunità basate su una combinazione di criteri, utilizzate il filtro **Con opportunità**, **È stato aggiunto a opportunità** o **È stato rimosso dal filtro Opportunità**. Vi dicono:

* **Presenta opportunità**: Se questo lead dispone attualmente di un&#39;opportunità di corrispondenza
* **È stato aggiunto all&#39;opportunità**: Se questo lead è stato aggiunto a un&#39;opportunità di corrispondenza
* **È stato rimosso dall&#39;opportunità**: Se questo lead è stato rimosso da un&#39;opportunità di corrispondenza

Aggiungete i criteri di ricerca come **Vincoli** sul filtro. I vincoli includono i campi standard delle opportunità e personalizzati:

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Ad esempio, supponiamo di voler trovare lead con opportunità aperte di almeno $5.000. Trascinare nel filtro **Con opportunità** e utilizzare i vincoli **È chiusa** e **Importo**:

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>Quando utilizzate più filtri Opportunità, potreste ottenere risposte errate. Se l&#39;esempio precedente è stato creato con due filtri Opportunità, si ottiene un elenco di lead che hanno opportunità di almeno $5.000 e qualsiasi opportunità che viene chiusa, anche se si tratta di opportunità separate.

**Opportunità aggiornata**

Il filtro **Opportunità è stata aggiornata** cerca qualsiasi opportunità quando un campo opportunità specifico è stato aggiornato. Selezionare il campo da controllare con il pulldown Attributo attivatore, quindi utilizzare i vincoli per restringere il set di modifiche.

Ad esempio, questo filtro mostrerà tutti i lead che hanno subito una modifica della data di chiusura negli ultimi 30 giorni:

![](assets/image2015-6-11-12-3a33-3a7.png)

## Attivatori opportunità {#opportunity-triggers}

Sono disponibili i seguenti trigger di opportunità. Funzionano esattamente come i filtri corrispondenti (descritti in precedenza), con la differenza che possono attivare le campagne subito dopo l’evento:

* Opportunità aggiornata
* Aggiunta all&#39;opportunità
* Rimosso dall&#39;opportunità

Ad esempio, potete utilizzare questo Smart List per attivare eventuali lead aggiunti a qualsiasi opportunità. Nel flusso, potete aggiungerli all&#39;elenco Marketing Suspended (Sospensione marketing) o inviarli un&#39;e-mail di destinazione.

![](assets/image2015-6-11-12-3a33-3a48.png)

Per attivare i campi personalizzati delle opportunità, utilizzare l&#39;attivatore **Opportunità è stata aggiornata** e selezionare il campo nel pulldown:

![](assets/image2015-6-11-12-3a33-3a34.png)

