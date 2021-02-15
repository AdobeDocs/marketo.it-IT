---
unique-page-id: 42762322
description: Scheda Configurazione analisi vendite Marketo in Salesforce - Documenti Marketo - Documentazione prodotto
title: Scheda Configurazione analisi vendite Marketo in Salesforce
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---


# Scheda Configurazione analisi vendite Marketo in Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Impostazioni operative {#operational-settings}

Per iniziare a utilizzare Sales Insight in SFDC, è necessario disporre di questa configurazione.

![](assets/one.png)

* MSI utilizza sia Soap che Rest API
* Nella pagina Sales Insight del tuo account Marketo saranno presenti due pannelli corrispondenti con le credenziali API Soap e Rest che puoi copiare e incollare qui
* Le API Soap e Rest dispongono di timeout separati che puoi impostare in base alle esigenze della tua organizzazione. Il tempo massimo consentito è di 120 secondi
* Disattivazione del dashboard di Insights: Potete rimuovere le credenziali Rest API e utilizzare solo Soap API. In questo modo la scheda Insights Dashboard verrà disattivata in tutti i pannelli della forza di visualizzazione MSI

## Configurazione MSI {#msi-configuration}

Le configurazioni sono applicabili a tutti gli utenti MSI e non sono specifiche per i profili.

**Impostazioni scheda Marketo**

* Modalità di debug delle migliori soluzioni
* Nascondi predefinito - L&#39;opzione scelta qui sarà il numero di giorni in cui una scommessa migliore sarà nascosta nella scheda Best Bets in Marketo quando si fa clic sull&#39;icona &quot;Nascondi&quot;
* Campo stato contatto - L&#39;opzione selezionata qui corrisponderà al valore inserito nella colonna Intestazione stato della scheda Best Bets in Marketo
* Impostazioni scheda - Per impostazione predefinita saranno disponibili tutte e 5 le schede. Potete scegliere l&#39;ordine delle schede nella pagina globale Marketo

**Impostazioni pagina Visualforce**

* Attiva azione, elenco a discesa:

   * Possibilità di nascondere l’e-mail Invia Marketo dall’elenco a discesa in Layout MSI lead e contatto
   * Possibilità di nascondere le opzioni Aggiungi a campagna marketing dall’elenco a discesa nel layout MSI Lead &amp; Contatta

* Prossimi eventi: Possibilità di mostrare gli eventi invitati, tutti gli eventi agli utenti o nascondere completamente questa scheda
* Prossime campagne: Possibilità di visualizzare tutte le campagne e-mail o nascondere completamente questa scheda
* Impostazioni scheda - Per impostazione predefinita saranno disponibili tutte e 5 le schede. Tutte le 5 schede saranno disponibili per impostazione predefinita. È possibile scegliere l&#39;ordine delle schede nel pannello Sales Insight. Lo stesso ordine sarà applicabile a tutto il layout (Lead, Contatto, Account, Opportunità)

![](assets/two.png)

**Limiti**

* L&#39;attività (Momento interessante, Attività Web, E-mail) è impostata su 1000 per impostazione predefinita. Per impostazione predefinita, le campagne e gli eventi e-mail sono impostati su 200
* Se noti problemi di timeout nell’organizzazione, puoi ridurre il limite

## Reimposta analisi vendite marketing {#reset-marketo-sales-insight}

La scelta di questa opzione comporterà l&#39;eliminazione di tutte le configurazioni della DSC e non sarà possibile ripristinarle. Dovrai riconfigurare tutto.

![](assets/three.png)
