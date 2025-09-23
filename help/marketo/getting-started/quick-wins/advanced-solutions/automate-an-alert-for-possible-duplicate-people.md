---
unique-page-id: 7513680
description: Automatizzare un avviso per potenziali persone duplicate - Documentazione di Marketo - Documentazione del prodotto
title: Automatizzare un avviso per possibili persone duplicate
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 10%

---

# Automatizzare un avviso per possibili persone duplicate {#automate-an-alert-for-possible-duplicate-people}

Vuoi ricevere un avviso ogni volta che viene creata una persona duplicata? Ecco come impostare una campagna avanzata per farlo.

1. [Crea una nuova campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}. Definisci il seguente elenco avanzato:

* Trigger: **[!UICONTROL Person is Created]**
* Filtro: **[!UICONTROL Duplicate Fields]**. Nome Campo **[!UICONTROL is][!UICONTROL Full Name]**

  ![](assets/automate-an-alert-1.png)

  >[!TIP]
  >
  >Sii creativo. Sperimenta diversi campi per ottenere risultati di filtro migliori.

1. Nel passaggio del flusso, scegliere [[!UICONTROL Send Alert]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target="_blank"} azione di flusso.

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >Utilizzo del token [Invia informazioni avviso](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"} per includere un collegamento alla persona nel CRM.

   >[!CAUTION]
   >
   >Se si importa un elenco di grandi dimensioni, è possibile che vengano visualizzati alcuni di questi avvisi contemporaneamente.
   >
   >Inoltre, due persone con lo stesso nome non significa automaticamente che siano la stessa persona.

1. Attiva la campagna nella scheda **[!UICONTROL Schedule]**.

   ![](assets/automate-an-alert-3.png)

Tutto qui. Questa campagna intelligente verrà attivata ogni volta che in Marketo viene creata una nuova persona con un nome completo esistente.

>[!MORELIKETHIS]
>
>[Trova e unisci persone duplicate](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}
