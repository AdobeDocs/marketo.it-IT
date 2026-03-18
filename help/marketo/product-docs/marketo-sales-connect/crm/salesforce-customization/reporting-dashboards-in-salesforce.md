---
unique-page-id: 14352464
description: Scopri le dashboard di reporting in Salesforce che utilizzano i dati di Sales Connect. Visualizza le chiamate e le attività e-mail nei rapporti e nelle dashboard di Salesforce.
title: Dashboard di reporting in Salesforce
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
feature: Marketo Sales Connect
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 4%

---

# Dashboard di reporting in Salesforce {#reporting-dashboards-in-salesforce}

Scopri come impostare le dashboard di seguito.

## Apri e fai clic sul rapporto {#open-and-click-report}

1. Selezionare il tipo di record **[!UICONTROL Tasks and Events]**.
1. Definisci i parametri del rapporto in base all’intervallo di tempo desiderato e alla struttura gerarchica.
1. Aggiungere un filtro per rimuovere le e-mail interne registrate in [!DNL Salesforce] (ad esempio, Azienda/Account non uguale a Marketo).
1. Selezionare il formato del report **[!UICONTROL Summary]**.
1. Aggiungere al rapporto i campi Oggetto, Assegnato e Vendite Marketo selezionate/Vendite Marketo visualizzate.
1. Fare doppio clic su **[!UICONTROL Add Formula]** all&#39;interno del riquadro Campi.
1. Aggiungere un nome alla formula, selezionare **[!UICONTROL Percent]** nel formato e selezionare **[!UICONTROL Grouping 1]**.
1. Selezionare **[!UICONTROL Marketo Sales Clicked/Marketo Sales Viewed]**, quindi **[!UICONTROL Sum]** nei campi di riepilogo.
1. Aggiungere un segno di divisione alla formula, quindi selezionare **[!UICONTROL Record Count]** nei campi Riepilogo - _Salva con nome_.

## Report Prestazioni Modello {#template-performance-report}

1. Personalizzare il report Apri e fai clic per includere i campi seguenti: _Salva con nome_.

## Report volume modello {#template-volume-report}

1. Modificare il rapporto Prestazioni modello e includere il filtro &quot;Modello vendite Marketo non uguale a vuoto&quot;.
1. Rimuovi il campo Vendite Marketo selezionate - _Salva con nome_.

## Rapporto Conti di tendenza {#trending-accounts-report}

1. Selezionare Attività con tipo di record Conti.
1. Imposta i parametri e i campi del report come indicato di seguito - _Salva con nome_.
