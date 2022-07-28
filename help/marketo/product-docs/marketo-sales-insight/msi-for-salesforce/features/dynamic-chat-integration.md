---
description: Integrazione dinamica della chat - Documenti Marketo - Documentazione del prodotto
title: Integrazione Chat dinamica
hide: true
hidefromtoc: true
source-git-commit: ea2ee32a4c8805154f17717d515bb994dbfbe982
workflow-type: tm+mt
source-wordcount: '304'
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

1. Accedi al tuo account Salesforce, fai clic sul segno + alla fine della barra delle schede e fai clic su **Configurazione di Marketo Sales Insight**.

1. Fai clic su per espandere il &quot;Pannello Visualforce&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Seleziona la **Abilita dati chat dinamici** casella di controllo.

   ![](assets/dynamic-chat-integration-2.png)

## Panoramica delle funzioni {#feature-overview}

Le attività di Chat dinamica riportate di seguito possono essere sfruttate dagli utenti di Sales Insight.

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

La scheda Chat è disponibile nei pannelli Lead e Contatto . Include le colonne Tipo di attività, Nome finestra di dialogo e Data .

![](assets/dynamic-chat-integration-3.png)

Per ulteriori informazioni su un tipo di attività, fai clic su di esso.

![](assets/dynamic-chat-integration-4.png)

Analogamente, i pannelli Account e Opportunità includono le colonne Nome, Tipo di attività, Nome finestra di dialogo e Data .

![](assets/dynamic-chat-integration-5.png)

La scheda Chat è inclusa anche nella scheda Marketo globale. Include tre tipi di attività (Finestra di dialogo impegnata, Appuntamento pianificato, Obiettivo raggiunto), insieme alle colonne seguenti:

* Persona
* Account
* Tipo di attività (finestra di dialogo impegnata, appuntamento pianificato, obiettivo raggiunto)
* Nome dialogo
* Data e ora

Anche in questo caso, fai clic su di esso per ulteriori informazioni su un tipo di attività.

![](assets/dynamic-chat-integration-6.png)

>[!NOTE]
>
>L’attività &quot;Interagito con il documento&quot; sarà disponibile in MSI in una prossima versione.
