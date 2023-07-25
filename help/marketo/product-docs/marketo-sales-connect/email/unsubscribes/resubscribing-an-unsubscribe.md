---
unique-page-id: 14746177
description: Riscrizione e annullamento dell’abbonamento - Documentazione di Marketo - Documentazione del prodotto
title: Risottoscrizione e annullamento dell’abbonamento
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Risottoscrizione e annullamento dell’abbonamento {#resubscribing-an-unsubscribe}

A volte le persone vogliono rinunciare alla ricezione di e-mail. Ecco come rendere nuovamente inviabili gli annullamenti dell’abbonamento.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!CAUTION]
>
>Prima di sottoscrivere nuovamente un abbonamento, devi essere in grado di dimostrare che l’autorizzazione per sottoscriverlo nuovamente è documentata e conforme a tutte le leggi applicabili.

>[!NOTE]
>
>Se la sincronizzazione dell’annullamento dell’abbonamento è attivata, rimuovi l’annullamento dell’abbonamento da ToutApp e deseleziona la rinuncia in Salesforce affinché il record della persona non venga sincronizzato nuovamente.

1. Vai a [applicazione web](https://toutapp.com/login) e fai clic su **Persone**.

1. Selezionare la persona per aprire la visualizzazione dettagli persona.

   ![](assets/two.png)

1. Fai clic sui tre punti nella visualizzazione dettagli persona e seleziona **Rimuovi Annulla iscrizione**.

   ![](assets/three.png)

1. Seleziona il motivo per cui la persona ha rinunciato a ricevere e-mail, quindi fai clic su **Rimuovi Annulla iscrizione**.

   ![](assets/four.png)

>[!NOTE]
>
>Se la sincronizzazione per l’annullamento dell’iscrizione è attivata, devi deselezionare anche la casella di rinuncia nel record in Salesforce, altrimenti la sincronizzazione notturna annullerà nuovamente l’iscrizione della persona in Sales Connect, in quanto rileverà che la persona è stata esclusa in Salesforce. Se uno dei record è stato escluso/annullato, la sincronizzazione contrassegnerà il record collegato come tale.
