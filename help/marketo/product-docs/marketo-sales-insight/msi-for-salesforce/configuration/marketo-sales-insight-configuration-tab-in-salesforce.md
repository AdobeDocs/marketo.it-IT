---
unique-page-id: 42762322
description: Scheda Configurazione Approfondimenti vendite Marketo in Salesforce - Documenti Marketo - Documentazione del prodotto
title: Scheda Configurazione Approfondimenti vendite Marketo in Salesforce
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# Scheda Configurazione Approfondimenti vendite Marketo in Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Impostazioni operative {#operational-settings}

Sarà necessario impostare questa impostazione per iniziare a utilizzare Sales Insight in SFDC.

![](assets/one.png)

* MSI utilizza sia l’API Soap che Rest
* Nella pagina Approfondimenti vendite del tuo account Marketo saranno presenti due pannelli corrispondenti con le credenziali API Soap e Rest che puoi copiare e incollare qui
* Le API Soap e Rest dispongono di timeout separati che puoi impostare in base alle esigenze della tua organizzazione. Il tempo massimo consentito è di 120 secondi
* Disabilitazione del dashboard di Insights: Puoi rimuovere le credenziali API per il resto e utilizzare solo l’API Soap. In questo modo si disabilita la scheda Dashboard approfondimenti in tutti i pannelli della forza visivo MSI

## Configurazione MSI {#msi-configuration}

Le configurazioni sono applicabili a tutti gli utenti MSI e non sono specifiche per i profili.

**Impostazioni della scheda Marketo**

* Modalità di debug delle migliori operazioni
* Nascondi predefinito - L&#39;opzione che scegli qui sarà il numero di giorni in cui una scommessa migliore sarà nascosta nella scheda Best Bets in Marketo quando fai clic sull&#39;icona &quot;Nascondi&quot;
* Campo stato contatto : l’opzione selezionata sarà il valore compilato nella colonna Intestazione stato della scheda Best Bets in Marketo
* Impostazioni scheda : per impostazione predefinita saranno disponibili tutte e 5 le schede. Puoi scegliere l’ordine delle schede nella pagina globale Marketo .

**Impostazioni pagina della visualizzazione**

* Menu a discesa Abilita azione :

   * Possibilità di nascondere l’e-mail Send Marketo dall’elenco a discesa in Layout lead &amp; Contact MSI
   * Possibilità di nascondere le opzioni Aggiungi a Marketo Campaign dal menu a discesa in Layout lead e contatta MSI

* Prossimi eventi: Possibilità di mostrare gli eventi invitati, tutti gli eventi agli utenti o nascondere completamente questa scheda
* Prossime campagne: Possibilità di mostrare tutte le campagne e-mail o nascondere completamente questa scheda
* Carica campagne ed eventi in arrivo: Possibilità di ridurre il numero di chiamate API rimanenti effettuate dagli utenti inserendo gli eventi e la scheda delle campagne dietro un pulsante &quot;Carica gli elementi in arrivo&quot; on-demand
* Impostazioni scheda : per impostazione predefinita saranno disponibili tutte e 5 le schede. Per impostazione predefinita saranno disponibili tutte e 5 le schede. È possibile scegliere l&#39;ordine delle schede nel pannello Approfondimenti vendite. Lo stesso ordine sarà applicabile a tutto il layout (lead, contatti, account, opportunità)

![](assets/two.png)

**Limiti**

* L’attività (Momento interessante, Attività web, E-mail) è impostata su 1000 per impostazione predefinita. Per impostazione predefinita, le campagne e gli eventi e-mail sono impostati su 200
* Nel caso noti problemi di timeout sull&#39;organizzazione, puoi ridurre il limite

## Approfondimenti vendite marketing {#reset-marketo-sales-insight}

La scelta di questo tipo di configurazione eliminerà tutte le configurazioni della DSC e non sarà possibile ripristinarle. Dovrai riconfigurare tutto.

![](assets/three.png)

>[!MORELIKETHIS]
>
>[Impostazione di Sales Insight per il team](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)
