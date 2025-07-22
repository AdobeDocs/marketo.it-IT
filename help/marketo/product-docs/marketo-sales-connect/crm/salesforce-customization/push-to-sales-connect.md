---
unique-page-id: 14352477
description: Invia a  [!DNL Sales Connect] - Documentazione Marketo - Documentazione del prodotto
title: Invia a  [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 2%

---

# Invia a [!DNL Sales Connect] {#push-to-sales-connect}

Il pulsante [!UICONTROL Push to Tout] conterrà un elenco dei lead/contatti in [!DNL Salesforce] e li invierà a un gruppo in [!DNL Sales Connect]. Puoi quindi inviare rapidamente un’e-mail di gruppo personalizzabile con il tracciamento Tout allegato.

## Requisiti {#requirements}

* Pacchetto [!DNL Sales Connect Salesforce] installato dall&#39;amministratore [!DNL Salesforce]

* Pulsante [!UICONTROL Push to Sales Connect] installato nella visualizzazione elenco dall&#39;amministratore [!DNL Salesforce]

* Connessione [!DNL Salesforce] effettuata con [!DNL Sales Connect] per l&#39;utente che ha eseguito l&#39;invio

## Procedura {#how-to}

1. Fare clic sulla scheda **[!UICONTROL Lead/Contact]** in [!DNL Salesforce].
1. Passare alla visualizzazione elenco che si desidera inviare a [!DNL Sales Connect] accanto al pulsante [!UICONTROL Go].
1. Fai clic su **[!UICONTROL Go]**.
1. Seleziona tutti i lead/contatti che desideri inviare al tout.
1. Seleziona **[!UICONTROL Push to MSE]**.
1. Verrà visualizzata una nuova finestra che verifica il numero di lead/contatti che desideri trasferire. Seleziona **[!UICONTROL Proceed to Group]**.[!DNL Sales Connect] non eseguirà il push di alcun contatto contrassegnato come [!UICONTROL Email Opt Out] in [!DNL Salesforce] o [!UICONTROL Unsubscribed] in [!DNL Sales Connect].

   >[!NOTE]
   >
   >[!DNL Sales Connect] aggiungerà il gruppo denominato &quot;SFDC-...&quot; alla pagina Relazioni della [applicazione Web](https://toutapp.com/login).

1. Selezionare **[!UICONTROL Email Entire Group]** per inviare l&#39;e-mail del gruppo.
