---
unique-page-id: 9437991
description: Attivatori e filtri per campagne intelligenti mobile - Documentazione di Marketo - Documentazione del prodotto
title: Attivatori e filtri per campagne intelligenti mobile
exl-id: 76fc7a74-b27d-4898-a8ca-85c9c2828a28
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 0%

---

# Attivatori e filtri per campagne intelligenti mobile {#triggers-and-filters-for-mobile-smart-campaigns}

Puoi impostare trigger e filtri per una campagna intelligente per app mobili.

Per la maggior parte delle attività, esistono un trigger, un filtro e un filtro di inattività. Utilizzare i filtri di inattività per tenere traccia di un’azione, ad esempio toccare una notifica push, che *non ha* Accadrà.

* L&#39;App Mobile È/È Stata Installata
* L&#39;App Mobile È/È Stata Aperta
* Ha/Ha Avuto Attività Di App Mobile
* Ha/Ha Avuto Sessione App Mobile
* Notifica push mobile toccata/toccata

Esistono solo filtri per questa attività:

* Notifica push inviata: filtro e filtro di inattività

Cerca **app mobile** nel pannello a destra per elencare tutti i trigger e i filtri dell’app mobile.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-1.png)

## Vincoli {#constraints}

Utilizza i vincoli con trigger e filtri per ordinare ulteriormente i dati.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-2.png)

Tutti i trigger e i filtri, ad eccezione della notifica push inviata, contengono i due vincoli standard seguenti:

* Tipo di dispositivo - iPod, iPhone, iPhone 6 Plus, iPad mini, iPad, smartphone Android, tablet Android, Sconosciuto (elenco di predefiniti)

* Piattaforma - iPhone o Android

Alcuni trigger e filtri offrono vincoli aggiuntivi, ad esempio:

* Versione app: un modo per eseguire il targeting delle persone che non sono nella versione più recente. Ad esempio, se la versione più recente dell’app è 2.0, puoi utilizzarla per trovare persone che NON si trovano nella versione 2.0 dell’app

* Origine di installazione: al momento l’unica opzione è API

* Locale: l’impostazione sul dispositivo

* App mobile: nome dell’app specifica. Utile per specificare se si dispone di più di un

* Versione piattaforma: versione del sistema operativo

* Durata sessione (secondi) - Tempo della sessione quando l’app è in primo piano

* È abilitato per push - **Vero** significa che è possibile inviare notifiche push. **Falso** significa che non possono; ad esempio, la persona potrebbe aver rinunciato a ricevere notifiche push

## Trigger e filtri {#triggers-and-filters}

**Ha un’app mobile**

Usa questo filtro per scoprire tutte le persone che hanno mai avuto la tua app installata. Questa opzione è disponibile solo come filtro.

>[!NOTE]
>
>Il filtro individua sia le installazioni correnti che quelle precedenti, in quanto Marketo non tiene traccia delle disinstallazioni dell’app.

**Vincoli** - Tipo di dispositivo, Piattaforma, App mobile, Versione app mobile, Tipo di dispositivo, Origine di installazione, È abilitato per push e Impostazioni internazionali

![](assets/triggers-and-filters-for-mobile-smart-campaigns-3.png)

>[!TIP]
>
>È consigliabile specificare Has Mobile App = true and Is Push Enabled = true (Ha app mobile = true e Push abilitato = true), nonché il nome dell’app mobile, quando si definisce l’elenco avanzato di chi deve ricevere una notifica push.

L&#39;App Mobile È/È Stata Installata

* L’app mobile è installata - trigger

* App mobile installata - filtro

* Non è stata installata alcuna app mobile - filtro di inattività

**Vincoli** - Tipo di dispositivo, piattaforma, versione app, impostazioni internazionali e origine di installazione

![](assets/triggers-and-filters-for-mobile-smart-campaigns-4.png)

L&#39;App Mobile È/È Stata Aperta

* L’app mobile è aperta - trigger

* L&#39;app mobile è stata aperta - filtro

* NON è stata aperta alcuna app mobile - filtro di inattività

**Vincoli** - Tipo di dispositivo e piattaforma

![](assets/triggers-and-filters-for-mobile-smart-campaigns-5.png)

Ha/Ha Avuto Attività Di App Mobile

Questi forniscono un modo potente per tenere traccia delle attività mobili personalizzate. Devi collaborare con il tuo sviluppatore per configurare il tracciamento [per Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android) e [per iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios).

* Ha un&#39;attività in app mobile - trigger

* Aveva attività app mobile - filtro

* NON aveva attività app mobile - filtro di inattività

**Vincoli** - Tipo di dispositivo, piattaforma, versione app mobile, lingua, versione piattaforma, più cinque ulteriori:

* Azione: attività mobile personalizzata

* Tipo azione: (facoltativo) campo di testo utilizzato per categorizzare più azioni

* Dettagli azione: campo di testo (facoltativo) che fornisce informazioni aggiuntive su un’azione

* Metrica azione: (facoltativo) campo numerico che fornisce informazioni aggiuntive su un’azione (ad esempio, prezzo)

* Lunghezza azione (secondi): (facoltativo) campo numerico che può essere utilizzato per acquisire il tempo impiegato da un utente per completare un’azione

I vincoli di azione ti consentono di utilizzare il trigger e i filtri per monitorare molto da vicino le attività mobili.

>[!NOTE]
>
>**Esempio**
>
>Sotto il tipo di azione di *Acquisti*, ecco un’azione molto specifica, con gli altri vincoli che la definiscono:
>
>* Ha comprato una camicia
>   * Era rosso
>   * È costato 30 $
>   * Ci sono voluti 20 secondi per comprare

Ecco come si presenta il filtro in Marketo:

![](assets/triggers-and-filters-for-mobile-smart-campaigns-6.png)

>[!NOTE]
>
>**Esempio**
>
>Puoi avere più azioni sotto lo stesso tipo di azione. Infatti, la tua normale esperienza di acquisto può coinvolgere diverse colonne in Shopping! Che ne dite di un po&#39; di calze?
>
>| Tipo di azione | Acquisti | Acquisti |
>|---|---|---|
>| Azione | Camicia acquistata | Pantaloni acquistati |
>| Dettagli azione | Colore | Colore |
>| Metrica azione | Prezzo | Prezzo |

**Ha/Ha Avuto Sessione App Mobile**

* Ha una sessione per app mobile - trigger

* Sessione app mobile con filtro

* Sessione app mobile NON presente - filtro di inattività

**Vincoli** - Tipo di dispositivo, piattaforma e lunghezza della sessione (secondi)

![](assets/triggers-and-filters-for-mobile-smart-campaigns-7.png)

Notifica push toccata

* Notifica push toccate - trigger

* Notifica push toccata - filtro

* Notifica push NON toccata - filtro di inattività

**Vincoli** - Tipo di dispositivo, piattaforma, versione app mobile, notifica push e versione piattaforma

![](assets/triggers-and-filters-for-mobile-smart-campaigns-8.png)

>[!TIP]
>
>Utilizza il filtro di inattività Notifica push non toccata per trovare le persone che non hanno toccato una notifica push inviata di recente, in modo da poter seguire l’evento tramite e-mail.

**È Stata Inviata Una Notifica Push** Questa attività è disponibile solo come filtro.

* È stata inviata una notifica push - filtro

* Notifica push NOT - Filtro di inattività

**Vincoli** - Notifica push e app mobile

![](assets/triggers-and-filters-for-mobile-smart-campaigns-9.png)

>[!MORELIKETHIS]
>
>* [Aggiungere un vincolo a un filtro elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)
>* [Utilizzare i filtri di inattività in un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)
