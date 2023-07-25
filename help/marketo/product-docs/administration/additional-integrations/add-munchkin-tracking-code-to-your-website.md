---
unique-page-id: 2360354
description: "Aggiungi [!DNL Munchkin] Codice di tracciamento per il tuo sito web - Documentazione di Marketo - Documentazione del prodotto"
title: "Aggiungi [!DNL Munchkin] Codice di tracciamento per il tuo sito web"
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
feature: Administration, Munchkin Tracking Code
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Aggiungi [!DNL Munchkin] Codice di tracciamento per il sito web {#add-munchkin-tracking-code-to-your-website}

Codice di tracciamento JavaScript personalizzato di Marketo, denominato [!DNL Munchkin], tiene traccia di tutti i singoli utenti che visitano il tuo sito web in modo che tu possa reagire alle loro visite con campagne di marketing automatizzate. Anche i visitatori anonimi vengono tracciati insieme ai loro indirizzi IP e altre informazioni. **Senza questo codice di tracciamento, non potrai tenere traccia di visite o altre attività sul tuo sito web**!

>[!PREREQUISITES]
>
>Assicurati di avere accesso a uno sviluppatore JavaScript esperto. Il supporto tecnico Marketo non è configurato per assistere nella risoluzione dei problemi di JavaScript personalizzato.

## Aggiungi codice di tracciamento al tuo sito web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>I clienti Adobe Experience Cloud possono inoltre utilizzare l’integrazione di Marketo in Adobe Launch per includere [!DNL Munchkin] nelle loro pagine web. Scarica l’app [qui](https://www.adobeexchange.com/experiencecloud.details.101054.html){target="_blank"}.

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. Clic **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. Seleziona **[!UICONTROL Asincrono]** per **[!UICONTROL Tipo di codice di tracciamento]**.

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

   Per ottenere risultati ottimali, utilizzare la [!DNL Munchkin] e inseriscilo all&#39;interno del `<head>` elementi delle pagine. Se utilizzi il codice semplice (scelta non consigliata), questo viene visualizzato immediatamente prima del `</body>` tag.

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >Per i siti che registrano un elevato volume di traffico (ad esempio centinaia di migliaia di visite al mese), ti consigliamo di scegliere di non tenere traccia delle persone anonime. [Ulteriori informazioni](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/).

## Aggiungi Codice Di Tracciamento Quando Si Utilizzano Più Aree Di Lavoro {#add-tracking-code-when-using-multiple-workspaces}

Se utilizzi le aree di lavoro nell’account Marketo, probabilmente avrai anche presentazioni web separate che corrispondono alle aree di lavoro. In tal caso, puoi utilizzare [!DNL Munchkin] tracciamento di JavaScript per assegnare persone anonime all&#39;area di lavoro e alla partizione corrette.

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. Clic **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. Seleziona l’area di lavoro appropriata per le pagine web da monitorare.

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >Se non utilizzi l’area di lavoro speciale [!DNL Munchkin] , gli utenti verranno assegnati alla partizione predefinita creata al momento della configurazione dell&#39;account. Si chiama &quot;.[!UICONTROL Predefinito]&quot; inizialmente, ma potresti averlo modificato nel tuo account Marketo.

1. Seleziona **[!UICONTROL Asincrono]** per **[!UICONTROL Tipo di codice di tracciamento]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. Fai clic su e copia il codice di tracciamento JavaScript da inserire sul sito web.

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >Non utilizzare il codice mostrato in questa schermata: devi utilizzare il codice univoco visualizzato nel tuo account!

1. Inserisci il codice di tracciamento nelle pagine web di `<head>` elemento. Le nuove persone che visitano questa pagina verranno assegnate a questa partizione.

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >Puoi utilizzarne solo uno [!DNL Munchkin] script di tracciamento per una singola partizione e area di lavoro in una pagina. Non includere script di tracciamento per più partizioni/aree di lavoro nel sito Web.

   >[!NOTE]
   >
   >Le pagine di destinazione create in Marketo contengono automaticamente un codice di tracciamento, pertanto non è necessario inserirlo.

## Tipi di [!DNL Munchkin] Codici di tracciamento {#types-of-munchkin-tracking-codes}

Esistono tre tipi di [!DNL Munchkin] codici di tracciamento selezionabili. Ciascuno influisce sui tempi di caricamento della pagina web in modo diverso.

1. **[!UICONTROL Semplice]**: ha il minor numero di righe di codice, ma non ottimizza il tempo di caricamento della pagina web. Questo codice carica la libreria jQuery ogni volta che viene caricata una pagina Web.
1. **[!UICONTROL Asincrono]**: riduce il tempo di caricamento della pagina web.
1. **[!UICONTROL jQuery asincrona]**: riduce il tempo di caricamento delle pagine web e migliora le prestazioni del sistema. Questo codice presuppone che tu disponga già di jQuery e non controlla di caricarlo.

## Verifica se [!DNL Munchkin] Il codice funziona {#test-if-your-munchkin-code-is-working}

Per verificare che [!DNL Munchkin] il codice funziona dopo averlo aggiunto:

1. Visita la tua pagina web.

1. Nel tuo [!DNL My Marketo], fare clic su **[!UICONTROL Analytics]** affiancare.

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. Clic **[!UICONTROL Attività pagina web]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. Fai clic su **[!UICONTROL Configurazione]** , fare doppio clic **[!UICONTROL Origine attività]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. Modificare il [!UICONTROL Origine attività] a **[!UICONTROL Visitatori anonimi (inclusi ISP)]** e fai clic su **[!UICONTROL Applica]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. Fai clic su **[!UICONTROL Report]** scheda.

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >Se non trovi dati, attendi alcuni minuti, quindi fai clic sull’icona di aggiornamento in basso.
