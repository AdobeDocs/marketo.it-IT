---
unique-page-id: 9437340
description: Implementazione di RTP tramite Tealium Tag Manager - Marketo Docs - Documentazione prodotto
title: Implementazione di RTP tramite Tealium Tag Manager
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Implementazione di RTP tramite Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Per implementare il tag RTP, segui le istruzioni di installazione riportate di seguito.

1. Accedi al tuo account Tealium Tag Manager.
1. Passate alla scheda Tag e aggiungete il tag del contenitore personalizzato Tealium, situato nella scheda Varie del marketplace Tag.
1. Nel campo Titolo, immettete **Marketo RTP** e fate clic su **Fine**.
1. Salvare le modifiche.

   >[!NOTE]
   >
   >Non è ancora necessario pubblicare il nuovo contenitore.

1. Dopo aver salvato il profilo, fate clic sul vostro nome/indirizzo e-mail nell’angolo in alto a destra della console iQ di Tealium.
1. Nel menu Admin, fate clic su **Gestisci modelli** in Amministrazione account.
1. Selezionate Contenitore personalizzato **Tealium: Per aprire il modello di tag, selezionate RTP** dall’elenco a discesa.
1. Accedi al tuo account RTP.
1. Vai a Impostazioni account.

   >[!NOTE]
   >
   >Se avete già ricevuto il tag JavaScript dal supporto tecnico, continuate con il passaggio 11.

1. In Dominio, individua il dominio appropriato e fai clic su **Genera tag**.
1. Copiate il tag JavaScript RTP e incollatelo tra Start Tag Library Code e End Tag Library Code nel modello di profilo del Tealium.

   >[!NOTE]
   >
   >**Passaggi importanti**
   >
   >Rimuovete i `<!-- RTP tag -->` tag e `<!-- End of RTP tag -->` dal codice inserito in questo file.
   >
   >Rimuovete eventuali `<script type='text/javascript'>` tag e `</script>` tag dal codice inserito in questo file.

1. **Fate clic su Salva modello** profilo e pubblicate il nuovo profilo.

