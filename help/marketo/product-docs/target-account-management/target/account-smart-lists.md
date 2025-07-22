---
unique-page-id: 11378814
description: Elenchi avanzati account - Documentazione Marketo - Documentazione del prodotto
title: Elenchi avanzati account
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Elenchi avanzati account {#account-smart-lists}

Ecco come identificare in modo rapido e accurato i tuoi account di alto valore.

>[!NOTE]
>
>Questa funzionalità è disponibile solo per coloro che dispongono sia del componente aggiuntivo [!UICONTROL Target Account Management] che di una licenza TAM rilasciata.

## Crea un [!UICONTROL Account Smart List] {#create-an-account-smart-list}

1. In Marketo, vai a **[!UICONTROL Marketing Activities]**.

   ![](assets/account-smart-lists-1.png)

1. Individuare e selezionare il programma desiderato.

   ![](assets/account-smart-lists-2.png)

1. Fare clic sul menu a discesa **[!UICONTROL New]** e selezionare **[!UICONTROL New Local Asset]**.

   ![](assets/account-smart-lists-3.png)

1. Fai clic su **[!UICONTROL Account Smart List]**.

   ![](assets/account-smart-lists-4.png)

1. Immettere un nome e fare clic su **[!UICONTROL Create]** (Descrizione ed etichette sono facoltativi).

   ![](assets/account-smart-lists-5.png)

[!UICONTROL Account Smart List] è stato creato Consulta di seguito per i passaggi per definirne le regole.

## [!UICONTROL Account Smart List] regole {#account-smart-list-rules}

[!UICONTROL Account Smart Lists] funziona in modo simile agli elenchi avanzati standard, con un&#39;eccezione degna di nota: i contenitori.

1. Per definire [!UICONTROL Account Smart List], fare clic sulla scheda **[!UICONTROL Account Smart List Rules]**.

   ![](assets/account-smart-lists-6.png)

1. Scegli i filtri account desiderati. In questo esempio _[!UICONTROL Industry]è[!UICONTROL Healthcare]_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >I dati dell&#39;indicatore ICP utilizzati nella [Classifica di profilatura account e ottimizzazione](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) verranno visualizzati come attributi dell&#39;account personalizzati da utilizzare nell&#39;elenco avanzato account. Questi dati attributo personalizzati si basano su quando è stato creato/aggiornato il modello di profilo account.

1. Scegli i filtri persona corrispondenti. In questo esempio si sta scegliendo _State come California_.

   ![](assets/account-smart-lists-9.png)

**PASSAGGIO FACOLTATIVO**: è qui che entrano i contenitori. Se scegli un filtro persona corrispondente aggiuntivo, puoi rilasciarlo sotto il primo o _in_ creando un contenitore. In questo esempio stiamo creando un contenitore aggiungendo _Il titolo del processo è CFO_.

![](assets/account-smart-lists-10.png)

Ecco come apparirà il contenitore.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>La creazione di un contenitore di filtri crea una regola &quot;e&quot;, che restituisce solo tutti i risultati combinati. In questo esempio, gli account con un settore sanitario, oltre a trovarsi in California _e_ con qualcuno elencato come CFO. Se non desideri utilizzare i contenitori, rilascia semplicemente il filtro al di sotto/al di sopra di quello esistente.

Ed è tutto! Consulta la sezione seguente per scoprire come utilizzare [!UICONTROL Account Smart List].

>[!TIP]
>
>Proprio come con gli elenchi avanzati standard, puoi utilizzare la logica avanzata per perfezionare ulteriormente i risultati. Sono necessari almeno tre filtri e in [!UICONTROL Account Smart Lists] un contenitore (indipendentemente dal numero di filtri contenuti) è uguale a un filtro.

## [!UICONTROL Account Smart List] azioni {#account-smart-list-actions}

Nella scheda Panoramica di [!UICONTROL Account Smart List], noterai alcune opzioni di azione.

**[!UICONTROL Export]**: esporta i risultati di [!UICONTROL Account Smart List] come CSV.

**[!UICONTROL Clone]**: crea una copia di [!UICONTROL Account Smart List].

**[!UICONTROL Send to Ad Network]**: invia l&#39;elenco a [!DNL LinkedIn] come nuovo pubblico corrispondente.

È inoltre possibile fare riferimento a [!UICONTROL Account Smart List] in un elenco/campagna Smart standard utilizzando il filtro _[!UICONTROL People Member of Account Smart List]_.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>I risultati di [!UICONTROL People Member of Account Smart List] mostreranno tutte le persone negli account identificati, non solo le persone trovate tramite i filtri Persona corrispondente nell&#39;elenco avanzato degli account.

>[!NOTE]
>
>**Definizione**
>
>**[!UICONTROL People Member of Account Smart List]**: in questo caso la parola &quot;membro&quot; fa riferimento all&#39;account stesso, quindi &quot;membro persone&quot; significa le persone effettive (record Marketo) in tali account.
