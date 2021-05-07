---
unique-page-id: 11378814
description: Elenchi avanzati account - Documenti Marketo - Documentazione del prodotto
title: Elenchi avanzati account
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
translation-type: tm+mt
source-git-commit: 35e86ac356e61e9d6b9a663e468ced1e9a947144
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Elenchi avanzati account {#account-smart-lists}

Ecco come identificare in modo rapido e preciso gli account di alto valore.

>[!NOTE]
>
>Questa funzione verrà abilitata per tutte le istanze Marketo qualificate la sera di martedì 11 maggio.

>[!NOTE]
>
>Questa funzione è disponibile solo per coloro che dispongono sia di TAM che dell’esperienza utente di Marketo Engage Adobe Next-Gen abilitata.

## Creare un elenco smart account {#create-an-account-smart-list}

1. In Marketo, vai a **Attività di marketing**.

   ![](assets/account-smart-lists-1.png)

1. Trova e seleziona il programma desiderato.

   ![](assets/account-smart-lists-2.png)

1. Fai clic sul menu a discesa **Nuovo** e seleziona **Nuova risorsa locale**.

   ![](assets/account-smart-lists-3.png)

1. Fai clic su **Elenco avanzato account**.

   ![](assets/account-smart-lists-4.png)

1. Immetti un nome e fai clic su **Crea** (la descrizione e le etichette sono facoltative).

   ![](assets/account-smart-lists-5.png)

Il tuo Account Smart List è stato creato. Vedi sotto per i passaggi per la definizione delle sue regole.

## Regole elenco avanzato account {#account-smart-list-rules}

Gli elenchi smart account funzionano in modo simile agli elenchi smart standard, con un&#39;eccezione notevole: contenitori.

1. Per definire l&#39;Elenco avanzato account, fai clic sulla scheda **Regole elenco avanzato account** .

   ![](assets/account-smart-lists-6.png)

1. Scegli i filtri account desiderati. In questo esempio scegliamo _Settore sanitario_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

1. Scegli i filtri persona corrispondenti. In questo esempio scegliamo _Stato è California_.

   ![](assets/account-smart-lists-9.png)

**Passaggio** facoltativo: Ecco dove entrano i contenitori. Se scegli un filtro persona aggiuntivo corrispondente, puoi rilasciarlo sotto il primo o _in_, creando un contenitore. In questo esempio stiamo creando un contenitore aggiungendo _Il titolo del lavoro è CFO_.

![](assets/account-smart-lists-10.png)

Ecco come apparirà il contenitore.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>La creazione di un contenitore di filtri crea una regola &quot;e&quot;, il che significa che restituisce solo tutti i risultati combinati. In questo esempio, account con un settore sanitario, insieme ad essere situato in California _e_ con qualcuno elencato come CFO. Se non desideri utilizzare i contenitori, rilascia semplicemente il filtro sotto o sopra quello esistente.

Ed è tutto! Consulta la sezione seguente per scoprire come sfruttare il tuo Account Smart List.

>[!TIP]
>
>Come per gli elenchi avanzati standard, puoi utilizzare la logica avanzata per perfezionare ulteriormente i risultati. Per farlo, sono necessari almeno tre filtri e in Elenchi avanzati account un contenitore (indipendentemente dal numero di filtri che contiene) è uguale a un filtro.

## Azioni elenco avanzato account {#account-smart-list-actions}

Nella scheda Panoramica dell’elenco avanzato account, noterai alcune opzioni di azione.

**Esportazione**: In questo modo i risultati dell’elenco avanzato account vengono esportati come CSV.

**Clona**: Crea una copia del tuo Account Smart List.

**Invia ad rete** pubblicitaria: Invia l’elenco a LinkedIn come nuovo pubblico con corrispondenza.

Puoi anche fare riferimento al tuo Account Smart List in una Smart Campaign/List standard utilizzando il filtro _Persone membro di Account Smart List_ .

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>I risultati del membro persone dell’elenco smart dell’account mostreranno ogni persona negli account identificati, non solo le persone che si trovano tramite filtri a persona abbinata nell’elenco smart dell’account.

>[!NOTE]
>
>**Definizione**
>
>**Persone membro dell’elenco** avanzato account: In questo caso la parola &quot;membro&quot; si riferisce all&#39;account stesso, quindi &quot;membro della gente&quot; significa la persona effettiva (record Marketo) in tali account.
