---
unique-page-id: 7512454
description: Configurare le notifiche push per dispositivi mobili - Documenti Marketo - Documentazione del prodotto
title: Configurare le notifiche push per dispositivi mobili
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Configurare le notifiche push per dispositivi mobili {#configure-mobile-push-notification}

1. Vai a **Attività di marketing** area.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Seleziona la risorsa push e fai clic su **Modifica bozza**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Vai a **Configurazione**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Seleziona l’app desiderata. Le piattaforme Android e Apple sono abilitate per impostazione predefinita.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

1. Se il messaggio push si applica a una sola piattaforma (ad esempio, casi per iPhone), puoi escludere l’altra piattaforma facendo scorrere il relativo selettore su Disabilitato.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

1. Clic **Successivo**.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Inserisci il testo del messaggio o seleziona l’icona del token per aggiungere token. Quindi, seleziona una **Azione tocco**.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Se una piattaforma è abilitata, appare sul lato sinistro dello schermo del telefono. Quando è selezionato, viene visualizzato a colori.

   >[!NOTE]
   >
   >Esistono tre tipi di azioni di tocco:
   >
   >**Avvia app** - **Questa app** apre la home page dell’app quando viene toccata la notifica. **Personalizzato** utilizza un collegamento profondo per aprire altre aree dell’app o qualsiasi altra app a cui si ha il collegamento (vedi [URI di collegamenti profondi](#Deeplink) per i dettagli).
   >
   >**Pagina di destinazione** : consente di accedere a una pagina di destinazione di Marketo specifica.
   >
   >**URL esterno** : per passare a una pagina di destinazione non Marketo.

1. Per inserire un collegamento profondo per un’azione di tocco personalizzata, fai clic su Personalizzato e immetti il [URI collegamento profondo](#Deeplink) nel campo.

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

1. Visualizza l’anteprima dell’altra piattaforma e fai clic su **Fine**.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Clic **Approva e chiudi**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

Congratulazioni! Ora la notifica push è pronta per essere inviata.

## URI di collegamenti profondi {#deep-link-uris}

Quando gli abbonati fanno clic su un pulsante in un messaggio push, possono accedervi direttamente alla home page dell’app o direttamente a una pagina specifica all’interno dell’app. Un collegamento profondo è un riferimento univoco a una pagina specifica dell’app e ha l’aspetto di un collegamento a un sito web.

Un URI di collegamento profondo è costituito da tre parti: nome dello schema, percorso e identificatore. Nell’esempio seguente, &quot;myappname&quot; è lo schema. &quot;products&quot; è il percorso, mentre &quot;purple-shirt&quot; è l’identificatore. Quando il cliente tocca, vengono portati specificamente all’articolo della camicia viola all’interno delle pagine dei prodotti della tua app.

![](assets/image2016-7-29-12-3a49-3a1.png)

Detto questo, la struttura del collegamento profondo dell’app potrebbe essere diversa da quella dell’esempio precedente. Lo sviluppatore dispone di molte opzioni per la definizione degli URI di collegamento profondo. Chiedi allo sviluppatore di inviarti gli URI (collegamenti) per le pagine che ti interessano. In questo modo gli URI immessi nei messaggi push saranno posizionati correttamente. Lo sviluppatore può [ulteriori informazioni qui](https://developers.marketo.com/mobile/enabling-deep-links-in-your-app/).

>[!MORELIKETHIS]
>
>[Inviare una notifica push per dispositivi mobili](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
