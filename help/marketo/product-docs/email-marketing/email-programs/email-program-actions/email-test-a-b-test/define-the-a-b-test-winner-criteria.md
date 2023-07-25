---
unique-page-id: 2359545
description: Definire i criteri per i vincitori dei test A/B - Documentazione di Marketo - Documentazione del prodotto
title: Definire i criteri vincitori del test A/B
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Definire i criteri vincitori del test A/B {#define-the-a-b-test-winner-criteria}

Quando [aggiunta di un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"} to your email program, you will need to pick a test type, [schedule the A/B test](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}, quindi definisci i criteri del vincitore. Ecco come decidere quale e-mail vince.

>[!PREREQUISITES]
>
>[Aggiungere un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}

## Criteri vincitori {#winner-criteria}

1. Il valore predefinito **Criteri vincitori** Le opzioni sono elencate per prime.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>Aperture</b></td>
   <td>Un messaggio aperto si registra quando le immagini vengono scaricate in un messaggio e-mail. Anche se non includi un’immagine, per impostazione predefinita Marketo inserisce un singolo pixel di tracciamento in tutte le e-mail HTML.</td>
   </tr>
   <tr>
   <td><b>Clic</b></td>
   <td>Per impostazione predefinita, i collegamenti nelle e-mail incorporano il tracciamento che consente di vedere chi ha fatto clic su quale collegamento, quanti collegamenti totali hanno fatto clic su di esso e così via.</td>
   </tr>
   <tr>
   <td><b>Fare clic per aprire %</b></td>
   <td>Percentuale di e-mail aperte su cui è stato fatto clic su un collegamento nell’e-mail. Misura la rilevanza e il contesto di un’e-mail in base al numero di clic univoci diviso per il numero di aperture univoche, quindi moltiplicandolo per 100 per visualizzarlo come percentuale.</td>
   </tr>
   <tr>
   <td><b>Punteggio di coinvolgimento</b></td>
   <td>Il <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">punteggio di coinvolgimento</a> consente di determinare l’efficacia dei contenuti.</td>
   </tr>
   </table>

   >[!TIP]
   >
   >Se scegli il punteggio di coinvolgimento, il test dovrà essere eseguito per almeno 24 ore. Ulteriori informazioni su [comprensione del punteggio di coinvolgimento](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}.

1. Puoi anche personalizzare i criteri selezionando Conversione personalizzata e facendo clic su Modifica.

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >Conversione personalizzata consente di scegliere qualsiasi evento come conversione utilizzando trigger e filtri.

1. Viene visualizzata una finestra. Trova il trigger desiderato e trascinalo nell’area di lavoro.

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. Definisci il trigger.

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!IMPORTANT]
   >
   >Marketo consente trigger/filtri solo per le persone a cui è stata inviata l’e-mail da questo programma e-mail, quindi non è necessario aggiungere un filtro &quot;E-mail inviata&quot;. Inoltre, quando utilizzi un trigger/filtro relativo alle e-mail, assicurati di utilizzare &quot;è qualsiasi&quot; come operatore.

1. Fai clic su **Chiudi**.

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   Fantastico! Ora è il momento di decidere come viene determinato il vincitore.

## Dichiara vincitore {#declare-winner}

1. Scegliete una delle due opzioni disponibili.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >Se si sta eseguendo una **Data/ora** Test A/B, puoi solo scegliere **Manuale**.

   Al termine del test A/B, Marketo può inviare automaticamente l’e-mail vincente all’orario pianificato, oppure puoi rivedere i risultati e decidere quale e-mail viene inviata quando.

1. Automatico è fantastico ed è l&#39;opzione predefinita. Fai clic su **Successivo**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Scelta **Manuale** invierà il test e vi aspetterà per dichiarare un vincitore. Riceverai un rapporto sui risultati.

Perfetto! Ora andiamo [pianificare il test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}.
