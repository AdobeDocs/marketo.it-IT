---
title: tracking-obiettivo-obiettivo-e-proiezioni-registrazioni
description: Comprendere il tracciamento degli obiettivi e le registrazioni previste
translation-type: tm+mt
source-git-commit: 1231bc32a3abdf66c10864d6605234763618dbe0
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 0%

---


# Comprendere il tracciamento degli obiettivi e le registrazioni previste

<br> 

Dopo aver [fissato gli obiettivi](/help/sky/setting-event-goals.md)dell&#39;evento e aver inviato gli inviti tramite una campagna [](/help/sky/create-a-smart-campaign.md)intelligente, ecco come monitorare i progressi dell&#39;obiettivo e capire le previsioni di Marketo.

>[!NOTE]
>
>Quando un programma evento viene creato nell&#39;esperienza Marketo Classic, la data di inizio dell&#39;evento è impostata per impostazione predefinita sulla data di creazione dell&#39;evento. Poiché le registrazioni previste tengono conto del tempo trascorso prima della data di inizio di un evento, questi numeri potrebbero non essere precisi se la data di inizio e la data di creazione sono uguali (a meno che non siano impostati intenzionalmente).

## Tracciamento degli obiettivi e registrazioni previste

1. Potete trovare i dettagli di tracciamento obiettivo nella scheda [!UICONTROL **Rapporti**] del programma dell&#39;evento. In questo particolare esempio, ci sono 150 iscritti finora contro l&#39;obiettivo di 200 (75%).

   ![Immagine uno](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-1.png)

Verranno inoltre visualizzate le registrazioni [!UICONTROL **previste**] . Passa il cursore del mouse sull’icona info per visualizzare una suddivisione di questo numero per segmento probabilità.

![Immagine due](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>Il grafico Partecipanti e Superiore rimarrà vuoto fino al giorno dell’evento.

1. Fate clic sull’interruttore Grafico per passare a una suddivisione dei membri in base alla probabilità di registrazione. Verranno visualizzate le percentuali di registrazione correnti per ciascun segmento, confrontate con la percentuale media per quel segmento nei programmi passati.

   ![Immagine tre](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-3.png)

Tutti i membri (registrati e non ancora registrati) sono classificati in base alla loro probabilità di registrazione. Passate il puntatore sull’icona delle informazioni per vedere come vengono definite queste categorie di probabilità.

![Immagine quattro](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-4.png)

>[!NOTE]
>
>I numeri di previsione vengono aggiornati ogni 24 ore fino al giorno dell’evento. Tutti i membri elencati come _Elaborazione_ verranno inclusi nel prossimo ciclo di calcolo.

## Programmi simili

È possibile ottenere informazioni dettagliate sull&#39;evento corrente analizzando le prestazioni di programmi simili in passato. Questa sezione mostra fino a 5 programmi simili degli ultimi 6 mesi, con il numero/percentuale di membri _registrati_ o superiori.

Nel calcolo di programmi simili, includiamo, tra l&#39;altro, i seguenti fattori:

* Tipo di programma
* Canale del programma
* Dimensione dell&#39;audience
* Tag programma
* Durata del tempo dalla creazione dell&#39;evento all&#39;inizio dell&#39;evento
* Durata evento

   ![Immagine cinque](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-5.png)

## Recommendations

Nella parte superiore della pagina Rapporti potete trovare raccomandazioni basate su AI/ML in base ai vostri progressi. Controlla periodicamente per suggerimenti utili e approfondimenti!

![Immagine Sei](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-6.png)

## previsioni a livello di persona

Fare clic sulla scheda [!UICONTROL **Membri**] per visualizzare tutti i membri del programma. Passa il cursore del mouse sulle barre di probabilità di [!UICONTROL **registrazione**] o di [!UICONTROL **probabilità**] di partecipazione per visualizzare le percentuali e le categorie esatte. Potete quindi intervenire sui membri di una particolare categoria (ad esempio, tutti nella categoria &quot;Minori probabilità&quot; di registrare) e mirare specificatamente a incrementare i numeri di registrazione.

![Immagine sette](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-7.png)

>[!NOTE]
>
>La probabilità individuale tiene conto di più di 40 fattori di persona, tra cui gli attributi del profilo, l&#39;attività della persona e le attività pregresse invitate/registrate/frequentate.

## Domande frequenti

**D: Qual è il segmento?**

A: È probabile che la registrazione sia un valore compreso tra 0 e 100. Ogni utente membro del programma dell&#39;evento avrà un valore di probabilità compreso tra 0 e 100.

Inseriamo i valori di probabilità in tre segmenti:

* Probabilità di registrazione > 50% = segmento altamente probabile
* Probabilità di registrazione > 25% a &lt;50% = probabile segmento
* Probabilità di registrare &lt;25% = segmento meno probabile

Quando una persona ha la probabilità di registrarsi, la previsione cadrà in uno di questi segmenti (ogni persona che è membro di un programma rientrerà in uno di essi). Ad esempio, se un programma di eventi ha 1000 membri in base alle previsioni di probabilità, questi 1000 verranno distribuiti in segmenti _Altamente probabili_, _Probabili_ o _Meno probabili_ .

Pertanto, le persone che rientrano nel segmento Altamente probabile avranno maggiori possibilità di registrarsi all’evento.

Conversione in registro = numero di persone nel segmento registrato diviso per il numero di persone che rientrano nel segmento (ad esempio, se 100 persone rientrano nel segmento Molto probabile e 60 si registrano, il tasso di conversione è del 60%).

La percentuale di conversione da registrare seguirà il seguente pattern: Molto probabilmente > Probabile > Meno probabile.

**D: Come si utilizzano le informazioni?**

A: La best practice prevede quanto segue:

i. Potete creare un programma, e poi una Smart Campaign utilizza filtri predittivi con &quot;maggiore di X&quot;, che genererebbero una certa quantità di persone (ad esempio 1000) ed eseguireste la campagna.

ii) Dopo 24 ore, nella [!UICONTROL Reports] scheda è possibile visualizzare le registrazioni previste calcolate in base alla probabilità di registrare i valori di tutte le persone attualmente invitate.

iii) Se le registrazioni previste sono inferiori all&#39;obiettivo, dovrete invitare più persone. A questo punto, potete vedere le intuizioni che vi dicono quale fosse la soglia che funzionava nei programmi passati.

![Immagine otto](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-8.png)

IV. Puoi creare una nuova Smart Campaign con tale soglia per invitare più persone.

v. In qualsiasi momento, se si desidera comprendere il motivo per cui un numero proiettato viene visualizzato, è possibile visualizzare la distribuzione dell&#39;audience tra i segmenti, i relativi tassi di conversione dal passato e applicare tali tassi di conversione al pubblico corrente (vedere la videata di seguito).

**D: Qual è il grafico Segmenti per registrazione?**

A: Tre barre, ciascuna delle quali rappresenta un segmento (molto probabile, probabile, meno probabile).

**Linea punteggiata viola:** Tasso di conversazione medio per la registrazione in quel segmento, in base a programmi simili passati.

**Barra blu:** Percentuale di registrazione di tutte le persone in quel segmento.

![Image Nine](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-9.png)

Ad esempio, supponiamo che 100 persone abbiano probabilità di registrarsi > 50% e 60 di quelle 100 persone registrate. Molto probabilmente ha una conversione del 60%. Quindi, tutti i membri aggiunti al programma hanno probabilità di registrare valori, poi vengono inseriti nei segmenti e come per il numero di persone registrate in ogni tasso di conversione del segmento viene calcolato.

**D: Cosa significa &quot;Registrato e Superiore&quot;?**

A: Qualsiasi persona elencata come registrata o qualsiasi altro stato con un numero di passaggio uguale o superiore.

Potete creare nuovi stati di avanzamento per un programma di eventi, ma tali stati vengono mappati con stati standard. Considerare un caso in cui una persona viene spostata da invitata a promemoria, che è un passo più alto rispetto al registro. Questa persona sarà anche considerata come registrata e mostrata nel tracciamento dell&#39;obiettivo.

![Immagine dieci](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-10.png)

**D: Come vengono calcolate le registrazioni previste?**

A: Vedere di seguito.

![Image Eleven](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-11.png)
