---
unique-page-id: 42762514
description: Scopri la dashboard di approfondimenti in Marketo Sales Insight. Visualizza la velocità di coinvolgimento, le campagne e le attività imminenti nel pannello.
title: Panoramica delle funzioni della dashboard Approfondimenti
exl-id: a32f8694-faf2-4183-a485-82fd859b77d2
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/pMPRzDtLNKUNPoOSV9F9OxsiYFdHrU2wYpGQMZAJ7hQ
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2:
  - id: d5f08d55-2fea-44e2-b699-c9c3a8a79cf1
  - id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 1489
ht-degree: 0%

---

# Panoramica delle funzioni della dashboard Approfondimenti {#insights-dashboard-feature-overview}

Ulteriori informazioni sulle funzionalità disponibili nel dashboard di [!DNL Sales Insights].

>[!PREREQUISITES]
>
>È necessario disporre del pacchetto SFDC MSI più recente e della [configurazione](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

![](assets/insights-dashboard-feature-overview-1.png)

## Layout contatto {#contact-layout}

**Griglia Velocità Di Coinvolgimento**

* Questa griglia intelligente include i momenti di interesse, e-mail e attività Web negli ultimi 90 giorni
* L&#39;utente può scegliere di &quot;[!UICONTROL Show Account]&quot; l&#39;attività, in questo modo verrà impostato il livello Tutti i momenti di interesse dell&#39;account, l&#39;attività Web e di posta elettronica nella visualizzazione Contatto
* L’utente può evidenziare una settimana specifica per visualizzare le attività entro tale settimana
* Visualizzazione predefinita: è selezionata la settimana corrente

**Espansione e riepilogo del coinvolgimento**

* Espandere schede attività per i momenti di interesse, e-mail e attività web
* Scheda Attività Momenti di interesse - Include l’opzione di abbonamento
* Scheda Attività e-mail - Include l’opzione Anteprima
* Scheda Attività Web: include la possibilità di fare clic sul collegamento
* La barra di riepilogo settimanale mostra i momenti di interesse, l’e-mail e l’attività web per quella settimana. Ogni icona è cliccabile e può essere usata come filtro per mostrare un’attività specifica
* Visualizzazione predefinita: elenco delle attività della visualizzazione corrente

**Prossime campagne ed eventi e-mail**

Scheda Campagne e-mail:

* Include campagne che fanno parte di programmi e-mail o programmi predefiniti pianificati nei successivi 90 giorni
* Non specifico per il contatto/lead (ad esempio, l’elenco delle campagne è un elenco generico di tutte le campagne e-mail pianificate nell’istanza di Marketo). L’elenco delle campagne in tutti i pannelli lead, contatto, account e opportunità sarà lo stesso
* Se la ricorrenza della campagna è tale che viene eseguita più di tre volte nei successivi 90 giorni, verranno mostrate solo le tre esecuzioni successive in un dato momento (in modo simile al comportamento in Marketo)
* La scheda dei dettagli dell’attività in questa sezione avrà un’opzione di anteprima. Se il flusso include più passaggi dell’e-mail di invio, tutte le e-mail saranno disponibili per l’anteprima. Nel passaggio Invia flusso e-mail, se sono presenti più &quot;scelte e-mail&quot;, l’opzione predefinita sarà disponibile per l’anteprima
* I filtri includono &quot;[!UICONTROL Search]&quot; e &quot;[!UICONTROL Date Range]&quot;

![](assets/insights-dashboard-feature-overview-2.png)

Scheda Evento:

* Include i programmi evento pianificati nei prossimi 90 giorni
* Utilizza l’opzione di filtro per visualizzare tutti gli eventi/eventi invitati (in base alle impostazioni dell’amministratore)
* Selezionando gli eventi invitati verranno visualizzati gli eventi a cui è stato invitato il contatto specifico, insieme allo stato del membro
* Selezionando tutti gli eventi verrà visualizzato l’elenco degli eventi pianificati nei successivi 90 giorni
* La scheda Dettagli attività in questa sezione presenta l’opzione di anteprima
* Il filtro include &quot;[!UICONTROL Search]&quot;, &quot;[!UICONTROL Show only invited events]&quot; e &quot;[!UICONTROL Date Range]&quot;

![](assets/insights-dashboard-feature-overview-3.png)

## Layout lead {#lead-layout}

**Griglia Velocità Di Coinvolgimento**

* Questa griglia intelligente include i momenti di interesse, e-mail e attività Web negli ultimi 90 giorni
* L’utente può evidenziare una settimana specifica per visualizzare le attività entro tale settimana
* Visualizzazione predefinita: è selezionata la settimana corrente
* La funzionalità &quot;[!UICONTROL Show Account Activity]&quot; non è disponibile per i lead perché non fa parte di alcun account in [!DNL Salesforce] finché non viene convertita in un contatto

**Espansione e riepilogo del coinvolgimento**

* Schede di attività drill-down per i momenti di interesse, e-mail e attività web
* Scheda Attività Momenti di interesse - Include l’opzione di abbonamento
* Scheda Attività e-mail - Include l’opzione Anteprima
* Scheda Attività Web: include la possibilità di fare clic sul collegamento
* La barra di riepilogo settimanale mostra i momenti di interesse, l’e-mail e l’attività web per quella settimana. Ogni icona è cliccabile e può essere usata come filtro per mostrare un’attività specifica
* Visualizzazione predefinita: elenco delle attività della visualizzazione corrente

**Prossime campagne ed eventi e-mail:**

Scheda Campagne e-mail:

* Include campagne che fanno parte di programmi e-mail o programmi predefiniti pianificati nei successivi 90 giorni
* Non specifico per il contatto/lead (ad esempio, l’elenco delle campagne è un elenco generico di tutte le campagne e-mail pianificate nell’istanza di Marketo). L’elenco delle campagne in tutti i pannelli lead, contatto, account e opportunità sarà lo stesso
* Se la ricorrenza della campagna è tale che viene eseguita più di tre volte nei successivi 90 giorni, verranno mostrate solo le tre esecuzioni successive in un dato momento (in modo simile al comportamento in Marketo)
* La scheda dei dettagli dell’attività in questa sezione avrà un’opzione di anteprima. Se il flusso include più passaggi dell’e-mail di invio, tutte le e-mail saranno disponibili per l’anteprima. Nel passaggio Invia flusso e-mail, se sono presenti più &quot;scelte e-mail&quot;, l’opzione predefinita sarà disponibile per l’anteprima
* I filtri includono &quot;[!UICONTROL Search]&quot; e &quot;[!UICONTROL Date Range]&quot;

![](assets/insights-dashboard-feature-overview-4.png)

Scheda Evento:

* Include i programmi evento pianificati nei prossimi 90 giorni
* Utilizza l’opzione di filtro per visualizzare tutti gli eventi/eventi invitati (in base alle impostazioni dell’amministratore)
* Selezionando gli eventi invitati verranno visualizzati gli eventi a cui è stato invitato il contatto specifico, insieme allo stato del membro
* Selezionando tutti gli eventi verrà visualizzato l’elenco degli eventi pianificati nei successivi 90 giorni
* La scheda Dettagli attività in questa sezione presenta l’opzione di anteprima
* Il filtro include &quot;[!UICONTROL Search]&quot;, &quot;[!UICONTROL Show only invited events]&quot; e &quot;[!UICONTROL Date Range]&quot;

![](assets/insights-dashboard-feature-overview-5.png)

## Layout account {#account-layout}

**Griglia Velocità Di Coinvolgimento**

* Questa griglia intelligente include i momenti di interesse, e-mail e attività Web degli ultimi 90 giorni per tutti i contatti nell’account
* L’utente può evidenziare una settimana specifica per visualizzare le attività entro tale settimana
* Visualizzazione predefinita: è selezionata la settimana corrente

**Drill-down e riepilogo del coinvolgimento**

* Schede di attività drill-down per i momenti di interesse, e-mail e attività web, compreso il nome del contatto
* Scheda Attività Momenti di interesse - Include l’opzione di abbonamento
* Scheda Attività e-mail - Include l’opzione Anteprima
* Scheda Attività Web: include la possibilità di fare clic sul collegamento
* La barra di riepilogo settimanale mostra i momenti di interesse, l’e-mail e l’attività web per quella settimana. Ogni icona è cliccabile e può essere usata come filtro per mostrare un’attività specifica
* Visualizzazione predefinita: elenco delle attività della visualizzazione corrente

**Prossime campagne ed eventi e-mail**

Scheda Campagne e-mail:

* Include campagne che fanno parte di programmi e-mail o programmi predefiniti pianificati nei successivi 90 giorni
* Non specifico per il contatto/lead (ad esempio, l’elenco delle campagne è un elenco generico di tutte le campagne e-mail pianificate nell’istanza di Marketo). L’elenco delle campagne in tutti i pannelli lead, contatto, account e opportunità sarà lo stesso
* Se la ricorrenza della campagna è tale che viene eseguita più di tre volte nei successivi 90 giorni, verranno mostrate solo le tre esecuzioni successive in un dato momento (in modo simile al comportamento in Marketo)
* La scheda dei dettagli dell’attività in questa sezione avrà un’opzione di anteprima. Se il flusso include più passaggi dell’e-mail di invio, tutte le e-mail saranno disponibili per l’anteprima. Nel passaggio Invia flusso e-mail, se sono presenti più &quot;scelte e-mail&quot;, l’opzione predefinita sarà disponibile per l’anteprima
* I filtri includono &quot;[!UICONTROL Search]&quot; e &quot;[!UICONTROL Date Range]&quot;

Scheda Evento:

* Include i programmi evento pianificati nei prossimi 90 giorni
* Utilizza l’opzione di filtro per visualizzare tutti gli eventi/eventi invitati (in base alle impostazioni dell’amministratore)
* Selezionando gli eventi invitati verranno visualizzati gli eventi a cui è stato invitato il contatto specifico, insieme allo stato del membro
* Selezionando tutti gli eventi verrà visualizzato l’elenco degli eventi pianificati nei successivi 90 giorni
* La scheda Dettagli attività in questa sezione presenta l’opzione di anteprima
* Il filtro include &quot;[!UICONTROL Search]&quot;, &quot;[!UICONTROL Show only invited events]&quot; e &quot;[!UICONTROL Date Range]&quot;

## Layout opportunità {#opportunity-layout}

**Griglia Velocità Di Coinvolgimento**

* Questa griglia intelligente include i momenti di interesse, e-mail e attività Web degli ultimi 90 giorni per tutti i contatti nell’opportunità
* L’utente può evidenziare una settimana specifica per visualizzare le attività entro tale settimana
* Visualizzazione predefinita: è selezionata la settimana corrente

**Drill-down e riepilogo del coinvolgimento**

* Schede di attività drill-down per i momenti di interesse, e-mail e attività web, compreso il nome del contatto
* Scheda Attività Momenti di interesse - Include l’opzione di abbonamento
* Scheda Attività e-mail - Include l’opzione Anteprima
* Scheda Attività Web: include la possibilità di fare clic sul collegamento
* La barra di riepilogo settimanale mostra i momenti di interesse, l’e-mail e l’attività web per quella settimana. Ogni icona è cliccabile e può essere usata come filtro per mostrare un’attività specifica
* Visualizzazione predefinita: elenco delle attività della visualizzazione corrente

**Prossime campagne ed eventi e-mail** scheda Campagne e-mail:

* Include campagne che fanno parte di programmi e-mail o programmi predefiniti pianificati nei successivi 90 giorni
* Non specifico per il contatto/lead (ad esempio, l’elenco delle campagne è un elenco generico di tutte le campagne e-mail pianificate nell’istanza di Marketo). L’elenco delle campagne in tutti i pannelli lead, contatto, account e opportunità sarà lo stesso
* Se la ricorrenza della campagna è tale che viene eseguita più di tre volte nei successivi 90 giorni, verranno mostrate solo le tre esecuzioni successive in un dato momento (in modo simile al comportamento in Marketo)
* La scheda dei dettagli dell’attività in questa sezione avrà un’opzione di anteprima. Se il flusso include più passaggi dell’e-mail di invio, tutte le e-mail saranno disponibili per l’anteprima. Nel passaggio Invia flusso e-mail, se sono presenti più &quot;scelte e-mail&quot;, l’opzione predefinita sarà disponibile per l’anteprima
* I filtri includono &quot;[!UICONTROL Search]&quot; e &quot;[!UICONTROL Date Range]&quot;

Scheda Evento:

* Include i programmi evento pianificati nei prossimi 90 giorni
* Utilizza l’opzione di filtro per visualizzare tutti gli eventi/eventi invitati (in base alle impostazioni dell’amministratore)
* Selezionando gli eventi invitati verranno visualizzati gli eventi a cui è stato invitato il contatto specifico, insieme allo stato del membro
* Selezionando tutti gli eventi verrà visualizzato l’elenco degli eventi pianificati nei successivi 90 giorni
* La scheda Dettagli attività in questa sezione presenta l’opzione di anteprima
* Il filtro include &quot;[!UICONTROL Search]&quot;, &quot;[!UICONTROL Show only invited events]&quot; e &quot;[!UICONTROL Date Range]&quot;

>[!NOTE]
>
>Se l’account o l’opportunità dispone di più di 800 contatti, la dashboard non visualizzerà alcun dato. Tuttavia, puoi andare dai singoli contatti per visualizzarne approfondimenti e coinvolgimento. Se il tuo account ha più di 800 contatti, &quot;[!UICONTROL Show Account Level Activity]&quot; verrà disabilitato.
