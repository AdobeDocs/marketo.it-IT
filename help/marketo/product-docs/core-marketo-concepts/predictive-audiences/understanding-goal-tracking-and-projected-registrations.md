---
description: Informazioni sul tracciamento degli obiettivi e sulle registrazioni previste - Documenti Marketo - Documentazione del prodotto
title: Informazioni sul tracciamento degli obiettivi e sulle registrazioni previste
exl-id: 110768f4-46ed-4951-96b2-a97813d7b257
feature: Predictive Audiences
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 0%

---

# Informazioni sul tracciamento degli obiettivi e sulle registrazioni previste {#understanding-goal-tracking-and-projected-registrations}

Ecco come tenere traccia dell’avanzamento dell’obiettivo e comprendere le previsioni di Marketo.

>[!PREREQUISITES]
>
>Per accedere alla maggior parte di queste funzioni, assicurati di abilitare [interruttore di nuova generazione](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md){target="_blank"} per i programmi evento.

>[!NOTE]
>
>Quando un programma evento viene creato nell’esperienza Marketo Classic, la data di inizio dell’evento attualmente corrisponde per impostazione predefinita alla data di creazione dell’evento. Poiché le registrazioni previste tengono conto del tempo che precede la data di inizio di un evento, questi numeri potrebbero non essere precisi se la data di inizio e la data di creazione sono uguali (a meno che non siano impostate intenzionalmente).

## Tracciamento degli obiettivi e registrazioni previste

1. Puoi trovare i dettagli di tracciamento dell’obiettivo in **[!UICONTROL Rapporti]** del programma eventi. In questo esempio, ci sono 150 membri registrati finora contro un obiettivo di 200 (75%).

   ![](assets/understanding-goal-tracking-and-projected-registrations-1.png)

Vedrai anche il tuo **[!UICONTROL Previsto]** registrazioni. Passa il cursore del mouse sull’icona delle informazioni per visualizzare un raggruppamento di questo numero per segmento di probabilità.

![](assets/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>Il grafico Partecipato e Superiore rimarrà vuoto fino al giorno dell&#39;evento.

Se non hai attivato l’interruttore di attivazione, ecco come apparirà nell’interfaccia utente della classe Marketo:

![](assets/understanding-goal-tracking-and-projected-registrations-3.png)

1. Fai clic sull’interruttore Grafico per passare a un raggruppamento dei membri in base alla probabilità di registrazione. Visualizzerai le percentuali di registrazione correnti per ciascun segmento, rispetto alla percentuale media per quel segmento nei tuoi programmi passati.

   ![](assets/understanding-goal-tracking-and-projected-registrations-4.png)

Tutti i membri (registrati e non ancora registrati) sono classificati in base alla probabilità di registrazione. Passa il cursore del mouse sull’icona delle informazioni per vedere come vengono definite queste categorie di probabilità.

![](assets/understanding-goal-tracking-and-projected-registrations-5.png)

>[!NOTE]
>
>I numeri di previsione vengono aggiornati ogni 24 ore fino al giorno dell’evento. Tutti i membri elencati come _Elaborazione_ sarà incluso nel successivo ciclo di calcolo.

## Programmi simili

Puoi ottenere informazioni approfondite sull’evento corrente osservando le prestazioni di programmi simili in passato. Questa sezione mostra fino a 5 programmi simili degli ultimi 6 mesi, con il numero/percentuale di membri che sono stati _Registrato_ o superiore.

Nel calcolare programmi simili, includiamo i seguenti fattori, tra gli altri:

* Tipo di programma
* Canale del programma
* Dimensione del pubblico
* Tag del programma
* Durata dalla creazione dell’evento all’inizio dell’evento
* Durata evento

  ![](assets/understanding-goal-tracking-and-projected-registrations-6.png)

## Recommendations

Nella parte superiore della pagina Rapporti, puoi trovare consigli basati su AI/ML in base all’avanzamento. Controlla periodicamente la disponibilità di suggerimenti e informazioni utili.

![](assets/understanding-goal-tracking-and-projected-registrations-7.png)

## Previsioni a livello di persona

Fai clic su **[!UICONTROL Membri]** per visualizzare tutti i membri del programma. Passa il puntatore del mouse sopra **[!UICONTROL Probabilità di registrazione]** o **[!UICONTROL Probabilità di partecipazione]** barre per visualizzare percentuali e categorizzazioni esatte. Potrai quindi intervenire sui membri di una particolare categoria (ad esempio, tutti coloro che rientrano nella categoria &quot;Meno probabili&quot; per la registrazione) e indirizzarli in modo specifico per aumentare potenzialmente i numeri di registrazione.

![](assets/understanding-goal-tracking-and-projected-registrations-8.png)

>[!NOTE]
>
>La probabilità individuale tiene conto di oltre 40 fattori relativi alla persona, tra cui attributi di profilo, attività della persona e attività precedenti di invito/registrazione/partecipazione.

## Domande frequenti

**D: Cos’è il segmento?**

R: Probabile valore di registrazione compreso tra 0 e 100. Ogni membro del programma dell’evento avrà un valore di probabilità compreso tra 0 e 100.

I valori di probabilità vengono inseriti in tre segmenti:

* Probabilità di registrare > 50% = segmento con alta probabilità
* Probabilità di registrazione da > 25% a &lt;50% = Segmento probabile
* Probabilità di registrazione &lt;25% = segmento meno probabile

Quando una persona ha la probabilità di registrarsi, la previsione rientra in uno di questi segmenti (ogni persona che è membro di un programma rientra in uno di questi segmenti). Ad esempio, se un programma per eventi ha 1000 membri in base alle previsioni di probabilità, questi 1000 verranno distribuiti in _Molto probabile_, _Probabile_, o _Meno probabile_ segmenti.

Pertanto, le persone che rientrano nel segmento Altamente probabile avranno maggiori possibilità di registrarsi all’evento.

Conversione al registro = # delle persone nel segmento registrate diviso per # delle persone che rientrano nel segmento (ad esempio, se 100 persone rientrano nel segmento altamente probabile e 60 di loro si registrano, il tasso di conversione è del 60%).

La percentuale di conversione da registrare seguirà questo schema: Molto probabile > Probabile > Meno probabile.

**D: Come posso utilizzare le informazioni?**

R: La best practice prevede quanto segue:

i. Quando crei un programma, una campagna avanzata utilizza filtri predittivi con &quot;maggiore di X&quot;, che determinerebbe l’esecuzione di una determinata quantità di persone (ad esempio, 1000).

ii. Dopo 24 ore, nella [!UICONTROL Rapporti] scheda puoi visualizzare le registrazioni previste calcolate in base alla probabilità di registrare i valori di tutte le persone attualmente invitate.

iii. Se le registrazioni previste sono inferiori all’obiettivo, dovrai invitare più persone. A questo punto, puoi vedere le informazioni che ti dicono qual è stata la soglia di funzionamento nei programmi passati.

![](assets/understanding-goal-tracking-and-projected-registrations-9.png)

iv. Puoi creare una nuova campagna avanzata con tale soglia per invitare più persone.

v. In qualsiasi momento, se desideri comprendere il motivo per cui viene visualizzato un numero previsto, puoi visualizzare alternativamente la distribuzione del pubblico tra i segmenti e i relativi tassi di conversione del passato, e applicare tali tassi di conversione al pubblico corrente (vedi la schermata seguente).

**D: Cos’è il grafico Segmenti per registrazione?**

R: Tre barre, ciascuna che rappresenta un segmento (molto probabile, probabile, meno probabile).

**Linea tratteggiata viola:** Tasso medio di conversazione per la registrazione in quel segmento, in base a precedenti programmi simili.

**Barra blu:** Percentuale di registrazione di tutte le persone in quel segmento.

![](assets/understanding-goal-tracking-and-projected-registrations-10.png)

Ad esempio, supponiamo che 100 persone abbiano probabilità di registrarsi > 50% e che 60 di quelle 100 persone si siano registrate. Molto probabilmente ha una conversione del 60%. Pertanto, tutti i membri aggiunti al programma hanno la probabilità di registrare valori, quindi vengono inseriti in segmenti e in base al numero di persone registrate in ciascun segmento viene calcolato il tasso di conversione.

**D: Cosa significa &quot;Registrato e superiore&quot;?**

R: Qualsiasi persona elencata come registrata o qualsiasi altro stato con un numero di passaggio uguale o superiore.

È possibile creare nuovi stati di progressione per un programma evento, ma tali stati vengono mappati con stati standard. Considera un caso in cui una persona viene spostata da invitata a ricordato, che è un passaggio più alto rispetto a registrazione. Questa persona verrà anche considerata registrata e visualizzata nel tracciamento dell’obiettivo.

![](assets/understanding-goal-tracking-and-projected-registrations-11.png)

**D: Come vengono calcolate le registrazioni previste?**

R: Vedi sotto.

![](assets/understanding-goal-tracking-and-projected-registrations-12.png)
