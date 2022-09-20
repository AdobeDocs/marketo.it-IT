---
unique-page-id: 7513680
description: Automatizzare un avviso per le persone duplicate possibili - Documenti Marketo - Documentazione del prodotto
title: Automatizzare un avviso per le persone duplicate possibili
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
source-git-commit: 50fc46312d2c7c25556994fad4e118c01cf92fc0
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Automatizzare un avviso per le persone duplicate possibili {#automate-an-alert-for-possible-duplicate-people}

Vuoi un avviso ogni volta che viene creata una persona duplicata possibile? Ecco come impostare una campagna avanzata per farlo.

1. [Creare una nuova campagna intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target=&quot;_blank&quot;}. Definisci il seguente elenco di smart:

* Trigger: **Persona creata**
* Filtro: **Campi duplicati.** Nome campo **è Nome completo**

   ![](assets/automate-an-alert-1.png)

   >[!TIP]
   >
   >Sii creativo. Sperimenta con campi diversi per ottenere risultati di filtro migliori.

1. Nel passaggio del flusso, scegli [Invia avviso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)Azione di flusso {target=&quot;_blank&quot;}.

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >Utilizzo della [Invia token informazioni avviso](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;} per includere un collegamento alla persona nel CRM.

   >[!CAUTION]
   >
   >Se importi un elenco di grandi dimensioni, puoi ricevere un sacco di questi avvisi tutti contemporaneamente!
   >
   >Inoltre, due persone con lo stesso nome non significa automaticamente che sono la stessa persona.

1. Attiva la campagna nella **Pianificazione** scheda .

   ![](assets/automate-an-alert-3.png)

Tutto qui! Questa campagna intelligente viene attivata ogni volta che una nuova persona con un nome completo esistente viene creata in Marketo.

>[!MORELIKETHIS]
>
>[Trova e unisci persone duplicate](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target=&quot;_blank&quot;}
