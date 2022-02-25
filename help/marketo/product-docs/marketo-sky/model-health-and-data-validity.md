---
description: Stato del modello e validità dei dati - Documenti Marketo - Documentazione del prodotto
title: Salute del modello e validità dei dati
hide: true
hidefromtoc: true
source-git-commit: ab20d9683aa5987778970fd32793dc0f3056c84b
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# Salute del modello e validità dei dati {#model-health-and-data-validity}

Le prestazioni dei modelli dipendono dalla qualità e dalla completezza dei dati di input. Vedi il fattore di influenza principale per ciascuno dei tuoi modelli di probabilità AI. Puoi vedere anche i fattori principali che determinano una registrazione degli eventi più elevata/minore, la partecipazione agli eventi o l’annullamento dell’abbonamento.

>[!NOTE]
>
>I comportamenti contrassegnati con (+) influenzano positivamente le previsioni (e viceversa).

Ecco come valutare lo stato di salute del modello.

Passa a **[!UICONTROL Modelli e integrità dei dati]** sezione **[!UICONTROL Predictive Audiences]** in **[!UICONTROL Amministratore]** area di Marketo Classic. Qui potrai vedere tutti i tuoi modelli e i loro stati.

![Immagine uno](assets/model-health-and-data-validity-1.png)

* **Stato formazione**: Indica se il modello è in corso di formazione attiva (miglioramento delle previsioni). L&#39;allenamento avviene automaticamente ogni 2 settimane. Qualsiasi modello _Elaborazione_ potrebbero richiedere fino a 24 ore per finire. Per qualsiasi _Non riuscito_ modelli, contattare [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).
* **Stato punteggio**: Indica se il modello sta calcolando attivamente le previsioni (percentuali di probabilità) per i membri del programma.
* **Prestazioni**: categorizzazione dello stato di salute del modello in base al completamento dei dati e alla qualità dei dati (vedi di seguito).
* **Completezza dei dati**: Percentuale di attributi di dati presenti/completi.
* **Qualità dei dati**: Percentuale di attributi che contengono dati validi e utilizzabili.