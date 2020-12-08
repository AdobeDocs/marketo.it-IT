---
unique-page-id: 9437991
description: Attivatori e filtri per le campagne mobili intelligenti - Documenti Marketo - Documentazione prodotto
title: Attivatori e filtri per le campagne mobili intelligenti
translation-type: tm+mt
source-git-commit: 1c4c4c62215550a09125f76fb76017348aba2bdf
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---


# Attivatori e filtri per le campagne mobili intelligenti {#triggers-and-filters-for-mobile-smart-campaigns}

Puoi impostare attivatori e filtri per una campagna intelligente per app mobile.

Per la maggior parte delle attività sono presenti un trigger, un filtro e un filtro di inattività. Usate i filtri di inattività per tenere traccia di un’azione, ad esempio toccando una notifica push, che *non* è avvenuta.

* L&#39;App Mobile È/È Stata Installata
* App Mobile Aperta
* Con/Avevano Attività App Mobile
* Con/Avevano Sessione App Mobile
* Toccate/Toccate Notifica push mobile

Esistono solo filtri per questa attività:

* È stata inviata una notifica push - filtro e filtro di inattività

Cerca l’app **** mobile nel pannello a destra per elencare tutti gli attivatori e i filtri per l’app mobile.

![](assets/image2015-8-12-17-3a25-3a18.png)

## Vincoli {#constraints}

Usa i vincoli con attivatori e filtri per ordinare ulteriormente i dati.

![](assets/image2015-8-17-12-3a6-3a33.png)

Tutti gli attivatori e i filtri, ad eccezione di Invia notifica push, contengono i due vincoli standard seguenti:

* Tipo di dispositivo - iPod, iPhone, iPhone 6 Plus, iPad mini, iPad, smartphone Android, tablet Android, Sconosciuto (questo è un elenco di predefiniti)

* Piattaforma - iPhone o Android

Alcuni attivatori e filtri offrono vincoli aggiuntivi, ad esempio:

* Versione app - Un modo per eseguire il targeting delle persone che non sono sulla versione più recente. Ad esempio, se l&#39;ultima versione dell&#39;app è 2.0, potete usarla per trovare persone che NON sono sull&#39;app versione 2.0

* Installa origine - Attualmente, l&#39;unica opzione è API

* Impostazioni internazionali - L&#39;impostazione sul dispositivo

* App mobile: il nome di un&#39;app specifica. Utile per specificare se si dispone di più

* Versione piattaforma - Versione del sistema operativo

* Durata sessione (secondi) - Ora della sessione in cui l&#39;app è in primo piano

* È abilitato per push - **True** significa che è possibile inviare le notifiche push. **False** significa che non possono; ad esempio, la persona potrebbe aver rinunciato alla ricezione delle notifiche push

## Triggers e filtri {#triggers-and-filters}

**Con app mobile**

Utilizzate questo filtro per scoprire tutti gli utenti che hanno già installato la vostra app. Questo è disponibile solo come filtro.

>[!NOTE]
>
>Il filtro individuerà sia le installazioni correnti che quelle precedenti in quanto Marketo non tiene traccia dei disinstalli dell&#39;app.

**Vincoli**: Tipo di dispositivo, Piattaforma, App mobile, Versione app mobile, Tipo di dispositivo, Sorgente di installazione, È abilitato push e Impostazioni internazionali

![](assets/image2015-8-21-13-3a33-3a54.png)

>[!TIP]
>
>È buona norma specificare se l&#39;app con dispositivi mobili è impostata su True e se è abilitata la funzione Push = true, nonché il nome dell&#39;app mobile quando si definisce l&#39;elenco smart di chi deve ricevere una notifica push.

L&#39;App Mobile È/È Stata Installata

* App mobile installata - attiva

* App mobile installata - filtro

* NON è stata installata l&#39;app mobile - filtro di inattività

**Vincoli**: Tipo di dispositivo, piattaforma, versione app, lingua e origine di installazione

![](assets/image2015-8-17-13-3a11-3a3.png)

App Mobile Aperta

* L&#39;app mobile è aperta - attiva

* App mobile aperta - filtro

* L&#39;app NON mobile è stata aperta - filtro di inattività

**Vincoli**: Tipo di dispositivo e piattaforma

![](assets/image2015-8-17-13-3a13-3a55.png)

Con/Avevano Attività App Mobile

che forniscono un modo efficace per monitorare l&#39;attività mobile personalizzata. Dovrai collaborare con il tuo sviluppatore per configurare il tracciamento [per Android](http://developers.marketo.com/documentation/mobile/installation-instructions-on-android) e [per iOS](http://developers.marketo.com/documentation/mobile/installation-instructions-on-ios).

* Con attività app mobile - attivatore

* Avevano attività app mobile - filtro

* Attività app mobile NON presente - filtro di inattività

**Vincoli**: Tipo di dispositivo e piattaforma, più cinque ulteriori:

* Azione - Attività mobile personalizzata

* Tipo azione - (facoltativo) Campo di testo utilizzato per classificare più azioni

* Dettagli azione - (facoltativo) Campo di testo che fornisce informazioni aggiuntive su un&#39;azione

* Metrica azione - (facoltativo) Campo numerico che fornisce informazioni aggiuntive su un&#39;azione (ad esempio, prezzo)

* Lunghezza azione (secondi) - (facoltativo) Campo numerico che può essere utilizzato per acquisire il tempo necessario all’utente per completare un’azione

I vincoli Azione consentono di usare attivatore e filtri per tenere traccia dell’attività mobile molto da vicino.

>[!NOTE]
>
>**Esempio**
>
>Sotto il tipo di azione *Shopping*, ecco un&#39;azione molto specifica, con gli altri vincoli che la definiscono:
>
>* Ho comprato una camicia
>  * Era rosso
>  * È costato $ 30
>  * Ci sono voluti 20 secondi per comprare


Di seguito viene illustrato l’aspetto del filtro in Marketo:   ![](assets/image2015-8-17-13-3a16-3a12.png)

>[!NOTE]
>
>**Esempio**
>
>È possibile eseguire più azioni con lo stesso tipo di azione. In realtà, la vostra esperienza di acquisto normale può coinvolgere diverse colonne sotto Shopping! Che ne dite di un po&#39; di calze da accompagnare?
>
>| Tipo di azione | Shopping | Shopping |
>|---|---|---|
>| Azione | Camicia acquistata | Pantaloni acquistati |
>| Dettagli azione | Colore | Colore |
>| Metrica azione | Prezzo | Prezzo |


**Con/Avevano Sessione App Mobile**

* Con sessione app mobile - attivatore

* Sessione app mobile con filtro

* Sessione dell&#39;app mobile NON disponibile - filtro di inattività

**Vincoli**: Tipo di dispositivo, piattaforma e lunghezza della sessione (secondi)

![](assets/image2015-8-17-13-3a18-3a34.png)

Toccate/toccate la notifica push

* Tocca Notifica push - attivatore

* Notifica push con tocco - filtro

* NOTA push NON toccata - Filtro inattività

**Vincoli**: Tipo di dispositivo, piattaforma, versione dell&#39;app mobile, notifica push e versione della piattaforma

![](assets/image2015-8-21-14-3a2-3a24.png)

>[!TIP]
>
>Utilizzate il filtro di inattività delle notifiche push non toccate per individuare le persone che non hanno toccato una notifica push inviata di recente, in modo da poter essere seguite tramite e-mail.

**È stata inviata una notifica** push Questa attività è disponibile solo come filtro.

* È stata inviata una notifica push - filtro

* NON inviato la notifica push - filtro di inattività

**Vincoli**: Notifica push e app mobile

![](assets/image2015-8-21-14-3a3-3a50.png)

>[!NOTE]
>
>**Articoli correlati**
>
>* [Aggiunta di un vincolo a un filtro elenco avanzato](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)
>* [Utilizzo dei filtri per l&#39;inattività in un elenco avanzato](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

