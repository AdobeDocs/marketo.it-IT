---
unique-page-id: 9437340
description: Implementazione di RTP con Tealium Tag Manager - Documentazione di Marketo - Documentazione del prodotto
title: Implementazione di RTP con Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Implementazione di RTP con Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Per implementare il tag RTP, seguire le istruzioni di installazione riportate di seguito.

1. Accedi al tuo account Tealium Tag Manager.

1. Passa alla scheda Tag e aggiungi il tag contenitore personalizzato Tealium, che si trova nella scheda Varie del marketplace Tag.

1. Nel campo Titolo, immetti **Marketo RTP** e fai clic su **Fine**.

1. Salva le modifiche.

   >[!NOTE]
   >
   >Non è ancora necessario pubblicare il nuovo contenitore.

1. Dopo aver salvato il profilo, fai clic sul tuo nome/indirizzo e-mail nell’angolo superiore destro della console Tealium iQ.

1. Scegliere **Gestisci modelli** dal menu Amministrazione in Amministrazione account.

1. Selezionare **Contenitore personalizzato Tealium: Marketo RTP** dall&#39;elenco a discesa per aprire il modello di tag.

1. Accedi al tuo account RTP.

1. Vai a Impostazioni account.

   >[!NOTE]
   >
   >Se hai già ricevuto il tuo tag JavaScript dal Supporto, continua con il passaggio 11.

1. In Dominio individuare il dominio pertinente e fare clic su **Genera tag**.

1. Copiare il tag JavaScript RTP e incollarlo tra Start Tag Library Code e End Tag Library Code nel modello di profilo Tealium.

   >[!NOTE]
   >
   >**Passaggi importanti**
   >
   >Rimuovere i tag `<!-- RTP tag -->` e `<!-- End of RTP tag -->` dal codice inserito nel file.
   >
   >Rimuovere i tag `<script type='text/javascript'>` e `</script>` dal codice inserito nel file.

1. **Fai clic su Salva modello profilo** e pubblica il nuovo profilo.
