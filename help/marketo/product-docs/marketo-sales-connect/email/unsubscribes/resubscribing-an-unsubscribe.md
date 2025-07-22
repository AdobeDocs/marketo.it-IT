---
unique-page-id: 14746177
description: Riscrizione e annullamento dell’abbonamento - Documentazione di Marketo - Documentazione del prodotto
title: Risottoscrizione e annullamento dell’abbonamento
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Risottoscrizione di un [!UICONTROL Unsubscribe] {#resubscribing-an-unsubscribe}

A volte le persone vogliono rinunciare alla ricezione di e-mail. Ecco come rendere nuovamente inviabili gli annullamenti dell’abbonamento.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!CAUTION]
>
>Prima di sottoscrivere nuovamente un abbonamento, devi essere in grado di dimostrare che l’autorizzazione per sottoscriverlo nuovamente è documentata e conforme a tutte le leggi applicabili.

>[!NOTE]
>
>Se la sincronizzazione per l&#39;annullamento dell&#39;abbonamento è attivata, è necessario rimuovere l&#39;annullamento dell&#39;abbonamento da ToutApp e deselezionare la rinuncia in [!DNL Salesforce] affinché il record della persona non venga sincronizzato di nuovo.

1. Vai all&#39;[applicazione Web](https://toutapp.com/login) e fai clic su **[!UICONTROL People]**.

1. Selezionare la persona per aprire la visualizzazione dettagli persona.

   ![](assets/two.png)

1. Fare clic sui tre punti nella visualizzazione Dettagli persona e selezionare **[!UICONTROL Remove Unsubscribe]**.

   ![](assets/three.png)

1. Selezionare il motivo per cui la persona ha rifiutato di ricevere le e-mail, quindi fare clic su **[!UICONTROL Remove Unsubscribe]**.

   ![](assets/four.png)

>[!NOTE]
>
>Se la sincronizzazione per l&#39;annullamento dell&#39;iscrizione è attivata, è necessario deselezionare anche la casella di rinuncia nel record di Salesforce. In caso contrario, la sincronizzazione notturna annullerà nuovamente l&#39;iscrizione della persona in [!DNL Sales Connect], in quanto rileverà che la persona ha rinunciato in [!DNL Salesforce]. Se uno dei record è stato escluso/annullato, la sincronizzazione contrassegnerà il record collegato come tale.
