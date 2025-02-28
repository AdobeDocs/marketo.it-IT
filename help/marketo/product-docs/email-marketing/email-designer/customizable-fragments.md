---
solution: Marketo Engage
product: marketo
title: Frammenti personalizzabili
description: Scopri come personalizzare i frammenti rendendo modificabili alcuni dei loro campi.
feature: Email Editor
role: User
level: Beginner, Intermediate
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
source-git-commit: 2a01045abbc23bce9531c64e3494fb12a9adf1bd
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Frammenti personalizzabili {#customizable-fragments}

I frammenti utilizzati in un’e-mail o in un modello e-mail sono bloccati per impostazione predefinita a causa dell’ereditarietà. Ciò significa che eventuali modifiche apportate a un frammento vengono propagate automaticamente a tutte le risorse in cui viene utilizzato il frammento. Con i frammenti personalizzabili, campi specifici all’interno di un frammento possono essere definiti come modificabili quando il frammento viene aggiunto a un’e-mail o a un modello e-mail. Supponiamo ad esempio di avere un frammento con un banner, del testo e un pulsante. È possibile designare come modificabili alcuni campi, ad esempio l’URL di destinazione dell’immagine o del pulsante. Questo consente agli utenti di modificare questi elementi quando incorporano il frammento nel modello e-mail/e-mail, offrendo un’esperienza personalizzata senza influire sul frammento originale.

Sfruttando frammenti personalizzabili, puoi gestire e personalizzare in modo efficiente i contenuti senza creare blocchi di contenuto completamente nuovi o interrompere l’ereditarietà dal frammento originale. In questo modo, le modifiche apportate a livello di frammento vengono comunque propagate, consentendo al contempo la necessaria personalizzazione a livello di e-mail/modello e-mail.

I frammenti visivi e di espressione possono essere contrassegnati come personalizzabili. Per istruzioni dettagliate su come procedere con ciascun tipo di frammento, consulta le sezioni seguenti.

## Aggiungere campi modificabili nei frammenti visivi {#visual}

Per rendere modificabili parti di un frammento visivo, effettua le seguenti operazioni:

>[!NOTE]
>
>I campi modificabili possono essere aggiunti ai componenti **image**, **text** e **button**. Per i componenti di **HTML**, i campi modificabili vengono aggiunti utilizzando l&#39;editor di personalizzazione, in modo simile ai frammenti di espressione. [Scopri come aggiungere un campo modificabile nei componenti e nei frammenti di espressione di HTML](#expression)

1. Apri la schermata di modifica del contenuto del frammento.

1. Seleziona il componente nel frammento in cui desideri configurare i campi modificabili.

1. Il riquadro delle proprietà del componente viene visualizzato sul lato destro. Seleziona la scheda **[!UICONTROL Campi modificabili]**, quindi attiva l&#39;opzione **[!UICONTROL Abilita edizione]**.

1. Tutti i campi che possono essere modificati per il componente selezionato sono elencati nel riquadro. I campi disponibili per la modifica dipendono dal tipo di componente selezionato.

   Nell’esempio seguente, è consentita la modifica dell’URL del pulsante &quot;Fai clic qui&quot;.

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. Fai clic su **[!UICONTROL Panoramica]** per controllare tutti i campi modificabili e i relativi valori predefiniti.

   In questo esempio, il campo URL del pulsante viene visualizzato con il valore predefinito definito nel componente. Questo valore sarà personalizzabile dagli utenti dopo che avranno aggiunto il frammento al loro contenuto.

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. Al termine, salva le modifiche.

Dopo aver aggiunto il frammento in un messaggio e-mail, gli utenti potranno personalizzare tutti i campi modificabili configurati nel frammento.

## Aggiungere campi modificabili nei componenti HTML e nei frammenti di espressione {#expression}

Per rendere modificabili parti di un componente HTML o di un frammento di espressione, è necessario utilizzare una sintassi specifica nell’editor espressioni. Ciò comporta la dichiarazione di una _variabile_ con un valore predefinito che gli utenti possono ignorare dopo aver aggiunto il frammento al loro contenuto.

Ad esempio, supponi di voler creare un frammento da aggiungere alle e-mail e di consentire agli utenti di personalizzare un colore specifico utilizzato in posizioni diverse, ad esempio cornici o colori di sfondo dei pulsanti. Durante la creazione del frammento, devi dichiarare una variabile con un _ID univoco_ (ad esempio, &quot;colore&quot;) e chiamarla nelle posizioni desiderate nel contenuto del frammento in cui desideri applicare questo colore. Quando aggiungono il frammento al contenuto, gli utenti possono personalizzare il colore utilizzato ovunque venga fatto riferimento alla variabile.

Per i componenti HTML, solo elementi specifici possono diventare campi modificabili. Per ulteriori informazioni, espandi la sezione seguente.

+++Elementi modificabili nei componenti di HTML:

Gli elementi riportati di seguito possono diventare campi modificabili in un componente HTML:

* Parte di testo
* Un URL completo per collegamento o immagine (non funziona con parte di un URL)
* Intera proprietà CSS (non funziona con la proprietà parziale)

Ad esempio, nel codice seguente, ogni elemento evidenziato in rosso può diventare una proprietà:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++

>[!MORELIKETHIS]
>
>[Frammenti](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
