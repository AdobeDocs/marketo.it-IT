---
unique-page-id: 10912085
description: Indirizzi IP condivisi e dedicati - Documentazione di Marketo - Documentazione del prodotto
title: Indirizzi IP condivisi e dedicati
exl-id: 3d7a78f4-531a-4ad7-a20b-1385bd62d1d9
feature: Deliverability
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Indirizzi IP condivisi e dedicati {#shared-and-dedicated-ip-addresses}

## Che cos’è un indirizzo IP? {#what-is-an-ip-address}

Etichetta numerica che indica l&#39;indirizzo di un computer connesso a Internet.

## Cosa sono gli indirizzi IP condivisi? {#what-are-shared-ip-addresses}

Si riferisce a quando più mittenti utilizzano gli stessi indirizzi IP per avviare campagne e-mail. Condividono tutti gli stessi IP di invio.

## Che cos’è un indirizzo IP dedicato? {#what-is-a-dedicated-ip-address}

Un indirizzo IP specifico per l’utente inviato da un solo mittente.

## Qual è il migliore: condiviso o dedicato? {#which-is-better-shared-or-dedicated}

Come al solito, ci sono pro e contro per entrambe le opzioni.

**Pro e contro di un IP dedicato**

_Pro_

**Reputazione** - Sei completamente proprietario della tua reputazione e del tuo recapito messaggi.
**Monitoraggio** - Il monitoraggio del reporting sul recapito messaggi consente di rispondere rapidamente alle modifiche nelle metriche di consegna.
**Risoluzione dei problemi** - È più facile ricercare, comprendere e risolvere i problemi di consegna.

_Contro_

**Modifiche al volume** - I picchi nel volume possono influire negativamente sulla reputazione e devono essere gestiti.
**Processo di riscaldamento IP** - La reputazione è stata creata nel tempo. Alcuni provider di servizi Internet (ISP) limitano gli indirizzi IP senza cronologia dei volumi, pertanto dovrai creare una reputazione nelle prime settimane (Marketo può aiutarti).
**Costo** - In genere è previsto un costo aggiuntivo per l&#39;invio da un IP dedicato con qualsiasi provider.

**Pro e contro di un IP condiviso**

_Pro_

**Buoni coinquilini** - Se gli utenti che stai condividendo il tuo IP seguono le best practice di invio, ne trarrai vantaggio.
**Frequenza di invio** - Non è necessaria alcuna frequenza di invio minima per qualificarsi per un IP condiviso, a differenza di quanto avviene con gli IP dedicati.
**Costo** - Non esiste mai un costo aggiuntivo da inviare da un IP condiviso.

_Contro_

**Compagni di stanza non validi** - Se gli utenti che condividi il tuo IP sono coinvolti in pratiche di invio scadenti, le tue campagne e-mail potrebbero essere influenzate negativamente.
**Controllo** - Hai un controllo molto minore sulla reputazione del mittente.
**Risoluzione del problema** - Spesso può essere più difficile risolvere un problema durante l&#39;invio da IP condivisi.

>[!NOTE]
>
>Quando prendi una decisione, prendi in considerazione anche un altro fattore importante: il volume di invio. Se prevedi di inviare meno di 100.000 e-mail al mese, o meno di due e-mail in un mese, probabilmente non trarrai vantaggio da un IP dedicato. Inviare numeri come questo sono considerati bassi, e sarebbe difficile mantenere il tuo IP dedicato &quot;caldo&quot; abbastanza per essere considerato sicuro dai principali ISP. Fondamentalmente, se non invii abbastanza spesso, gli ISP vedranno un messaggio come un improvviso &quot;aumento&quot; di attività e potrebbero finire per bloccarlo come spam sospetto.

Per maggiori informazioni o se sei interessato alla configurazione di un IP dedicato, contatta il tuo rappresentante commerciale Marketo.
