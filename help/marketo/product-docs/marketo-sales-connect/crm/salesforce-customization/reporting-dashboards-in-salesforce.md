---
unique-page-id: 14352464
description: Dashboard di reporting in Salesforce - Documenti Marketo - Documentazione prodotto
title: Generazione di rapporti sui dashboard in Salesforce
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Generazione di rapporti sui dashboard in Salesforce {#reporting-dashboards-in-salesforce}

Scoprite come configurare le dashboard di seguito.

## Apri e fai clic su Rapporto {#open-and-click-report}

1. Selezionare il tipo di record **Attività ed eventi**.
1. Definite i parametri del rapporto in base all&#39;intervallo di tempo e alla struttura gerarchica desiderati.
1. Aggiungete un filtro per rimuovere le e-mail interne registrate in Salesforce (ad es. Azienda/Account non uguale a Marketo).
1. Selezionare il formato di report **Summary**.
1. Aggiungi al rapporto i campi Oggetto, Assegnato e Vendita marketing Clic/Vendite marketing.
1. Fare doppio clic su **Aggiungi formula** nel riquadro Campi.
1. Aggiungere un nome alla formula, selezionare **Percent** nel formato, quindi selezionare **Grouping 1**.
1. Selezionare **Vendite marketing Click/Marketing Vendite visualizzate,** quindi **Somma** nei campi Riepilogo.
1. Aggiungere un segno di divisione alla formula, quindi selezionare **Conteggio record** nei campi Riepilogo - _Salva con nome_.

## Report prestazioni modello {#template-performance-report}

1. Personalizzare il rapporto Apri e fai clic per includere i seguenti campi: _Salva con nome_.

## Report volume modello {#template-volume-report}

1. Modificate il Report prestazioni modello e includete il filtro &quot;Modello vendite marketing non uguale a vuoto&quot;.
1. Rimuovere il campo Vendite marketing Click - _Salva con nome_.

## Report dei conti di tendenza {#trending-accounts-report}

1. Selezionare Attività con tipo di record Account.
1. Impostate i parametri e i campi del rapporto come indicato di seguito - _Salva con nome_.
