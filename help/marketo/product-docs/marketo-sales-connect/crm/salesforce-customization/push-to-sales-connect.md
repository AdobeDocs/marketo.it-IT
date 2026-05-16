---
unique-page-id: 14352477
description: Scopri come utilizzare il pulsante Push to Sales Connect in Salesforce. Aggiungere lead o contatti da Salesforce a Sales Connect con un clic.
title: Invia a  [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/piy3bPtiO48FQhWEmpu5qo4denlJ8v1ZU-VXBlWh0Mg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 166
ht-degree: 1%

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
   >[!DNL Sales Connect] aggiungerà questo gruppo denominato &quot;SFDC-...&quot; nella pagina Relazioni dell&#39;[applicazione Web](https://toutapp.com/login).

1. Selezionare **[!UICONTROL Email Entire Group]** per inviare l&#39;e-mail del gruppo.
