---
unique-page-id: 9437340
description: Implementazione di RTP tramite Tealium Tag Manager - Marketo Docs - Documentazione prodotto
title: Implementazione di RTP tramite Tealium Tag Manager
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Implementazione di RTP tramite Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Per implementare il tag RTP, segui le istruzioni di installazione riportate di seguito.

1. Accedi al tuo account Tealium Tag Manager.

1. Passate alla scheda Tag e aggiungete il tag del contenitore personalizzato Tealium, situato nella scheda Varie del marketplace Tag.

1. Nel campo Titolo, immettere **Marketo RTP** e fare clic su **Fine**.

1. Salvare le modifiche.

   >[!NOTE]
   >
   >Non è ancora necessario pubblicare il nuovo contenitore.

1. Dopo aver salvato il profilo, fate clic sul vostro nome/indirizzo e-mail nell’angolo in alto a destra della console iQ di Tealium.

1. Nel menu Admin, fate clic su **Gestisci modelli** in Amministrazione account.

1. Selezionare **Contenitore personalizzato Tealium: Dall’elenco a discesa Marketo RTP** per aprire il modello di tag.

1. Accedi al tuo account RTP.

1. Vai a Impostazioni account.

   >[!NOTE]
   >
   >Se avete già ricevuto il tag JavaScript dal supporto tecnico, continuate con il passaggio 11.

1. In Domain (Dominio), individua il dominio appropriato e fai clic su **Generate Tag**.

1. Copiate il tag JavaScript RTP e incollatelo tra Start Tag Library Code e End Tag Library Code nel modello di profilo del Tealium.

   >[!NOTE]
   >
   >**Passaggi importanti**
   >
   >Rimuovere i tag `<!-- RTP tag -->` e `<!-- End of RTP tag -->` dal codice inserito in questo file.
   >
   >Rimuovete eventuali tag `<script type='text/javascript'>` e `</script>` dal codice inserito in questo file.

1. **Fate clic su Salva** modello profilo e pubblicate il nuovo profilo.
