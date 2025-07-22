---
unique-page-id: 10617431
description: Impostare Il Pubblico Dei Messaggi In-App - Documentazione Di Marketo - Documentazione Del Prodotto
title: Impostare Il Pubblico Dei Messaggi In-App
exl-id: 696ae5b6-7063-41bc-bcef-27879182ff1e
feature: Mobile Marketing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 1%

---

# Impostare Il Pubblico Dei Messaggi In-App {#set-your-in-app-message-audience}

Il primo passaggio consiste nel decidere chi deve ricevere il messaggio in-app. Devi impostare l’elenco avanzato.

1. Fai clic su **[!UICONTROL Edit Smart List]**.

   ![](assets/image2016-5-9-15-3a15-3a7.png)

1. Nell&#39;elenco avanzato, il trigger **[!UICONTROL Has Mobile App Activity]** viene popolato automaticamente. Fai clic sul menu a discesa e seleziona l’app in cui desideri inserire il messaggio.

   ![](assets/image2016-5-9-15-3a18-3a10.png)

   >[!NOTE]
   >
   >Al momento, più valori per il campo App mobile non sono supportati per i programmi di messaggistica in-app.

1. **[!UICONTROL App Open]** è l&#39;impostazione predefinita di Action, ma è possibile selezionare qualsiasi evento personalizzato già configurato.

   ![](assets/image2016-5-9-15-3a20-3a23.png)

   >[!NOTE]
   >
   >Il trigger predefinito ([!UICONTROL App Open]) ed eventuali trigger personalizzati aggiunti al codice dallo sviluppatore vengono visualizzati automaticamente nel selettore [!UICONTROL Action]. Se manca un evento personalizzato, contatta lo sviluppatore per assicurarti che abbia aggiunto gli eventi personalizzati all&#39;app. Tieni presente che il completamento della codifica e dell’approvazione degli eventi personalizzati potrebbe richiedere un po’ di tempo. Per ulteriori informazioni, consulta [questo articolo](/help/marketo/product-docs/mobile-marketing/admin/before-you-create-push-notifications-and-in-app-messages.md).

1. Se necessario, sono disponibili vincoli per il trigger **[!UICONTROL Has Mobile App Activity]**.

   ![](assets/image2016-5-9-15-3a22-3a27.png)

1. Puoi aggiungere filtri all’elenco avanzato per limitare chi riceve il messaggio in-app. In questo esempio, utilizzando il filtro **[!UICONTROL Acquisition Date]**, solo le persone acquisite il 9 giugno 2016 riceveranno il messaggio in-app.

   ![](assets/image2016-5-9-15-3a26-3a2.png)

1. Torna al Pannello di controllo Campaign di messaggi in-app. Imposta il limite di visualizzazione nel menu a discesa.

   ![](assets/image2016-5-9-15-3a30-3a35.png)

   >[!NOTE]
   >
   >Il limite di visualizzazione predefinito è **[!UICONTROL Once per session]**. Se si desidera interrompere la visualizzazione del messaggio dopo la risposta del destinatario, selezionare **[!UICONTROL Every time until tapped]**. Se deve essere visualizzato ogni volta, indipendentemente dalle operazioni del destinatario, scegli **[!UICONTROL Every time]**.

   ![](assets/image2016-5-9-15-3a32-3a6.png)

Ottimo lavoro. Il pubblico è pronto. Hai ottenuto la barra blu e il segno di spunta verde.

È ora di [selezionare il messaggio in-app](/help/marketo/product-docs/mobile-marketing/in-app-messages/sending-your-in-app-message/select-your-in-app-message.md).
