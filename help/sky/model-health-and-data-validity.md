---
title: model-health-and-data-valid
description: Salute del modello e validità dei dati
exl-id: b14ec648-be1c-467b-b41d-2c53d74e25ea
source-git-commit: 41a51afde7942d6973a01636810bc5862d023e99
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Salute del modello e validità dei dati

Le prestazioni dei modelli dipendono dalla qualità e dalla completezza dei dati di input. Vedi il fattore di influenza principale per ciascuno dei tuoi modelli di probabilità AI. Puoi vedere anche i fattori principali che determinano una registrazione degli eventi più elevata/minore, la partecipazione agli eventi o l’annullamento dell’abbonamento.

>[!NOTE]
>
>I comportamenti contrassegnati con (+) influenzano positivamente le previsioni (e viceversa).

Ecco come valutare lo stato di salute del modello.

Passa a **[!UICONTROL Models and Data Health]** sezione **[!UICONTROL Predictive Audiences]** in **[!UICONTROL Admin]** area di Marketo Classic. Qui potrai vedere tutti i tuoi modelli e i loro stati.

![Immagine uno](/help/sky/assets/predictive-audiences/model-health-and-data-validity/model-health-and-data-validity-1.png)

* **Stato formazione**: Indica se il modello è in corso di formazione attiva (miglioramento delle previsioni). L&#39;allenamento avviene automaticamente ogni 2 settimane. Qualsiasi modello _Elaborazione_ potrebbero richiedere fino a 24 ore per finire. Per qualsiasi _Non riuscito_ modelli, contattare [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).
* **Stato punteggio**: Indica se il modello sta calcolando attivamente le previsioni (percentuali di probabilità) per i membri del programma.
* **Prestazioni**: categorizzazione dello stato di salute del modello in base al completamento dei dati e alla qualità dei dati (vedi di seguito).
* **Completezza dei dati**: Percentuale di attributi di dati presenti/completi.
* **Qualità dei dati**: Percentuale di attributi che contengono dati validi e utilizzabili.
