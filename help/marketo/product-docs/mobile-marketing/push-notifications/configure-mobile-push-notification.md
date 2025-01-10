---
unique-page-id: 7512454
description: Configurare le notifiche push per dispositivi mobili - Documenti Marketo - Documentazione del prodotto
title: Configurare le notifiche push per dispositivi mobili
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: 736e21d45d8a62e50f449e0ee6d0fc4df5963dfb
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Configurare le notifiche push per dispositivi mobili {#configure-mobile-push-notification}

1. Vai all&#39;area **Attività di marketing**.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Seleziona la risorsa push e fai clic su **Modifica bozza**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Vai a **Configurazione**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Seleziona l’app desiderata. Le piattaforme Android e Apple sono abilitate per impostazione predefinita.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

1. Se il messaggio push si applica a una sola piattaforma (ad esempio, casi per iPhone), puoi escludere l’altra piattaforma facendo scorrere il relativo selettore su Disabilitato.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

1. Fai clic su **Avanti**.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Inserisci il testo del messaggio o seleziona l’icona del token per aggiungere token. Quindi, seleziona **Azione tocco**.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Se una piattaforma è abilitata, appare sul lato sinistro dello schermo del telefono. Quando è selezionato, viene visualizzato a colori.

   >[!NOTE]
   >
   >Esistono tre tipi di azioni di tocco:
   >
   >**Avvia app** - **Questa app** apre la home page dell&#39;app quando viene toccata la notifica. **Personalizzato** utilizza un collegamento profondo per aprire altre aree dell&#39;app o qualsiasi altra app a cui hai il collegamento (vedi [URI di collegamento profondo](#deep-link-uris) di seguito per i dettagli).
   >
   >**Pagina di destinazione** - consente di accedere a una pagina di destinazione di Marketo specificata.
   >
   >**External URL** - consente di accedere a una pagina di destinazione non Marketo.

1. Per inserire un collegamento profondo per un&#39;azione di tocco personalizzata, fare clic su Personalizzato e immettere l&#39;[URI collegamento profondo](#deep-link-uris) nel campo.

   ![](assets/image2016-7-28-16-3a19-3a13.png)

1. Per inserire i token, selezionali, immetti un valore predefinito e fai clic su Inserisci.

   >[!NOTE]
   >
   >I token vengono visualizzati nel punto in cui si posiziona il cursore nella casella di testo. Puoi utilizzare più di un token.

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >I messaggi e le azioni di tocco avranno lo stesso aspetto su entrambe le piattaforme.

1. Solo per iOS, seleziona la casella di controllo per indicare all’app di riprodurre un suono quando arriva il messaggio. Android riproduce automaticamente il suono.

   ![](assets/ios-tap-and-notification-hand.png)

1. Visualizzare l&#39;anteprima dell&#39;altra piattaforma e fare clic su **Fine**.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Fare clic su **Approva e chiudi**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

Congratulazioni! Ora la notifica push è pronta per essere inviata.

## URI di collegamenti profondi {#deep-link-uris}

Quando gli abbonati fanno clic su un pulsante in un messaggio push, possono accedervi direttamente alla home page dell’app o direttamente a una pagina specifica all’interno dell’app. Un collegamento profondo è un riferimento univoco a una pagina specifica dell’app e ha l’aspetto di un collegamento a un sito web.

Un URI di collegamento profondo è costituito da tre parti: nome dello schema, percorso e identificatore. Nell’esempio seguente, &quot;myappname&quot; è lo schema. &quot;products&quot; è il percorso, mentre &quot;purple-shirt&quot; è l’identificatore. Quando il cliente tocca, questi vengono portati specificamente all’elemento della camicia viola all’interno delle pagine dei prodotti della tua app.

![](assets/image2016-7-29-12-3a49-3a1.png)

Detto questo, la struttura dei collegamenti profondi dell&#39;app potrebbe essere diversa da quella dell&#39;esempio precedente. Il tuo sviluppatore dispone di molte opzioni per definire gli URI dei collegamenti profondi, pertanto chiedi allo sviluppatore di inviarti gli URI (collegamenti) per le pagine che ti interessano. In questo modo gli URI immessi nei messaggi push saranno posizionati correttamente. Il tuo sviluppatore può [trovare ulteriori informazioni qui](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/enabling-deep-links-in-your-app).

>[!MORELIKETHIS]
>
>[Invia una notifica push mobile](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
