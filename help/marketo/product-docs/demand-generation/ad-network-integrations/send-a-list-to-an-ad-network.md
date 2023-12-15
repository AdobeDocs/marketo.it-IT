---
description: Inviare un elenco a un Ad Network - Documentazione di Marketo - Documentazione del prodotto
title: Inviare un elenco a una rete di annunci
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Inviare un elenco a una rete di annunci {#send-a-list-to-an-ad-network}

Scopri come inviare un elenco statico a LinkedIn, Facebook o Google.

## Come inviare un elenco {#how-to-send-a-list}

1. In Marketo Engage, seleziona l’elenco, fai clic su **[!UICONTROL Azioni elenco]** e selezionare **[!UICONTROL Invia ad Ad Network]**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Scegli tra LinkedIn, Facebook o Google (le altre opzioni non sono al momento disponibili). In questo esempio, stiamo scegliendo **[!UICONTROL LinkedIn]**. Clic **[!UICONTROL Successivo]**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Fai clic su **[!UICONTROL Pubblico]** e selezionare il pubblico desiderato.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Se hai bisogno di controllare, puoi vedere il pubblico di destinazione in cui viene sincronizzato un elenco tramite la scheda Stato.

1. Scegli il tipo di push desiderato e fai clic su **[!UICONTROL Aggiorna]**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Se selezioni &quot;Abilita sincronizzazione continua del pubblico&quot;, Marketo mantiene l’elenco aggiornato nella rete di annunci selezionata quando l’elenco cambia nell’istanza di Marketo. Aggiungiamo entrambi _e_ rimuovi le persone dal pubblico se vengono aggiunte o rimosse dall’elenco statico.

1. Ed è tutto! Clic **[!UICONTROL OK]** per uscire.

   ![](assets/send-a-list-to-an-ad-network-5.png)

## Domande frequenti {#faq}

**È possibile sincronizzare un singolo elenco statico con più tipi di pubblico di annunci?**

No, un elenco può essere sincronizzato solo con un singolo pubblico di destinazione.

**Se si abilita la sincronizzazione continua con un pubblico di annunci esistente, questo verrà sostituito?**

No, il pubblico esistente verrà aggiunto a, non sostituito.
