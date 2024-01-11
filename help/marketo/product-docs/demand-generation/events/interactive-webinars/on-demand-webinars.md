---
description: Webinar on-demand - Documentazione di Marketo - Documentazione del prodotto
title: Webinar on demand
hide: true
hidefromtoc: true
feature: Interactive Webinars
source-git-commit: 4dccf70f42153045f630bf646a6a193e27dbf637
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Webinar on demand {#on-demand-webinars}

I webinar on-demand acquisiscono e perfezionano i lead che si sono registrati per l’evento e che non hanno partecipato, ma desiderano ottenere informazioni relative all’evento guardando la registrazione. Informazioni quali Nome, ID e-mail e Data/durata di controllo possono essere acquisite nel Marketo Engage e utilizzate per individuare questi lead non visibili.

L’URL di unione del webinar condiviso con gli utenti registrati prima dell’evento può essere utilizzato per guardare la registrazione on-demand. Quando un utente registrato che non ha partecipato all’evento live (ad esempio, un lead con lo stato di programma &quot;No-Show&quot;) fa clic sull’URL di iscrizione al webinar, lo stato di tale lead cambia da &quot;No-Show&quot; a &quot;Partecipated On-Demand&quot;. Lo stato del programma dei lead che hanno guardato l’evento in diretta e che hanno lo stato &quot;Partecipato&quot; non subisce modifiche se decidono di visitare l’URL di unione e guardare la registrazione on-demand.

Adobe Connect, la tecnologia che alimenta i webinar interattivi, tiene traccia della visita e della durata dell’orologio relativi ai lead che guardano la registrazione e segnala le informazioni a Marketo su base giornaliera. La registrazione è disponibile nell’URL di join per 30 giorni dopo l’evento. Impossibile modificare la durata.

Marketo fornisce le statistiche di controllo per i webinar on-demand sulla scheda Dashboard con l’aiuto dei seguenti widget:

* Riepilogo on-demand: fornisce un riepilogo del numero di visitatori (no-show) che guardano la registrazione dopo l’evento in un dato giorno/i

* Statistiche on-demand: questo widget fornisce informazioni su:
   * Giorni in cui è disponibile per la visualizzazione la registrazione su richiesta: consente agli addetti al marketing di eseguire azioni, ad esempio eseguire campagne e-mail prossime alla fine della durata di disponibilità della registrazione di 30 giorni.
   * Conteggio complessivo dei visitatori per i webinar on-demand fino ad oggi: il conteggio di tutti i partecipanti che hanno guardato la registrazione on-demand fino ad oggi.
   * Durata media dell’orologio in minuti per tutti i visitatori: fornisce agli addetti al marketing un’idea di quanta registrazione viene visualizzata e di quali campagne intelligenti possono essere utilizzate per indirizzare i lead oltre una determinata durata dell’orologio.

![](assets/on-demand-webinars-1.png)

I filtri e i trigger per i webinar interattivi sono stati modificati per soddisfare i webinar on-demand. Il trigger &quot;Partecipa all’evento&quot; e il filtro &quot;Ha partecipato all’evento&quot; vengono aggiunti con un vincolo aggiuntivo (&quot;Modalità evento&quot;), in cui un addetto marketing può scegliere se il target è Pubblico live o Pubblico on demand. Se il vincolo &quot;Modalità evento&quot; non è selezionato, verrà eseguito il targeting sia del pubblico Live che di quello On-Demand. Con la modalità evento &quot;On-Demand&quot; è possibile utilizzare altri vincoli, ad esempio &quot;Watch Date&quot; (Data di osservazione) e &quot;Watch Duration&quot; (Durata osservazione). Il filtro di inattività &quot;Non ha partecipato a un evento&quot; può essere utilizzato anche per i webinar on-demand con modalità evento &quot;on-demand&quot;.
