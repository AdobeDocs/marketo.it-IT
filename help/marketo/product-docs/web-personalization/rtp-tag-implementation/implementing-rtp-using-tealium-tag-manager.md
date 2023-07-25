---
unique-page-id: 9437340
description: Implementazione di RTP con Tealium Tag Manager - Documentazione di Marketo - Documentazione del prodotto
title: Implementazione di RTP con Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Implementazione di RTP con Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Per implementare il tag RTP, seguire le istruzioni di installazione riportate di seguito.

1. Accedi al tuo account Tealium Tag Manager.

1. Passa alla scheda Tag e aggiungi il tag contenitore personalizzato Tealium, che si trova nella scheda Varie del marketplace Tag.

1. Nel campo Titolo, immetti **MARKETO RTP** e fai clic su **Fine**.

1. Salva le modifiche.

   >[!NOTE]
   >
   >Non è ancora necessario pubblicare il nuovo contenitore.

1. Dopo aver salvato il profilo, fai clic sul tuo nome/indirizzo e-mail nell’angolo superiore destro della console Tealium iQ.

1. Scegliere Amministratore dal menu **Gestisci modelli** in Amministratore account.

1. Seleziona **Contenitore personalizzato Tealium: Marketo RTP** dall’elenco a discesa per aprire il modello di tag.

1. Accedi al tuo account RTP.

1. Vai a Impostazioni account.

   >[!NOTE]
   >
   >Se hai già ricevuto il tag JavaScript dal Supporto, continua con il passaggio 11.

1. In Dominio, individua il dominio pertinente e fai clic su **Genera tag**.

1. Copia il tag JavaScript RTP e incollalo tra Start Tag Library Code e End Tag Library Code nel modello di profilo Tealium.

   >[!NOTE]
   >
   >**Passaggi importanti**
   >
   >Rimuovi il `<!-- RTP tag -->` e `<!-- End of RTP tag -->` dal codice inserito in questo file.
   >
   >Rimuovi qualsiasi `<script type='text/javascript'>` e `</script>` dal codice inserito in questo file.

1. **Fai clic su Salva modello profilo** e pubblica il nuovo profilo.
