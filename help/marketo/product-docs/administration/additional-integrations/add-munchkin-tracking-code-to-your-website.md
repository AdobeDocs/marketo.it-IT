---
unique-page-id: 2360354
description: Aggiungi  [!DNL Munchkin] Codice di tracciamento al tuo sito Web - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungi  [!DNL Munchkin] Codice di tracciamento al tuo sito Web
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
feature: Administration, Munchkin Tracking Code
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 1%

---

# Aggiungi il codice di tracciamento [!DNL Munchkin] al tuo sito Web {#add-munchkin-tracking-code-to-your-website}

Il codice di tracciamento JavaScript personalizzato di Marketo, denominato [!DNL Munchkin], tiene traccia di tutti gli utenti che visitano il tuo sito Web in modo che tu possa reagire alle loro visite con campagne di marketing automatizzate. Anche i visitatori anonimi vengono tracciati insieme ai loro indirizzi IP e altre informazioni. **Senza questo codice di tracciamento, non potrai tenere traccia di visite o altre attività sul tuo sito Web**.

>[!PREREQUISITES]
>
>Assicurati di avere accesso a uno sviluppatore JavaScript esperto. Il supporto tecnico Marketo non è configurato per fornire assistenza nella risoluzione dei problemi relativi al JavaScript personalizzato.

## Aggiungi codice di tracciamento al tuo sito web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Gli utenti di Adobe Experience Cloud possono inoltre utilizzare l&#39;integrazione di [Marketo in Adobe Launch](https://exchange.adobe.com/apps/ec/100223/adobe-launch-core-extension){target="_blank"} per includere lo script [!DNL Munchkin] nelle proprie pagine Web. Se si utilizza Adobe Launch, _lo script [!DNL Munchkin] viene aggiunto automaticamente_, pertanto non è necessario aggiungerlo manualmente.

1. Passare all&#39;area **[!UICONTROL Admin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. Fai clic su **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. Selezionare **[!UICONTROL Asynchronous]** per **[!UICONTROL Tracking Code Type]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-3.png)

   >[!NOTE]
   >
   >Nella maggior parte dei casi, devi utilizzare il codice asincrono. [Ulteriori informazioni](#types-of-munchkin-tracking-codes).

1. Fai clic su e copia il codice di tracciamento JavaScript da inserire sul sito web.

   ![](assets/add-munchkin-tracking-code-to-your-website-4.png)

   >[!CAUTION]
   >
   >Non utilizzare il codice mostrato in questa schermata: devi utilizzare il codice univoco visualizzato nel tuo account!

   >[!TIP]
   >
   >Inserisci il codice di tracciamento nelle pagine web che desideri tracciare. Può trattarsi di tutte le pagine per i siti più piccoli o solo di pagine chiave per i siti con molte pagine Web generate dinamicamente, forum utente e così via.

   Per ottenere risultati ottimali, utilizzare il codice [!DNL Munchkin] asincrono e inserirlo negli elementi `<head>` delle pagine. Se utilizzi il codice semplice (scelta non consigliata), si trova immediatamente prima del tag `</body>`.

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >Per i siti che registrano un elevato volume di traffico (ad esempio centinaia di migliaia di visite al mese), ti consigliamo di scegliere di non tenere traccia delle persone anonime. [Ulteriori informazioni](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking){target="_blank"}.

## Aggiungi Codice Di Tracciamento Quando Si Utilizzano Più Aree Di Lavoro {#add-tracking-code-when-using-multiple-workspaces}

Se utilizzi le aree di lavoro nell’account Marketo, probabilmente avrai anche presentazioni web separate che corrispondono alle aree di lavoro. In tal caso, è possibile utilizzare JavaScript di monitoraggio [!DNL Munchkin] per assegnare le persone anonime all&#39;area di lavoro e alla partizione corrette.

1. Passare all&#39;area **[!UICONTROL Admin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. Fai clic su **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. Seleziona l’area di lavoro appropriata per le pagine web da monitorare.

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >Se non si utilizza il codice speciale dell&#39;area di lavoro [!DNL Munchkin], le persone verranno assegnate alla partizione predefinita creata al momento della configurazione dell&#39;account. Si chiama inizialmente &quot;[!UICONTROL Default]&quot;, ma potresti averlo modificato nel tuo account Marketo.

1. Selezionare **[!UICONTROL Asynchronous]** per **[!UICONTROL Tracking Code Type]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. Fai clic su e copia il codice di tracciamento JavaScript da inserire sul sito web.

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >Non utilizzare il codice mostrato in questa schermata: devi utilizzare il codice univoco visualizzato nel tuo account!

1. Inserire il codice di tracciamento nelle pagine Web nell&#39;elemento `<head>`. Le nuove persone che visitano questa pagina verranno assegnate a questa partizione.

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >È possibile utilizzare un solo script di tracciamento [!DNL Munchkin] per una singola partizione e area di lavoro in una pagina. Non includere script di tracciamento per più partizioni/aree di lavoro nel sito Web.

   >[!NOTE]
   >
   >Le pagine di destinazione create in Marketo contengono automaticamente un codice di tracciamento, pertanto non è necessario inserirlo.

## Tipi di codici di tracciamento [!DNL Munchkin] {#types-of-munchkin-tracking-codes}

È possibile scegliere tra tre tipi di codici di tracciamento [!DNL Munchkin]. Ciascuno influisce sui tempi di caricamento della pagina web in modo diverso.

1. **[!UICONTROL Simple]**: ha il minor numero di righe di codice, ma non è ottimizzato per il tempo di caricamento della pagina Web. Questo codice carica la libreria jQuery ogni volta che viene caricata una pagina Web.
1. **[!UICONTROL Asynchronous]**: riduce il tempo di caricamento della pagina Web.
1. **[!UICONTROL Asynchronous jQuery]**: riduce il tempo di caricamento della pagina Web e migliora le prestazioni del sistema. Questo codice presuppone che tu disponga già di jQuery e non controlla di caricarlo.

## Verifica se il codice [!DNL Munchkin] funziona {#test-if-your-munchkin-code-is-working}

Per verificare che il codice [!DNL Munchkin] funzioni dopo averlo aggiunto:

1. Visita la tua pagina web.

1. In [!DNL My Marketo], fare clic sul riquadro **[!UICONTROL Analytics]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. Fai clic su **[!UICONTROL Web Page Activity]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. Fare clic sulla scheda **[!UICONTROL Setup]**, quindi fare doppio clic su **[!UICONTROL Activity Source]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. Modificare [!UICONTROL Activity Source] in **[!UICONTROL Anonymous Visitors (including ISPs)]** e fare clic su **[!UICONTROL Apply]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. Fare clic sulla scheda **[!UICONTROL Report]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >Se non trovi dati, attendi alcuni minuti e fai clic sull&#39;icona [!UICONTROL refresh] in basso.
