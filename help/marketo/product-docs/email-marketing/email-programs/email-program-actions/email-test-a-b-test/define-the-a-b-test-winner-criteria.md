---
unique-page-id: 2359545
description: Definire i criteri per i vincitori dei test A/B - Documentazione di Marketo - Documentazione del prodotto
title: Definire i criteri vincitori del test A/B
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
feature: Email Programs, A/B Testing
source-git-commit: c80d25aeafe2314fcff1d99359ff146c88acad06
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 21%

---

# Definire i criteri vincitori del test A/B {#define-the-a-b-test-winner-criteria}

Quando [aggiungi un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"} al tuo programma e-mail, dovrai scegliere un tipo di test, [pianificare il test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}, quindi definire i criteri dei vincitori. Ecco come decidere quale e-mail vince.

>[!PREREQUISITES]
>
>[Aggiungi un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}

## Criteri vincitori {#winner-criteria}

1. Le opzioni **[!UICONTROL Winner Criteria]** predefinite sono elencate per prime.

   ![](assets/define-the-a-b-test-winner-criteria-1.png)

   <table>
   <tr>
   <td><b>[!UICONTROL Opens]</b></td>
   <td>Un messaggio aperto si registra quando le immagini vengono scaricate in un messaggio e-mail. Anche se non includi un’immagine, per impostazione predefinita Marketo inserisce un singolo pixel di tracciamento in tutte le e-mail di HTML.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Clicks]</b></td>
   <td>Per impostazione predefinita, i link nelle e-mail incorporano il tracciamento che consente di vedere chi ha fatto clic su un link, su quanti link totali è stato fatto clic e così via.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Click to Open] %</b></td>
   <td>Percentuale di e-mail aperte su cui è stato fatto clic su un collegamento nell’e-mail. Misura la rilevanza e il contesto di un’e-mail in base al numero di clic univoci diviso per il numero di aperture univoche, quindi moltiplicandolo per 100 per visualizzarlo come percentuale.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Engagement Score]</b></td>
   <td>Il <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">punteggio di coinvolgimento</a> consente di determinare l'efficacia del contenuto.</td>
   </tr>
   </table>

   >[!TIP]
   >
   >Se scegli il punteggio di coinvolgimento, il test dovrà essere eseguito per almeno 24 ore. Ulteriori informazioni su [comprendere il punteggio di coinvolgimento](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}.

1. È inoltre possibile personalizzare i criteri selezionando **[!UICONTROL Custom Conversion]** e facendo clic su **[!UICONTROL Edit]**.

   ![](assets/define-the-a-b-test-winner-criteria-2.png)

   >[!NOTE]
   >
   >Conversione personalizzata consente di scegliere qualsiasi evento come conversione utilizzando trigger e filtri.

1. Viene visualizzata una finestra. Trova il trigger desiderato e trascinalo nell’area di lavoro.

   ![](assets/define-the-a-b-test-winner-criteria-3.png)

1. Definisci il trigger.

   ![](assets/define-the-a-b-test-winner-criteria-4.png)

   >[!IMPORTANT]
   >
   >Marketo consente trigger/filtri solo per le persone a cui è stata inviata l’e-mail da questo programma e-mail, quindi non è necessario aggiungere un filtro &quot;E-mail inviata&quot;. Inoltre, quando utilizzi un trigger/filtro relativo alle e-mail, assicurati di utilizzare &quot;è qualsiasi&quot; come operatore.

1. Chiudere la nuova finestra (o scheda) aperta. L’elenco avanzato viene salvato automaticamente.

Ora è il momento di decidere come viene determinato il vincitore.

## Dichiara vincitore {#declare-winner}

1. Scegliete una delle due opzioni disponibili.

   ![](assets/define-the-a-b-test-winner-criteria-5.png)

   >[!NOTE]
   >
   >Se esegui un test A/B di **Data/ora**, puoi scegliere solo **[!UICONTROL Manual]**.

   Al termine del test A/B, Marketo può inviare automaticamente l’e-mail vincente all’orario pianificato, oppure puoi rivedere i risultati e decidere quale e-mail viene inviata quando.

1. Automatico è fantastico ed è l&#39;opzione predefinita. Fai clic su **[!UICONTROL Next]**.

   ![](assets/define-the-a-b-test-winner-criteria-6.png)

   >[!TIP]
   >
   >Scegliendo **[!UICONTROL Manual]** verrà inviato il test e si attenderà la dichiarazione di un vincitore. Riceverai un rapporto sui risultati.

Ora [pianifica il test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}.
