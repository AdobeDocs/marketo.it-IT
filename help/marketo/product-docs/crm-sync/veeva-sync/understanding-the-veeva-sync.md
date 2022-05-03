---
description: Informazioni sulla sincronizzazione di Veeva - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulla sincronizzazione di Veeva
hide: true
hidefromtoc: true
source-git-commit: c36b9206494c14a52937fa787a37601eaf6f4bd4
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Informazioni sulla sincronizzazione di Veeva {#understanding-the-veeva-sync}

In pochi semplici passi, è facile eseguire una sincronizzazione tra Adobe Marketo Engage e Veeva CRM.

## Funzionamento della sincronizzazione {#how-the-sync-works}

Marketo Engage sincronizza con Veeva CRM tutto il giorno, ogni giorno. Ogni sincronizzazione richiede un po&#39; di tempo, si mette in pausa per 5 minuti, quindi si riavvia.

>[!NOTE]
>
>La prima sincronizzazione potrebbe richiedere ore o anche giorni perché il Marketo Engage sta copiando l&#39;intero database da Veeva. In seguito, ogni sincronizzazione richiede in genere minuti (a volte secondi) e sincronizza solo i dati che sono cambiati.

![](assets/understanding-the-veeva-sync-1.png)

La sincronizzazione tra Veeva e Marketo Engage è bidirezionale solo per i campi Contatto sull&#39;oggetto account Persona. In questi casi, ogni volta che apporti modifiche in Veeva o nel Marketo Engage, gli aggiornamenti verranno rispecchiati in entrambi i sistemi. Tutte le altre sincronizzazioni sono da Veeva al solo Marketo Engage. Fai clic sui link qui sotto per i dettagli su ciascuno.

## Sincronizzazione tra Marketo e Veeva {#what-is-synced-between-marketo-and-veeva}

Account personali Gli utenti chiamano e richiamano oggetti chiave Oggetti personalizzati

## Cose da sapere {#things-to-know}

* Le credenziali immesse nel Marketo Engage per Veeva vengono utilizzate per sincronizzare i dati. Verranno inclusi solo i dati a cui tali credenziali hanno accesso.

* Veeva CRM è basato su force.com e il Marketo Engage di esperienze avanzate con la piattaforma viene ereditato in questa sincronizzazione.

* Veeva CRM mostra: Lead, contatto, account (account aziendali, opportunità, campagna e attività). Tuttavia, non sono supportati nella sincronizzazione con il Marketo Engage.
