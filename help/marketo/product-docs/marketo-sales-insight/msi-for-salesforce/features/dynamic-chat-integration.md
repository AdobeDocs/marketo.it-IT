---
description: Integrazione dei Dynamic Chat - Documentazione Marketo - Documentazione del prodotto
title: Integrazione Dynamic Chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 6e81a8891f7d6e5916549d453a694b42e08cd496
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 5%

---

# Integrazione Dynamic Chat {#dynamic-chat-integration}

Ulteriori informazioni sull’integrazione del Dynamic Chat con Sales Insight.

>[!PREREQUISITES]
>
>* La versione del pacchetto SFDC Sales Insight deve essere [2.4.0 o successiva](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* È necessario configurare l&#39;[integrazione di Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}
>
>* Assicurati che nel tuo approfondimento sulle vendite [Impostazioni operative](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"} sia compilato il campo &quot;Chiave segreta API&quot;. In caso contrario, scopri come recuperarlo [qui](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}.

## Scheda Configurazione di Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

Per abilitare l’integrazione del Dynamic Chat, segui i passaggi indicati di seguito.

1. Accedi al tuo account Salesforce, fai clic sul segno + alla fine della barra delle schede e fai clic su **Configurazione di Marketo Sales Insight**.

1. Fate clic su per aprire il pannello &quot;Visualforce&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Selezionare la casella di controllo **Abilita dati Dynamic Chat**.

   ![](assets/dynamic-chat-integration-2.png)

## Panoramica delle funzioni {#feature-overview}

Gli utenti di Sales Insight possono sfruttare le seguenti attività di Dynamic Chat...

Dialogo coinvolto: effettuato l’accesso a Marketo e popolato in Sales Insight quando un visitatore fa clic su un chatbot e si impegna con il dialogo.

* Nome Dialogo
* URL pagina
* Stato (Avviato / Rilasciato / Completato)

Appuntamento pianificato: effettuato l’accesso a Marketo e popolato in Sales Insight quando un visitatore pianifica correttamente un appuntamento tramite il chatbot.

* Nome Dialogo
* Agente
* URL pagina
* Data e ora pianificate (inserire la data e l&#39;ora)
* Stato (Programmato, Riprogrammato, Annullato)

Obiettivo raggiunto: effettuato l’accesso a Marketo e popolato in Sales Insight quando un visitatore raggiunge un obiettivo in un flusso di dialogo.

* Nome Dialogo
* Nome obiettivo
* URL pagina

Interazione con il documento: effettuato l’accesso a Marketo e popolato in Sales Insight quando un visitatore interagisce con un documento condiviso tramite il chatbot.

* Nome Dialogo
* Documento
* Stato

Le attività di chat sono disponibili in Dashboard approfondimenti.

![](assets/dynamic-chat-integration-3.png)

Nei pannelli Lead e Contatto è disponibile una scheda Chat. Include le colonne Tipo di attività, Nome finestra di dialogo e Data.

![](assets/dynamic-chat-integration-4.png)

Per ulteriori informazioni su un tipo di attività, fai clic su di esso.

![](assets/dynamic-chat-integration-5.png)

Analogamente, i pannelli Account e Opportunità includono le colonne Nome, Tipo di attività, Nome finestra di dialogo e Data.

![](assets/dynamic-chat-integration-6.png)

La scheda Chat è inclusa anche nella scheda Global Marketo. Include tre tipi di attività (Dialogo coinvolto, Appuntamento pianificato, Obiettivo raggiunto), insieme alle colonne seguenti:

* Persona
* Account
* Tipo di attività (finestra di dialogo Coinvolto, appuntamento pianificato, obiettivo raggiunto)
* Nome Dialogo
* Data e ora

Di nuovo, puoi saperne di più su un tipo di attività facendo clic su di esso.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Se la casella di controllo &quot;Abilita dati di Dynamic Chat&quot; è disabilitata, le seguenti funzioni verranno disabilitate:
>
>* Riga con le attività di chat nel dashboard Approfondimenti (visualizzazione griglia intelligente e elenco settimanale)
>* Scheda Chat nei pannelli Lead, Contatto, Account e Opportunità
>* Scheda Chat nella scheda Global Marketo
>
>Non è possibile disattivare solo una di queste funzioni.

