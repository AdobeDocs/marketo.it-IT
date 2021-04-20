---
title: define-a-smart-list-for-a-batch-campaign
description: Definire un elenco avanzato per una campagna batch
exl-id: 35130f40-cce5-4677-8eaf-f9d73c995ba3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Definire un elenco avanzato per una campagna batch

<br> 

Gli elenchi avanzati sono il meccanismo utilizzato in Marketo per definire &quot;chi&quot; (quali persone) da includere, sia che si tratti di un rapporto, di un elenco o di una campagna intelligente. Ecco come definire un elenco smart per una campagna batch.

1. Scegli una campagna avanzata, quindi fai clic su **[!UICONTROL Smart List]**.

   ![Immagine uno](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-1.png)

1. Digita per cercare un filtro, quindi trascinalo e rilascialo nell’area di lavoro. Ripeti l’operazione per più filtri.

   ![Immagine 2](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-2.png)

   >[!NOTE]
   >
   >Una campagna intelligente con solo filtri viene eseguita in modalità batch. Trova le persone nel database che si qualificano in base ai filtri e le esegue tutte in una sola volta nel flusso.

   >[!IMPORTANT]
   >
   >Puoi eseguire una campagna intelligente su una persona alla volta in base agli eventi live aggiungendo dei trigger, che attivano la campagna intelligente in modalità Trigger.

1. Fai clic sull’elenco a discesa e scegli un operatore di filtro (ad es. **[!UICONTROL is]**, **[!UICONTROL is not]**, ecc.,) per il filtro scelto.

   ![Immagine tre](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-3.png)

   >[!CAUTION]
   >
   >Le linee rosse indicano errori o informazioni mancanti. Se non viene corretta, la campagna non sarà valida e non verrà eseguita.

1. Immetti il valore del filtro.

   ![Immagine quattro](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-4.png)

>[!NOTE]
>
>Per impostazione predefinita, le persone che soddisfano TUTTE le regole dell’elenco smart sono
>qualificati. Può essere modificato in base alle esigenze della campagna. Consulta [Regole di elenco avanzato per la logica complessa](https://docs.marketo.com/display/DOCS/Using+Advanced+Smart+List+Rule+Logic) per ulteriori informazioni.
>
>Per attivare eventi live una persona alla volta, scopri come [definire un elenco avanzato per Smart Campaign | Trigger](https://docs.marketo.com/display/DOCS/Define+Smart+List+for+Smart+Campaign+%7C+Trigger).
