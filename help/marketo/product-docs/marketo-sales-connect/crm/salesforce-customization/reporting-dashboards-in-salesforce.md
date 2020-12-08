---
unique-page-id: 14352464
description: Dashboard di reporting in Salesforce - Documenti Marketo - Documentazione prodotto
title: Generazione di rapporti sui dashboard in Salesforce
translation-type: tm+mt
source-git-commit: 07ae1b3f3ee3e9d7f35373eea039d336bd786f97
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Generazione di rapporti sui dashboard in Salesforce {#reporting-dashboards-in-salesforce}

Scoprite come configurare le dashboard di seguito.

## Apri e fai clic su Rapporto {#open-and-click-report}

1. Selezionare il tipo di record **Attività ed Eventi** .
1. Definite i parametri del rapporto in base all&#39;intervallo di tempo e alla struttura gerarchica desiderati.
1. Aggiungete un filtro per rimuovere le e-mail interne registrate in Salesforce (ad es. Azienda/Account non uguale a Marketo).
1. Selezionare il formato del rapporto **Riepilogo** .
1. Aggiungi al rapporto i campi Oggetto, Assegnato e Vendita marketing Clic/Vendite marketing.
1. Fare doppio clic su **Aggiungi formula** nel riquadro Campi.
1. Aggiungete un nome alla formula, selezionate **Percent **nel formato, quindi selezionate** Grouping 1 *.***
1. Selezionare Vendite **marketing cliccate/Vendite marketing visualizzate,** quindi **Somma** nei campi Riepilogo.
1. Aggiungere un segno di divisione alla formula, quindi selezionare **Record Count** (Conteggio record) nei campi Summary (Riepilogo) - *Save As (Salva con nome*).

## Report prestazioni modello {#template-performance-report}

1. Personalizzate il rapporto Apri e fai clic per includere i seguenti campi: *Salva con nome.*

## Report volume modello {#template-volume-report}

1. Modificate il Report prestazioni modello e includete il filtro &quot;Modello vendite marketing non uguale a vuoto&quot;.
1. Rimuovi il campo Vendite marketing Click - *Salva con nome*.

## Report dei conti di tendenza {#trending-accounts-report}

1. Selezionare Attività con tipo di record Account.
1. Impostare i parametri e i campi del rapporto come indicato di seguito - *Salva con nome.

