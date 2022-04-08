---
unique-page-id: 42762322
description: Scheda Configurazione Marketo Sales Insight in Salesforce - Documenti Marketo - Documentazione del prodotto
title: Scheda di configurazione Marketo Sales Insight in Salesforce
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Scheda di configurazione Marketo Sales Insight in Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Impostazioni operative {#operational-settings}

Sarà necessario impostare questa impostazione per iniziare a utilizzare Sales Insight in SFDC.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI utilizza sia l’API Soap che Rest
* Nella pagina Approfondimenti vendite del tuo account Marketo saranno presenti due pannelli corrispondenti con le credenziali API Soap e Rest che puoi copiare e incollare qui
* Le API Soap e Rest dispongono di timeout separati che puoi impostare in base alle esigenze della tua organizzazione. Il tempo massimo consentito è di 120 secondi
* Disabilitazione del dashboard di Insights: Puoi rimuovere le credenziali API per il resto e utilizzare solo l’API Soap. In questo modo si disabilita la scheda Dashboard approfondimenti in tutti i pannelli della forza visivo MSI

## Configurazione MSI {#msi-configuration}

Le configurazioni sono applicabili a tutti gli utenti MSI e non sono specifiche per i profili.

**Impostazioni pagina della visualizzazione**

* Menu a discesa Abilita azione :
   * Possibilità di nascondere l’elenco a discesa Invia e-mail Marketo nel layout Lead e Contatta MSI
   * Possibilità di nascondere le opzioni Aggiungi a Marketo Campaign dal menu a discesa in Layout lead e Contatta MSI
* Prossimi eventi: Possibilità di mostrare gli eventi invitati, tutti gli eventi agli utenti o nascondere completamente questa scheda
* Prossime campagne: Possibilità di mostrare tutte le campagne e-mail o nascondere completamente questa scheda
* Carica campagne ed eventi in arrivo: Possibilità di ridurre il numero di chiamate API rimanenti effettuate dagli utenti inserendo gli eventi e la scheda delle campagne dietro un pulsante &quot;Carica gli elementi in arrivo&quot; on-demand
* Impostazioni scheda: Per impostazione predefinita saranno disponibili tutte e cinque le schede. È possibile scegliere l&#39;ordine delle schede nel pannello Approfondimenti vendite. Lo stesso ordine sarà applicabile a tutti i layout (lead, contatti, account, opportunità)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**Scheda globale Marketo**

* Feed RSS abilitato: Quando abilitato, gli utenti MSI possono visualizzare il proprio feed lead in un feed RSS (oltre al feed lead in Salesforce). Il feed RSS può funzionare solo se la funzione &quot;Scadenza token&quot; è disabilitata. Questa impostazione è controllata nella pagina Marketo Sales Insight Admin.
* Modalità di debug delle migliori operazioni
* Nascondi predefinito: L&#39;opzione che scegli qui sarà il numero di giorni in cui una scommessa migliore sarà nascosta nella scheda Best Bets in Marketo quando fai clic sull&#39;icona &quot;Nascondi&quot;
* Campo Stato contatto: L’opzione selezionata sarà il valore compilato nella colonna Intestazione di stato della scheda Best Bets in Marketo
* Impostazioni feed live: Opzione per scegliere di mostrare solo i feed live (nei pannelli Lead, Contatto, Account e Opportunità e nella pagina Marketo globale), solo i feed lead (nella pagina globale Marketo) o entrambi i feed Live e Lead
* Impostazioni scheda: Per impostazione predefinita saranno disponibili tutte e cinque le schede. Puoi scegliere l’ordine delle schede nella pagina globale Marketo

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**Limiti**

* L’attività (Momento interessante, Attività web, E-mail) è impostata su 1000 per impostazione predefinita. Per impostazione predefinita, le campagne e gli eventi e-mail sono impostati su 200
* Nel caso noti problemi di timeout sull&#39;organizzazione, puoi ridurre il limite

**Impostazioni azione**

* Invia e-mail Marketo: In questo modo tutti gli utenti di Sales Insight avranno accesso all’invio di e-mail dai pannelli Lead, Contatto, Account, Opportunità e dalla scheda Best Bets (azioni in blocco e coinvolgimento in linea)
* Aggiungi a Marketo Campaign: L’abilitazione di questo consente a tutti gli utenti di Sales Insight di accedere alle campagne dai pannelli Lead, Contact, Account, Opportunity e dalla scheda Best Bets (azioni in blocco e coinvolgimento in linea)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## Reimposta analisi vendite Marketo {#reset-marketo-sales-insight}

La scelta di questo tipo di configurazione eliminerà tutte le configurazioni della DSC e non sarà possibile ripristinarle. Dovrai riconfigurare tutto.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

>[!IMPORTANT]
>
>Non selezionare la casella di controllo &quot;Abilita azioni MSI&quot; a meno che non si utilizzino le funzioni Azioni Approfondimenti vendite.

>[!MORELIKETHIS]
>
>[Aggiungi accesso a informazioni sulle vendite nei profili](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;}
