---
description: Integrazione Dynamic Chat - Documentazione Marketo - Documentazione del prodotto
title: Integrazione Dynamic Chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 4%

---

# Integrazione Dynamic Chat {#dynamic-chat-integration}

Ulteriori informazioni sull&#39;integrazione di Dynamic Chat con Sales Insight.

>[!PREREQUISITES]
>
>* La versione del pacchetto Sales Insight SFDC deve essere [2.4.0 o successiva](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* È necessario configurare l&#39;[integrazione Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}
>
>* Assicurati che nel campo &quot;Chiave segreta API&quot; delle [impostazioni operative](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"} dell&#39;Insight di vendita sia popolato. In caso contrario, scopri come recuperarlo [qui](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}.

## Scheda Configurazione [!DNL Marketo Sales Insight] {#marketo-sales-insight-configuration-tab}

Per abilitare l&#39;integrazione di [!DNL Dynamic Chat], attenersi alla procedura riportata di seguito.

1. Accedi al tuo account [!DNL Salesforce], fai clic sul segno + alla fine della barra delle schede e fai clic su **[!DNL Marketo Sales Insight Config]**.

1. Fai clic su per scaricare &quot;[!UICONTROL Visualforce Panel]&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Selezionare la casella di controllo **[!UICONTROL Enable Dynamic Chat Data]**.

   ![](assets/dynamic-chat-integration-2.png)

## Panoramica delle funzioni {#feature-overview}

[!DNL Dynamic Chat] utenti possono sfruttare le seguenti [!DNL Sales Insight] attività...

Finestra di dialogo coinvolta: collegata a Marketo e popolata in [!DNL Sales Insight] quando un visitatore fa clic su un chatbot e interagisce con la finestra di dialogo.

* Nome Dialogo
* URL della pagina
* Stato (Avviato / Rilasciato / Completato)

Appuntamento pianificato: effettuato l&#39;accesso a Marketo e popolato in [!DNL Sales Insight] quando un visitatore pianifica correttamente un appuntamento tramite il chatbot.

* Nome Dialogo
* Agente
* URL della pagina
* Data e ora pianificate (inserire la data e l&#39;ora)
* Stato (Programmato, Riprogrammato, Annullato)

Obiettivo raggiunto: connesso a Marketo e popolato in [!DNL Sales Insight] quando un visitatore raggiunge un obiettivo in un flusso di dialogo.

* Nome Dialogo
* Nome obiettivo
* URL della pagina

Interazione con il documento: connesso a Marketo e popolato in [!DNL Sales Insight] quando un visitatore interagisce con un documento condiviso tramite il chatbot.

* Nome Dialogo
* Documento
* Stato

Le attività di chat sono disponibili in Dashboard approfondimenti.

![](assets/dynamic-chat-integration-3.png)

Nei pannelli Lead e Contatto è disponibile una scheda Chat. Include [!UICONTROL Activity Type], [!UICONTROL Dialogue Name] e [!UICONTROL Date] colonne.

![](assets/dynamic-chat-integration-4.png)

Per ulteriori informazioni su un tipo di attività, fai clic su di esso.

![](assets/dynamic-chat-integration-5.png)

Analogamente, i pannelli Account e Opportunità includono [!UICONTROL Name], [!UICONTROL Activity Type], [!UICONTROL Dialogue Name] e [!UICONTROL Date] colonne.

![](assets/dynamic-chat-integration-6.png)

La scheda Chat è inclusa anche nella scheda Global Marketo. Include tre tipi di attività ([!UICONTROL Engaged Dialogue], [!UICONTROL Scheduled Appointment], [!UICONTROL Reached Goal]) insieme alle colonne seguenti:

* [!UICONTROL Person]
* [!UICONTROL Account]
* [!UICONTROL Activity type] ([!UICONTROL Engaged Dialogue], [!UICONTROL Scheduled Appointment], [!UICONTROL Reached Goal])
* [!UICONTROL Dialogue Name]
* [!UICONTROL Date]

Di nuovo, puoi saperne di più su un tipo di attività facendo clic su di esso.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Se la casella di controllo &quot;[!UICONTROL Enable Dynamic Chat data]&quot; è disabilitata, le seguenti funzionalità verranno disabilitate:
>
>* Riga con le attività di chat nel dashboard Approfondimenti (visualizzazione griglia intelligente e elenco settimanale)
>* Scheda Chat nei pannelli Lead, Contatto, Account e Opportunità
>* Scheda Chat nella scheda Global Marketo
>
>Non è possibile disattivare solo una di queste funzioni.
