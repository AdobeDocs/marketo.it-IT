---
description: Inviare un elenco a un Ad Network - Documentazione di Marketo - Documentazione del prodotto
title: Inviare un elenco a una rete di annunci
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Inviare un elenco a una rete di annunci {#send-a-list-to-an-ad-network}

Scopri come inviare un elenco statico a LinkedIn, Facebook o Google.

## Come inviare un elenco {#how-to-send-a-list}

1. In Marketo, seleziona l’elenco, fai clic su **Azioni elenco** e selezionare **Invia ad Ad Network**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Scegli tra LinkedIn, Facebook o Google (le altre opzioni non sono al momento disponibili). In questo esempio, stiamo scegliendo **LinkedIn**. Clic **Successivo**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Fai clic sul menu a discesa Pubblico e seleziona il pubblico desiderato.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Se hai bisogno di controllare, puoi vedere il pubblico di destinazione in cui viene sincronizzato un elenco tramite la scheda Stato.

1. Scegli il tipo di push desiderato e fai clic su **Aggiorna**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Se selezioni &quot;Abilita sincronizzazione continua del pubblico&quot;, Marketo mantiene l’elenco aggiornato nella rete di annunci selezionata quando l’elenco cambia nell’istanza di Marketo. Aggiungiamo entrambi **e** rimuovi le persone dal pubblico se vengono aggiunte o rimosse dall’elenco statico.

1. Ed è tutto! Clic **OK** per uscire.

   ![](assets/send-a-list-to-an-ad-network-5.png)

## Domande frequenti {#faq}

**È possibile sincronizzare un singolo elenco statico con più tipi di pubblico di annunci?**

No, un elenco può essere sincronizzato solo con un singolo pubblico di destinazione.

**Se si abilita la sincronizzazione continua con un pubblico di annunci esistente, questo verrà sostituito?**

No, il pubblico esistente verrà aggiunto a, non sostituito.
