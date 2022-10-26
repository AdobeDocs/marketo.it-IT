---
description: Integrazione dinamica della chat - Documenti Marketo - Documentazione del prodotto
title: Integrazione Chat dinamica
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
source-git-commit: 9d5c941dc4869b03787a6135550a133ce12b365b
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 3%

---

# Integrazione Chat dinamica {#dynamic-chat-integration}

Scopri di più sull’integrazione della chat dinamica con Sales Insight.

>[!PREREQUISITES]
>
>* Il pacchetto SFDC di Insight delle vendite deve essere una versione [1.9 o superiore](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;}
>
>* Devi avere la [Integrazione della chat dinamica](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md)Configurazione di {target=&quot;_blank&quot;}


## Scheda Configurazione di Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

Segui i passaggi riportati di seguito per abilitare l’integrazione di Chat dinamica.

1. Accedi al tuo account Salesforce, fai clic sul segno + alla fine della barra delle schede e fai clic su **Configurazione di Marketo Sales Insight**.

1. Fai clic su per espandere il &quot;Pannello Visualforce&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Seleziona la **Abilita dati chat dinamici** casella di controllo.

   ![](assets/dynamic-chat-integration-2.png)

## Panoramica delle funzioni {#feature-overview}

Le seguenti attività di chat dinamica possono essere sfruttate dagli utenti di Sales Insight...

Finestra di dialogo interattiva: Effettuato l’accesso a Marketo e compilato in Sales Insight quando un visitatore fa clic su un chatbot e si impegna con la finestra di dialogo.

* Nome dialogo
* URL della pagina
* Stato (Iniziato/Rilasciato/Completato)

Appuntamento programmato: Effettuato l’accesso a Marketo e compilato in Sales Insight quando un visitatore pianifica correttamente un appuntamento tramite il chatbot.

* Nome dialogo
* Agente
* URL della pagina
* Pianificato il (inserire data e ora)
* Stato (Pianificato, Riprogrammato, Annullato)

Obiettivo raggiunto: Effettuato l’accesso a Marketo e compilato in Sales Insight quando un visitatore raggiunge un obiettivo in qualsiasi flusso di dialogo.

* Nome dialogo
* Nome obiettivo
* URL della pagina

Interagito con Document: Effettuato l’accesso a Marketo e compilato in Sales Insight quando un visitatore interagisce con un documento condiviso tramite il chatbot.

* Nome dialogo
* Documento
* Stato

Le attività di chat sono disponibili nel dashboard di Insights.

![](assets/dynamic-chat-integration-3.png)

La scheda Chat è disponibile nei pannelli Lead e Contatto . Include le colonne Tipo di attività, Nome finestra di dialogo e Data .

![](assets/dynamic-chat-integration-4.png)

Per ulteriori informazioni su un tipo di attività, fai clic su di esso.

![](assets/dynamic-chat-integration-5.png)

Analogamente, i pannelli Account e Opportunità includono le colonne Nome, Tipo di attività, Nome finestra di dialogo e Data .

![](assets/dynamic-chat-integration-6.png)

La scheda Chat è inclusa anche nella scheda Marketo globale. Include tre tipi di attività (Finestra di dialogo impegnata, Appuntamento pianificato, Obiettivo raggiunto), insieme alle colonne seguenti:

* Persona
* Account
* Tipo di attività (finestra di dialogo impegnata, appuntamento pianificato, obiettivo raggiunto)
* Nome dialogo
* Data e ora

Anche in questo caso, fai clic su di esso per ulteriori informazioni su un tipo di attività.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Se la casella di controllo &quot;Abilita dati chat dinamica&quot; è disabilitata, le seguenti funzioni saranno disattivate:
>
>* Riga con attività Chat nel dashboard Approfondimenti (smart grid e vista a elenco settimanale)
>* Scheda Chat nei pannelli Lead, Contatto, Account e Opportunità
>* Scheda Chat nella scheda Marketo globale
>
>Non è possibile disattivare solo una di queste funzioni.

