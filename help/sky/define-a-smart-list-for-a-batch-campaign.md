---
title: define-a-smart-list-for-a-batch-campaign
description: Definire un elenco avanzato per una campagna batch
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Definire un elenco avanzato per una campagna batch

<br> 

Gli elenchi avanzati sono il meccanismo utilizzato da Marketo per definire &quot;chi&quot; (quali persone) da includere, sia che si tratti di un rapporto, un elenco o una campagna intelligente. Di seguito viene illustrato come definire un elenco smart per una campagna batch.

1. Scegliete una campagna intelligente, quindi fate clic su **[!UICONTROL Smart List]**.

   ![Immagine uno](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-1.png)

1. Digitate per cercare un filtro, quindi trascinatelo e rilasciatelo sul quadro. Ripetere questa procedura per più filtri.

   ![Immagine due](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-2.png)

   >[!NOTE]
   >
   >Una campagna intelligente con solo filtri viene eseguita in modalità batch. Trova persone nel database che si qualificano in base ai filtri ed esegue tutte le persone attraverso il flusso contemporaneamente.

   >[!IMPORTANT]
   >
   >Potete eseguire una campagna intelligente su una persona alla volta in base agli eventi in diretta aggiungendo attivatori, che attivano la campagna in modalità Trigger.

1. Fate clic sul menu a discesa e scegliete un operatore di filtro (ad es. **[!UICONTROL is]**, **[!UICONTROL is not]**, ecc.) per il filtro scelto.

   ![Immagine tre](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-3.png)

   >[!CAUTION]
   >
   >Le linee rosse indicano errori o informazioni mancanti. Se non viene corretta, la campagna non sarà valida e non verrà eseguita.

1. Immettete il valore del filtro.

   ![Immagine quattro](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-4.png)

>[!NOTE]
>
>Per impostazione predefinita, le persone che soddisfano TUTTE le regole dell&#39;elenco smart sono
>qualificato. Può essere modificato in base alle esigenze della campagna. Per ulteriori informazioni, consultare le [Regole di elenchi avanzati per la logica complessa](https://docs.marketo.com/display/DOCS/Using+Advanced+Smart+List+Rule+Logic).
>
>Per attivare eventi in diretta una persona alla volta, scopri come [Definire l&#39;elenco avanzato per la campagna intelligente | Trigger](https://docs.marketo.com/display/DOCS/Define+Smart+List+for+Smart+Campaign+%7C+Trigger).
