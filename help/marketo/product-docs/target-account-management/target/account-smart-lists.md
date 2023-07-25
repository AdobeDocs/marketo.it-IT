---
unique-page-id: 11378814
description: Elenchi avanzati account - Documentazione Marketo - Documentazione del prodotto
title: Elenchi avanzati account
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
feature: Target Account Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Elenchi avanzati account {#account-smart-lists}

Ecco come identificare in modo rapido e accurato i tuoi account di alto valore.

>[!NOTE]
>
>Questa funzione è disponibile solo per coloro che dispongono sia del componente aggiuntivo Gestione account di Target che di una licenza TAM rilasciata.

## Creare un elenco avanzato dell’account {#create-an-account-smart-list}

1. In Marketo, vai a **Attività di marketing**.

   ![](assets/account-smart-lists-1.png)

1. Individuare e selezionare il programma desiderato.

   ![](assets/account-smart-lists-2.png)

1. Fai clic su **Nuovo** a discesa e selezionare **Nuova risorsa locale**.

   ![](assets/account-smart-lists-3.png)

1. Clic **Elenco avanzato account**.

   ![](assets/account-smart-lists-4.png)

1. Immetti un nome e fai clic su **Crea** (Descrizione ed etichette sono facoltative).

   ![](assets/account-smart-lists-5.png)

L&#39;elenco avanzato account è stato creato. Consulta di seguito per i passaggi per definirne le regole.

## Regole per elenchi avanzati account {#account-smart-list-rules}

Gli elenchi avanzati account funzionano in modo simile agli elenchi avanzati standard, con una notevole eccezione: i contenitori.

1. Per definire l’elenco avanzato degli account, fai clic su **Regole per elenchi avanzati account** scheda.

   ![](assets/account-smart-lists-6.png)

1. Scegli i filtri account desiderati. In questo esempio stiamo scegliendo _Il settore è quello sanitario_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >dati degli indicatori ICP utilizzati nel [Classificazione e tuning profilo account](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) verranno visualizzati come attributi dell’account personalizzati da utilizzare nell’elenco avanzato degli account. Questi dati attributo personalizzati si basano su quando è stato creato/aggiornato il modello di profilo account.

1. Scegli i filtri persona corrispondenti. In questo esempio stiamo scegliendo _Lo stato è la California_.

   ![](assets/account-smart-lists-9.png)

**PASSAGGIO FACOLTATIVO**: Ecco dove entrano i contenitori. Se scegli un filtro persona corrispondente aggiuntivo, puoi rilasciarlo sotto il primo, oppure _in_ creando un contenitore. In questo esempio stiamo creando un contenitore aggiungendo _La qualifica è CFO_.

![](assets/account-smart-lists-10.png)

Ecco come apparirà il contenitore.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>La creazione di un contenitore di filtri crea una regola &quot;e&quot;, che restituisce solo tutti i risultati combinati. In questo esempio, gli account con un settore sanitario, oltre a trovarsi in California _e_ con qualcuno elencato come direttore finanziario. Se non desideri utilizzare i contenitori, rilascia semplicemente il filtro al di sotto/al di sopra di quello esistente.

Ed è tutto! Consulta la sezione seguente per scoprire come sfruttare il tuo elenco avanzato degli account.

>[!TIP]
>
>Proprio come con gli elenchi avanzati standard, puoi utilizzare la logica avanzata per perfezionare ulteriormente i risultati. A tale scopo, sono necessari almeno tre filtri e, negli elenchi avanzati account, un contenitore (indipendentemente dal numero di filtri contenuti) equivale a un filtro.

## Azioni per elenchi avanzati account {#account-smart-list-actions}

Nella scheda Panoramica dell’elenco avanzato account, noterai alcune opzioni di azione.

**Esporta**: esporta i risultati dell’elenco avanzato dell’account come file CSV.

**Clona**: crea una copia dell’elenco avanzato dell’account.

**Invia ad Ad Network**: invia l’elenco a LinkedIn come nuovo pubblico corrispondente.

Puoi anche fare riferimento all’elenco avanzato dell’account in un elenco/campagna avanzato standard utilizzando _Persone Membro dell’elenco avanzato account_ filtro.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>I risultati dell’elenco avanzato Persone membro dell’account mostreranno tutte le persone negli account identificati, non solo le persone che si trovano tramite i filtri Persona corrispondente nell’elenco avanzato degli account.

>[!NOTE]
>
>**Definizione**
>
>**Persone Membro dell’elenco avanzato account**: in questo caso la parola &quot;membro&quot; fa riferimento all’account stesso, quindi &quot;membro persona&quot; indica le persone effettive (record Marketo) in tali account.
