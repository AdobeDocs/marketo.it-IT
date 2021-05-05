---
description: Come bloccare gli invii di moduli spam - Documenti Marketo - Documentazione del prodotto
title: Come bloccare gli invii di moduli spam
translation-type: tm+mt
source-git-commit: 35ab8d353a2518a1603cb508a6f8c0ea650483e4
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Come bloccare gli invii di moduli spam {#how-to-block-spam-form-submissions}

Spesso, l’invio di moduli con un checksum non valido o mancante (di solito dai bot) può produrre statistiche false. Ecco come prevenirlo.

>[!CAUTION]
>
>Questa funzione rifiuta l’invio di moduli effettuati tramite POST programmatici all’endpoint leadCapture/save2. Se l’azienda utilizza un’integrazione che invia i moduli a Marketo con tale metodo, l’attivazione di questa funzione bloccherà tali invii. L’utilizzo di leadCapture/save2 come API o l’esecuzione di invii di moduli programmatici direttamente ad essa non è supportato né vietato. Assicurati che la tua azienda invii solo i moduli utilizzando: Risorse del modulo, codice dei moduli incorporati, API Forms2.js o API REST del modulo di invio.

1. Fai clic su **Amministratore**.

   ![](assets/how-to-block-spam-form-submissions-1.png)

1. Fare clic su **Torta tesoro**.

   ![](assets/how-to-block-spam-form-submissions-2.png)

1. Accanto a **Cattura persona - Rifiuta valori di checksum non validi**, fare clic su **Modifica**.

   ![](assets/how-to-block-spam-form-submissions-3.png)

1. Seleziona la casella di controllo **Attivato** e fai clic su **Salva**.

   ![](assets/how-to-block-spam-form-submissions-4.png)

>[!NOTE]
>
>Quando si abilita questa funzione, è possibile che venga visualizzato un calo dell’attività del modulo quando i numeri falsi vengono filtrati.
