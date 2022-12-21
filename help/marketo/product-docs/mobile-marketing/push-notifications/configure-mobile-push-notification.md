---
unique-page-id: 7512454
description: Configurare le notifiche push per dispositivi mobili - Documenti Marketo - Documentazione del prodotto
title: Configurare le notifiche push mobili
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Configurare le notifiche push mobili {#configure-mobile-push-notification}

1. Vai a **Attività di marketing** area.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Seleziona la risorsa push e fai clic su **Modifica bozza**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Vai a **Configurazione**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Seleziona l’app desiderata. Le piattaforme Android e Apple sono abilitate per impostazione predefinita.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

1. Se il messaggio push si applica a una sola piattaforma (ad esempio, casi per iPhone), puoi escludere l’altra piattaforma spostando il relativo selettore su Disabilitato.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

1. Fai clic su **Successivo**.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Immetti il testo del messaggio o seleziona l’icona del token per aggiungere token. Quindi, seleziona una **Tocca azione**.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Se una piattaforma è abilitata, viene visualizzata sul lato sinistro della schermata del telefono. Viene visualizzato a colori quando è selezionato.

   >[!NOTE]
   >
   >Sono disponibili tre tipi di azioni di tocco:
   >
   >**Avvia app** - **Questa app** apre la home page dell’app quando viene toccata la notifica. **Personalizzato** utilizza un collegamento profondo per aprire altre aree dell&#39;app o qualsiasi altra app a cui hai collegato (vedi [URI di collegamento profondo](#Deeplink) qui sotto per i dettagli).
   >
   >**Pagina di destinazione** - consente di passare a una pagina di destinazione specifica di Marketo.
   >
   >**External URL** - consente di passare a una pagina di destinazione non Marketo.

1. Per inserire un collegamento profondo per un’azione di tocco personalizzata, fai clic su Personalizzato e immetti [URI collegamento profondo](#Deeplink) nel campo .

   ![](assets/image2016-7-28-16-3a19-3a13.png)

1. Per inserire i token, selezionare un token, immettere un valore predefinito e fare clic su Inserisci.

   >[!NOTE]
   >
   >I token vengono visualizzati nella posizione in cui si posiziona il cursore nella casella di testo. Puoi utilizzare più di un token.

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >I messaggi e le azioni touch avranno lo stesso aspetto su entrambe le piattaforme.

1. Solo per iOS, seleziona la casella di controllo per indicare all’app di riprodurre un suono all’arrivo del messaggio. Android riproduce il suono automaticamente.

   ![](assets/ios-tap-and-notification-hand.png)

1. Visualizza l’anteprima dell’altra piattaforma e fai clic su **Fine**.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Fai clic su **Approva e chiudi**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

Complimenti. Ora la notifica push è pronta per essere inviata.

## URI di collegamento profondo {#deep-link-uris}

Quando gli abbonati fanno clic su un pulsante in un messaggio push, possono essere portati alla home page dell’app o direttamente a una pagina specifica all’interno dell’app. Un collegamento profondo è un riferimento univoco a una pagina specifica dell&#39;app e assomiglia molto a un collegamento a un sito web.

Un URI di collegamento profondo è costituito da tre parti: nome, percorso e identificatore dello schema. Nell’esempio seguente, &quot;myappname&quot; è lo schema. &quot;products&quot; è il percorso, mentre &quot;viola-shirt&quot; è l’identificatore. Quando il cliente effettua un tocco, viene portato specificatamente all’elemento camicia viola all’interno delle pagine dei prodotti dell’app.

![](assets/image2016-7-29-12-3a49-3a1.png)

Detto questo, la struttura dei collegamenti profondi dell’app può essere diversa dall’esempio precedente. Lo sviluppatore dispone di molte opzioni per definire gli URI dei collegamenti profondi, quindi chiedi allo sviluppatore di inviarti gli URI (collegamenti) per le pagine che ti interessano. In questo modo gli URI immessi nei messaggi push verranno posizionati nei punti giusti. Lo sviluppatore può [trova ulteriori informazioni qui](https://developers.marketo.com/mobile/enabling-deep-links-in-your-app/).

>[!MORELIKETHIS]
>
>[Inviare una notifica push mobile](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
