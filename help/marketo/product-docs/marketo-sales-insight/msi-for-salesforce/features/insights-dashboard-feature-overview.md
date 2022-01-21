---
unique-page-id: 42762514
description: Panoramica delle funzioni del dashboard di approfondimenti - Documenti Marketo - Documentazione del prodotto
title: Panoramica della funzione del dashboard di Insights
exl-id: a32f8694-faf2-4183-a485-82fd859b77d2
source-git-commit: 15263f9c23c958499aaa2e4e6491b4962c617358
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# Panoramica della funzione del dashboard di Insights {#insights-dashboard-feature-overview}

Ulteriori informazioni sulle funzioni disponibili nel dashboard Informazioni sulle vendite.

>[!PREREQUISITES]
>
>È necessario disporre dell&#39;ultimo pacchetto MSI SFDC e [configurazione](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configuration-for-existing-customers.md).

![](assets/insights-dashboard-feature-overview-1.png)

## Layout dei contatti {#contact-layout}

**Griglia Velocity di coinvolgimento**

* Questa griglia intelligente include Momenti interessanti, e-mail e attività Web negli ultimi 90 giorni
* L&#39;utente può scegliere di &quot;Mostra attività account&quot;, questo stratificherà tutti i livelli di account Momenti interessanti, E-mail e attività web nella visualizzazione contatti
* L&#39;utente può evidenziare una settimana specifica per visualizzare le attività entro quella settimana
* Vista predefinita: La settimana corrente è selezionata

**Drill down e riepilogo del coinvolgimento**

* Approfondisci le schede delle attività per i momenti interessanti, le attività e-mail e web
* Scheda attività Momenti interessanti : include l’opzione di abbonamento
* Scheda Attività e-mail - Opzione Anteprima
* Scheda Attività web : consente di fare clic sul collegamento
* La barra Riepilogo settimanale mostrerà Momenti interessanti, E-mail e attività Web per quella settimana. Ogni icona è cliccabile e può essere utilizzata come filtro per mostrare un’attività specifica
* Vista predefinita: Elenco delle attività della visualizzazione corrente

**Prossime campagne ed eventi e-mail**

Scheda Campagne e-mail:

* Include campagne che fanno parte di programmi e-mail o programmi predefiniti pianificati nei successivi 90 giorni
* Non specifico per il contatto/lead (ad esempio, l’elenco delle campagne è un elenco generico di tutte le campagne e-mail pianificate nell’istanza Marketo). L’elenco delle campagne nei pannelli lead, contatti, account e opportunità sarà lo stesso
* Se la ricorrenza della campagna è tale che viene eseguita più di tre volte nei successivi 90 giorni, verranno visualizzate solo le tre esecuzioni successive in un dato momento (simile al comportamento in Marketo)
* La scheda dei dettagli dell’attività in questa sezione dispone di un’opzione di anteprima. Se il flusso include più passaggi e-mail di invio, tutte le e-mail saranno disponibili per l’anteprima. Nel passaggio di invio del flusso e-mail, se sono presenti più &quot;scelte e-mail&quot;, l’opzione predefinita sarà disponibile per l’anteprima
* I filtri includono &quot;Search&quot; e &quot;Date Range&quot;

![](assets/insights-dashboard-feature-overview-2.png)

Scheda Evento:

* Include i programmi evento pianificati nei prossimi 90 giorni
* Utilizza l’opzione filtro per visualizzare tutti gli eventi/eventi invitati (in base alle impostazioni amministratore)
* La selezione degli eventi invitati mostrerà gli eventi a cui è stato invitato un contatto specifico insieme allo stato membro
* Selezionando tutti gli eventi verrà visualizzato l’elenco degli eventi pianificati nei successivi 90 giorni
* La scheda dei dettagli dell’attività in questa sezione presenta l’opzione di anteprima
* Il filtro include &quot;Ricerca&quot;, &quot;Mostra solo eventi invitati&quot; e &quot;Intervallo date&quot;

![](assets/insights-dashboard-feature-overview-3.png)

## Layout lead {#lead-layout}

**Griglia Velocity di coinvolgimento**

* Questa griglia intelligente include Momenti interessanti, e-mail e attività Web negli ultimi 90 giorni
* L&#39;utente può evidenziare una settimana specifica per visualizzare le attività entro quella settimana
* Vista predefinita: La settimana corrente è selezionata
* La funzione &quot;Mostra attività account&quot; non è disponibile sui lead in quanto non fa parte di alcun account in Salesforce finché non viene convertita in un contatto

**Drill down e riepilogo del coinvolgimento**

* Schede di attività drill-down per momenti interessanti, e-mail e attività web
* Scheda attività Momenti interessanti : include l’opzione di abbonamento
* Scheda Attività e-mail - Opzione Anteprima
* Scheda Attività web : consente di fare clic sul collegamento
* La barra Riepilogo settimanale mostrerà Momenti interessanti, E-mail e attività Web per quella settimana. Ogni icona è cliccabile e può essere utilizzata come filtro per mostrare un’attività specifica
* Vista predefinita: Elenco delle attività della visualizzazione corrente

**Prossime campagne ed eventi e-mail:**

Scheda Campagne e-mail:

* Include campagne che fanno parte di programmi e-mail o programmi predefiniti pianificati nei successivi 90 giorni
* Non specifico per il contatto/lead (ad esempio, l’elenco delle campagne è un elenco generico di tutte le campagne e-mail pianificate nell’istanza Marketo). L’elenco delle campagne nei pannelli lead, contatti, account e opportunità sarà lo stesso
* Se la ricorrenza della campagna è tale che viene eseguita più di tre volte nei successivi 90 giorni, verranno visualizzate solo le tre esecuzioni successive in un dato momento (simile al comportamento in Marketo)
* La scheda dei dettagli dell’attività in questa sezione dispone di un’opzione di anteprima. Se il flusso include più passaggi e-mail di invio, tutte le e-mail saranno disponibili per l’anteprima. Nel passaggio di invio del flusso e-mail, se sono presenti più &quot;scelte e-mail&quot;, l’opzione predefinita sarà disponibile per l’anteprima
* I filtri includono &quot;Search&quot; e &quot;Date Range&quot;

![](assets/insights-dashboard-feature-overview-4.png)

Scheda Evento:

* Include i programmi evento pianificati nei prossimi 90 giorni
* Utilizza l’opzione filtro per visualizzare tutti gli eventi/eventi invitati (in base alle impostazioni amministratore)
* La selezione degli eventi invitati mostrerà gli eventi a cui è stato invitato un contatto specifico insieme allo stato membro
* Selezionando tutti gli eventi verrà visualizzato l’elenco degli eventi pianificati nei successivi 90 giorni
* La scheda dei dettagli dell’attività in questa sezione presenta l’opzione di anteprima
* Il filtro include &quot;Ricerca&quot;, &quot;Mostra solo eventi invitati&quot; e &quot;Intervallo date&quot;

![](assets/insights-dashboard-feature-overview-5.png)

## Layout account {#account-layout}

**Griglia Velocity di coinvolgimento**

* Questa griglia intelligente include Momenti interessanti, E-mail e attività Web negli ultimi 90 giorni per tutti i contatti dell&#39;account
* L&#39;utente può evidenziare una settimana specifica per visualizzare le attività entro quella settimana
* Vista predefinita: La settimana corrente è selezionata

**Drill-down e riepilogo del coinvolgimento**

* Schede di attività drill-down per Momenti interessanti, E-mail e attività web, incluso il nome del contatto
* Scheda attività Momenti interessanti : include l’opzione di abbonamento
* Scheda Attività e-mail - Opzione Anteprima
* Scheda Attività web : consente di fare clic sul collegamento
* La barra Riepilogo settimanale mostrerà Momenti interessanti, E-mail e attività Web per quella settimana. Ogni icona è cliccabile e può essere utilizzata come filtro per mostrare un’attività specifica
* Vista predefinita: Elenco delle attività della visualizzazione corrente

**Prossime campagne ed eventi e-mail**

Scheda Campagne e-mail:

* Include campagne che fanno parte di programmi e-mail o programmi predefiniti pianificati nei successivi 90 giorni
* Non specifico per il contatto/lead (ad esempio, l’elenco delle campagne è un elenco generico di tutte le campagne e-mail pianificate nell’istanza Marketo). L’elenco delle campagne nei pannelli lead, contatti, account e opportunità sarà lo stesso
* Se la ricorrenza della campagna è tale che viene eseguita più di tre volte nei successivi 90 giorni, verranno visualizzate solo le tre esecuzioni successive in un dato momento (simile al comportamento in Marketo)
* La scheda dei dettagli dell’attività in questa sezione dispone di un’opzione di anteprima. Se il flusso include più passaggi e-mail di invio, tutte le e-mail saranno disponibili per l’anteprima. Nel passaggio di invio del flusso e-mail, se sono presenti più &quot;scelte e-mail&quot;, l’opzione predefinita sarà disponibile per l’anteprima
* I filtri includono &quot;Search&quot; e &quot;Date Range&quot;

Scheda Evento:

* Include i programmi evento pianificati nei prossimi 90 giorni
* Utilizza l’opzione filtro per visualizzare tutti gli eventi/eventi invitati (in base alle impostazioni amministratore)
* La selezione degli eventi invitati mostrerà gli eventi a cui è stato invitato un contatto specifico insieme allo stato membro
* Selezionando tutti gli eventi verrà visualizzato l’elenco degli eventi pianificati nei successivi 90 giorni
* La scheda dei dettagli dell’attività in questa sezione presenta l’opzione di anteprima
* Il filtro include &quot;Ricerca&quot;, &quot;Mostra solo eventi invitati&quot; e &quot;Intervallo date&quot;

## Layout opportunità {#opportunity-layout}

**Griglia Velocity di coinvolgimento**

* Questa griglia intelligente include Momenti interessanti, e-mail e attività Web negli ultimi 90 giorni per tutti i contatti nell&#39;opportunità
* L&#39;utente può evidenziare una settimana specifica per visualizzare le attività entro quella settimana
* Vista predefinita: La settimana corrente è selezionata

**Drill-down e riepilogo del coinvolgimento**

* Schede di attività drill-down per Momenti interessanti, E-mail e attività web, incluso il nome del contatto
* Scheda attività Momenti interessanti : include l’opzione di abbonamento
* Scheda Attività e-mail - Opzione Anteprima
* Scheda Attività web : consente di fare clic sul collegamento
* La barra Riepilogo settimanale mostrerà Momenti interessanti, E-mail e attività Web per quella settimana. Ogni icona è cliccabile e può essere utilizzata come filtro per mostrare un’attività specifica
* Vista predefinita: Elenco delle attività della visualizzazione corrente

**Prossime campagne ed eventi e-mail** Scheda Campagne e-mail:

* Include campagne che fanno parte di programmi e-mail o programmi predefiniti pianificati nei successivi 90 giorni
* Non specifico per il contatto/lead (ad esempio, l’elenco delle campagne è un elenco generico di tutte le campagne e-mail pianificate nell’istanza Marketo). L’elenco delle campagne nei pannelli lead, contatti, account e opportunità sarà lo stesso
* Se la ricorrenza della campagna è tale che viene eseguita più di tre volte nei successivi 90 giorni, verranno visualizzate solo le tre esecuzioni successive in un dato momento (simile al comportamento in Marketo)
* La scheda dei dettagli dell’attività in questa sezione dispone di un’opzione di anteprima. Se il flusso include più passaggi e-mail di invio, tutte le e-mail saranno disponibili per l’anteprima. Nel passaggio di invio del flusso e-mail, se sono presenti più &quot;scelte e-mail&quot;, l’opzione predefinita sarà disponibile per l’anteprima
* I filtri includono &quot;Search&quot; e &quot;Date Range&quot;

Scheda Evento:

* Include i programmi evento pianificati nei prossimi 90 giorni
* Utilizza l’opzione filtro per visualizzare tutti gli eventi/eventi invitati (in base alle impostazioni amministratore)
* La selezione degli eventi invitati mostrerà gli eventi a cui è stato invitato un contatto specifico insieme allo stato membro
* Selezionando tutti gli eventi verrà visualizzato l’elenco degli eventi pianificati nei successivi 90 giorni
* La scheda dei dettagli dell’attività in questa sezione presenta l’opzione di anteprima
* Il filtro include &quot;Ricerca&quot;, &quot;Mostra solo eventi invitati&quot; e &quot;Intervallo date&quot;

>[!NOTE]
>
>Se il tuo account o opportunità dispone di più di 800 contatti, il dashboard non visualizzerà alcun dato. Tuttavia, puoi passare ai singoli contatti per vedere le loro informazioni e il loro coinvolgimento. Se il tuo account ha più di 800 contatti, &quot;Mostra attività a livello di account&quot; verrà disattivato.
