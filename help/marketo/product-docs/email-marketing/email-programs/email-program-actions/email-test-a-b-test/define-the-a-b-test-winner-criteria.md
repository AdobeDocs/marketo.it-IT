---
unique-page-id: 2359545
description: Definizione dei criteri vincitori del test A/B - Marketo Docs - Documentazione prodotto
title: Definire i criteri vincitori del test A/B
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# Definire i criteri vincitori test A/B {#define-the-a-b-test-winner-criteria}

Quando [aggiungete un test A/B](add-an-a-b-test.md) al programma e-mail, dovrete scegliere un tipo di test, [pianificare il test A/B](schedule-the-a-b-test.md), quindi definire i criteri vincenti. Ecco come decidere quale e-mail vince.

>[!PREREQUISITES]
>
>* [Aggiungere un test A/B](add-an-a-b-test.md)

>



## Criteri vincente {#winner-criteria}

1. Le opzioni predefinite **Criterio vincitore** sono elencate per prime.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   | **Apre** | Quando le immagini vengono scaricate in un messaggio e-mail, viene registrato un pulsante di apertura. Anche se non includete un&#39;immagine, per impostazione predefinita Marketo inserisce un singolo pixel di tracciamento in tutte le e-mail HTML. |
   |---|---|
   | **Clic** | Per impostazione predefinita, i collegamenti nelle e-mail presentano un tracciamento incorporato che consente di vedere chi ha fatto clic sul collegamento, quanti collegamenti totali è stato fatto clic su di esso, ecc. |
   | **Fare clic per aprire %** | Percentuale di e-mail che sono state aperte e per cui è stato fatto clic su un collegamento nel messaggio e-mail. Questo misura la rilevanza e il contesto di un’e-mail prendendo il numero di clic univoci diviso per il numero di aperture univoche, e poi moltiplicando per 100 per mostrarlo come percentuale. |
   | **Punteggio di coinvolgimento** | La [valutazione del coinvolgimento](http://docs.marketo.com/display/DOCS/Understanding+the+Engagement+Score) consente di determinare l&#39;efficacia dei contenuti. |

   >[!TIP]
   >
   >Se si sceglie il punteggio di coinvolgimento, il test dovrà essere eseguito per almeno 24 ore. Ulteriori informazioni su [come comprendere il punteggio relativo al coinvolgimento](../../../../../product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md).

   Potete inoltre personalizzare i criteri selezionando Conversione personalizzata e facendo clic su Modifica.
   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >Conversione personalizzata consente di scegliere qualsiasi evento come conversione utilizzando attivatori e filtri.

   Si aprirà una finestra. Individuate l’attivatore desiderato e trascinatelo nel quadro.
   ![](assets/image2014-9-12-15-3a52-3a18.png)

   >[!NOTE]
   >
   >**Tubo profondo**
   >
   >
   >Ulteriori informazioni sugli [elenchi smart ed elenchi statici](http://docs.marketo.com/display/docs/smart+lists+and+static+lists).

   Definire il trigger.
   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!NOTE]
   >
   >Marketo consentirà di attivare solo le attivazioni per le persone che hanno ricevuto l&#39;e-mail da questo programma e-mail. Non è necessario aggiungere un filtro &quot;È stato inviato un messaggio e-mail&quot;.

   Fate clic su Chiudi.
   ![](assets/image2014-9-12-15-3a53-3a36.png)

   Fantastico! Ora è il momento di decidere come si determina il vincitore.

## Dichiara vincitore {#declare-winner}

1. Scegliete una delle due opzioni disponibili.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >**Promemoria**
   >
   >
   >Se si esegue un test A/B **Data/Ora**, è possibile scegliere solo **Manuale**.

   Una volta terminato il test A/B, Marketo può inviare automaticamente l&#39;e-mail vincente all&#39;ora pianificata, oppure potete esaminare i risultati e decidere quale e-mail inviare.

1. Automatico è fantastico ed è l&#39;opzione predefinita. Fare clic su **Next**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Se si sceglie **Manual**, il test verrà inviato e si attende di dichiarare un vincitore. Riceverete un rapporto dei risultati.

   [programmare il test A/B](schedule-the-a-b-test.md)

Perfetto! Adesso andiamo.