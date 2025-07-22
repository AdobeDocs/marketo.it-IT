---
description: Inviare un elenco a un Ad Network - Documentazione di Marketo - Documentazione del prodotto
title: Inviare un elenco a una rete di annunci
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 1%

---

# Inviare un elenco a una rete di annunci {#send-a-list-to-an-ad-network}

Scopri come inviare un elenco statico a [!DNL LinkedIn], [!DNL Facebook] o Google.

## Come inviare un elenco {#how-to-send-a-list}

1. In Marketo, selezionare l&#39;elenco, fare clic sul menu a discesa **[!UICONTROL List Actions]** e selezionare **[!UICONTROL Send to Ad Network]**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Scegli tra [!DNL LinkedIn], [!DNL Facebook] o Google (le altre opzioni non sono al momento disponibili). In questo esempio, stiamo scegliendo **[!DNL LinkedIn]**. Fai clic su **[!UICONTROL Next]**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Fai clic sul menu a discesa **[!UICONTROL Audience]** e seleziona il pubblico desiderato.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Se hai bisogno di controllare, puoi vedere il pubblico di destinazione in cui viene sincronizzato un elenco tramite la scheda Stato.

1. Scegliere il [!UICONTROL Push Type] desiderato e fare clic su **[!UICONTROL Update]**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Se selezioni &quot;[!UICONTROL Enable continuous audience sync]&quot;, Marketo mantiene l&#39;elenco aggiornato nella rete di annunci scelta mentre l&#39;elenco cambia nell&#39;istanza di Marketo. Aggiungiamo entrambi **e** persone rimosse dal pubblico se vengono aggiunte o rimosse dall&#39;elenco statico.

1. Ed è tutto! Fare clic su **[!UICONTROL OK]** per uscire.

   ![](assets/send-a-list-to-an-ad-network-5.png)

## Domande frequenti {#faq}

**È possibile sincronizzare un singolo elenco statico con più tipi di pubblico di annunci?**

No, un elenco può essere sincronizzato solo con un singolo pubblico di destinazione.

**Se si abilita la sincronizzazione continua con un pubblico di annunci esistente, verrà sostituito il pubblico esistente?**

No, il pubblico esistente verrà aggiunto a, non sostituito.
