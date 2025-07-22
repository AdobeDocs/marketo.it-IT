---
unique-page-id: 42762322
description: Scheda Configurazione di Marketo Sales Insight in Salesforce - Documentazione di Marketo - Documentazione del prodotto
title: Scheda Configurazione di Marketo Sales Insight in Salesforce
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---

# Scheda Configurazione [!DNL Marketo Sales Insight] in [!DNL Salesforce] {#marketo-sales-insight-configuration-tab-in-salesforce}

## Impostazioni operative {#operational-settings}

Per iniziare a utilizzare [!DNL Sales Insight] in SFDC è necessario configurarlo.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI utilizza sia Soap che Rest API
* La pagina Insight di vendita del tuo account Marketo avrà due pannelli corrispondenti con credenziali API Soap e Rest che puoi copiare e incollare qui
* Le API Soap e Rest hanno timeout separati che puoi impostare in base alle esigenze della tua organizzazione. Il tempo massimo consentito è di 120 secondi
* Disabilitazione della dashboard di Insights: puoi rimuovere le credenziali API REST e utilizzare solo l’API Soap. Così facendo, disabiliterai la scheda Dashboard approfondimenti in tutti i pannelli MSI visualforce

## Configurazione MSI {#msi-configuration}

Le configurazioni sono applicabili a tutti gli utenti MSI e non sono specifiche per i profili.

**Impostazioni pagina Visualforce**

* Menu a discesa Abilita azione:
   * Possibilità di nascondere l’elenco a discesa Invia e-mail Marketo in Layout MSI lead e contatto
   * Possibilità di nascondere le opzioni Aggiungi a Marketo Campaign dall’elenco a discesa in Layout MSI lead e contatto
* Prossimi eventi: possibilità di mostrare gli eventi invitati, tutti gli eventi agli utenti o nascondere completamente questa scheda
* Prossime campagne: possibilità di mostrare tutte le campagne e-mail o nascondere completamente questa scheda
* Caricare campagne ed eventi futuri: possibilità di ridurre il numero di chiamate API REST effettuate dagli utenti posizionando la scheda eventi e campagne dietro un pulsante &quot;Carica prossimi elementi&quot; on-demand
* Impostazioni scheda: per impostazione predefinita, tutte e cinque le schede sono disponibili. Potete scegliere l&#39;ordine delle schede nel pannello Insight vendite. Lo stesso ordine sarà applicabile a tutti i layout (lead, contatto, account, opportunità)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**Scheda globale Marketo**

* Feed RSS abilitato: se attivato, gli utenti MSI possono visualizzare il proprio feed lead in un feed RSS (oltre al feed lead in Salesforce). Il feed RSS può funzionare solo se la funzione &quot;Scadenza token&quot; è disabilitata. Questa impostazione è controllata nella pagina di amministrazione di Marketo Sales Insight.
* Modalità di debug elementi di maggiore rilevanza
* Nascondi predefinito: l’opzione scelta qui corrisponde al numero di giorni in cui la puntata migliore verrà nascosta nella scheda Elementi di maggiore rilevanza in Marketo, quando si fa clic sull’icona &quot;Nascondi&quot;
* Campo stato contatto: l&#39;opzione scelta in questo campo sarà il valore inserito nella colonna Intestazione stato della scheda Elementi di maggiore rilevanza di Marketo
* Impostazioni feed live: opzione che consente di visualizzare solo feed live (nei pannelli Lead, Contatto, Account e Opportunità e nella pagina Marketo globale), solo feed lead (nella pagina globale di Marketo) o entrambi
* Impostazioni scheda: per impostazione predefinita, tutte e cinque le schede sono disponibili. È possibile scegliere l&#39;ordine delle schede nella pagina globale di Marketo

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**Limiti**

* L’attività (Momento di interesse, Attività web, E-mail) è impostata su 1000 per impostazione predefinita. Le campagne e gli eventi e-mail sono impostati su 200 per impostazione predefinita
* Se noti problemi di timeout nell’organizzazione, puoi ridurre il limite

**Impostazioni azione**

* Invia e-mail Marketo: questa opzione consente a tutti gli utenti di Sales Insight di accedere per inviare e-mail dai pannelli Lead, Contatto, Account, Opportunità e dalla scheda Elementi di maggiore rilevanza (azioni in blocco e coinvolgimento in linea)
* Aggiungi a Marketo Campaign: questa opzione consente a tutti gli utenti di Sales Insight di accedere alle campagne da lead, contatti, account, pannelli opportunità e scheda elementi di maggiore rilevanza (azioni in blocco e coinvolgimento in linea)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## Impostazioni di supporto {#support-settings}

Selezionando questa casella di controllo verrà abilitata la registrazione di debug nell’istanza di Salesforce. Può essere utile per risolvere eventuali problemi.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

## Reimposta Insight di vendita Marketo {#reset-marketo-sales-insight}

Scegliendo questa opzione, tutte le configurazioni in SFDC verranno cancellate e non potranno essere ripristinate. Dovrai riconfigurare tutto.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-6.png)

>[!IMPORTANT]
>
>Non selezionare la casella di controllo &quot;Abilita azioni MSI&quot; a meno che non si utilizzino le funzioni Azioni di Informazioni sulle vendite.

>[!MORELIKETHIS]
>
>[Aggiungere l&#39;accesso di Insight alle vendite ai profili](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
