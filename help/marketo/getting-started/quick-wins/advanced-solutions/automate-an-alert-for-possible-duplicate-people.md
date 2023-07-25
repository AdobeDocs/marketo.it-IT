---
unique-page-id: 7513680
description: Automatizzare un avviso per potenziali persone duplicate - Documentazione di Marketo - Documentazione del prodotto
title: Automatizzare un avviso per eventuali persone duplicate
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Automatizzare un avviso per eventuali persone duplicate {#automate-an-alert-for-possible-duplicate-people}

Vuoi ricevere un avviso ogni volta che viene creata una persona duplicata? Ecco come impostare una campagna avanzata per farlo.

1. [Creare una nuova campagna intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}. Definisci il seguente elenco avanzato:

* Attivatore: **[!UICONTROL Persona creata]**
* Filtro: **[!UICONTROL Campi duplicati]**. Nome campo **[!UICONTROL è] [!UICONTROL Nome e cognome]**

  ![](assets/automate-an-alert-1.png)

  >[!TIP]
  >
  >Sii creativo. Sperimenta diversi campi per ottenere risultati di filtro migliori.

1. Nel passaggio del flusso, scegli [[!UICONTROL Invia avviso]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target="_blank"} azione di flusso.

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >Utilizzo di [Invia token di informazioni avviso](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"} per includere un collegamento alla persona nel CRM.

   >[!CAUTION]
   >
   >Se si importa un elenco di grandi dimensioni, è possibile che vengano visualizzati alcuni di questi avvisi contemporaneamente.
   >
   >Inoltre, due persone con lo stesso nome non significa automaticamente che siano la stessa persona.

1. Attiva la campagna in **[!UICONTROL Pianificazione]** scheda.

   ![](assets/automate-an-alert-3.png)

Tutto qui! Questa campagna intelligente verrà attivata ogni volta che in Marketo viene creata una nuova persona con un nome completo esistente.

>[!MORELIKETHIS]
>
>[Trova e unisci persone duplicate](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}
