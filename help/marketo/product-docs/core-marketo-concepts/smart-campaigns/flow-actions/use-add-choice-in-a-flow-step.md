---
unique-page-id: 1146980
description: Utilizzare Aggiungi scelta in un passaggio di flusso - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzare Aggiungi scelta in un passaggio di flusso
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 7%

---

# Utilizzare Aggiungi scelta in un passaggio di flusso {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[Aggiungere un passaggio di flusso a una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

&quot;Aggiungi scelta&quot; consente di utilizzare un passaggio di flusso e di dire &quot;dipende&quot; quando si scelgono i dettagli.

1. Nella scheda **[!UICONTROL Flow]** di Smart Campaign, aggiungi un passaggio di flusso e fai clic su **[!UICONTROL Add Choice]**.

   ![](assets/use-add-choice-in-a-flow-step-1.png)

1. Seleziona la condizione di scelta.

   ![](assets/use-add-choice-in-a-flow-step-2.png)

1. Scegliere l&#39;operatore di scelta e immettere un valore di scelta. In questo modo si impostano i criteri o la scelta.

   ![](assets/use-add-choice-in-a-flow-step-3.png)

1. Immettere un valore per la fase di flusso per la scelta.

   ![](assets/use-add-choice-in-a-flow-step-4.png)

   >[!CAUTION]
   >
   >I token _non_ funzioneranno nella parte della condizione di un passaggio del flusso di scelta.

1. Ripeti i passaggi precedenti per aggiungere più scelte, quindi aggiungi/regola il valore predefinito.

   ![](assets/use-add-choice-in-a-flow-step-5.png)

   >[!TIP]
   >
   >È possibile impostare uno qualsiasi dei passaggi di flusso su - Nessuna azione -, nel qual caso non verrà intrapresa alcuna azione su tale scelta.

   >[!CAUTION]
   >
   >Al passaggio del flusso viene applicata solo la prima scelta corrispondente. Scopri come [riordinare &quot;Aggiungi scelta&quot; in un&#39;azione di flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}.

   Fantastico! È ora possibile creare una singola campagna avanzata con scelte dei passaggi di flusso anziché creare più campagne avanzate per ogni scelta.

   >[!MORELIKETHIS]
   >
   >[Riordina la scelta di aggiunta in un passaggio del flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}
