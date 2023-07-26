---
description: Integrazione dei Dynamic Chat - Documentazione Marketo - Documentazione del prodotto
title: Integrazione Dynamic Chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 02f3150cda31ec25fc47fc7f6ea50feaa9fed6b5
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 5%

---

# Integrazione Dynamic Chat {#dynamic-chat-integration}

Ulteriori informazioni sull’integrazione del Dynamic Chat con Sales Insight.

>[!PREREQUISITES]
>
>* La versione del pacchetto SFDC Sales Insight deve essere [1.9 o superiore](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* È necessario disporre di [Integrazione del Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} configurazione

## Scheda Configurazione di Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

Per abilitare l’integrazione del Dynamic Chat, segui i passaggi indicati di seguito.

1. Accedi al tuo account Salesforce, fai clic sul segno + alla fine della barra delle schede e fai clic su **Configurazione approfondimento vendite Marketo**.

1. Fate clic su per aprire il pannello &quot;Visualforce&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Seleziona la **Abilita dati Dynamic Chat** casella di controllo.

   ![](assets/dynamic-chat-integration-2.png)

## Panoramica delle funzioni {#feature-overview}

Gli utenti di Sales Insight possono sfruttare le seguenti attività di Dynamic Chat...

Dialogo coinvolto: effettuato l’accesso a Marketo e popolato in Sales Insight quando un visitatore fa clic su un chatbot e si impegna con il dialogo.

* Nome dialogo
* URL pagina
* Stato (Avviato / Rilasciato / Completato)

Appuntamento pianificato: effettuato l’accesso a Marketo e popolato in Sales Insight quando un visitatore pianifica correttamente un appuntamento tramite il chatbot.

* Nome dialogo
* Agente
* URL pagina
* Data e ora pianificate (inserire la data e l&#39;ora)
* Stato (Programmato, Riprogrammato, Annullato)

Obiettivo raggiunto: effettuato l’accesso a Marketo e popolato in Sales Insight quando un visitatore raggiunge un obiettivo in un flusso di dialogo.

* Nome dialogo
* Nome obiettivo
* URL pagina

Interazione con il documento: effettuato l’accesso a Marketo e popolato in Sales Insight quando un visitatore interagisce con un documento condiviso tramite il chatbot.

* Nome dialogo
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
* Nome dialogo
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

