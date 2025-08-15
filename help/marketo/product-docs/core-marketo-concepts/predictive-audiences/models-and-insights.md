---
description: Modelli e informazioni - Documentazione di Marketo - Documentazione del prodotto
title: Modelli e informazioni
exl-id: 7a01d6f0-000a-4b9a-8abb-9e7f9c4b1679
feature: Predictive Audiences
source-git-commit: 8101d9c73571948847d00dfc21f21c39bcd1d975
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Modelli e informazioni {#models-and-insights}

Le prestazioni dei modelli dipendono dalla qualità e dalla completezza dei dati di input. Visualizza il fattore di influenza principale per ciascuno dei modelli di IA per la probabilità. Inoltre, scopri i principali fattori che determinano una registrazione più o meno elevata di un evento, la partecipazione a un evento o l’annullamento degli abbonamenti.

>[!NOTE]
>
>I comportamenti contrassegnati con (+) influenzano positivamente le previsioni (e viceversa).

Ecco come valutare lo stato del modello.

Passare alla sezione **[!UICONTROL Models and Data Health]** in **[!UICONTROL Predictive Audiences]** nell&#39;area **[!UICONTROL Admin]** di Marketo Engage. Qui vedrai tutti i tuoi modelli e i loro stati.

![Immagine Uno](assets/models-and-insights-1.png)

* **Stato apprendimento**: indica se il modello sta eseguendo un addestramento attivo (migliorando le previsioni). L’addestramento viene eseguito automaticamente ogni due settimane. Il completamento di qualsiasi modello _in elaborazione_ potrebbe richiedere fino a 24 ore. Per qualsiasi modello _Non riuscito_, contatta il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.
* **Stato punteggio**: indica se il modello sta calcolando attivamente le previsioni (percentuali di probabilità) per i membri del programma.
* **Prestazioni**: categorizzazione dell&#39;integrità del modello in base alla completezza dei dati e alla qualità dei dati (vedere di seguito).
* **Completezza dati**: percentuale di attributi di dati presenti/completi.
* **Qualità dei dati**: percentuale di attributi che contengono dati validi e utilizzabili.
* **Ultimo addestramento**: la data del modello che è il migliore tra la valutazione del modello corrente e quella del nuovo modello che viene addestrato ogni due settimane.
