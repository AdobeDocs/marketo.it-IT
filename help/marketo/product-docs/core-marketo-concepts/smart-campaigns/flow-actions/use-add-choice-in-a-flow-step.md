---
unique-page-id: 1146980
description: Utilizzare Add Choice in un passaggio di flusso - Marketo Docs - Documentazione prodotto
title: Usa opzione Aggiungi in un passaggio di flusso
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# Usa opzione Aggiungi in un passaggio di flusso {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>* [Aggiunta di un passaggio di flusso a una campagna intelligente](add-a-flow-step-to-a-smart-campaign.md)

>



**Aggiungi scelta** consente di utilizzare un passaggio di flusso e di specificare &quot;Dipende&quot; quando si scelgono i dettagli.

1. Nella scheda **Flusso** della campagna intelligente, aggiungi un passaggio di flusso e fai clic su **Aggiungi scelta**.

   ![](assets/image2014-9-22-11-3a58-3a20.png)

1. Selezionare la condizione di scelta.

   ![](assets/image2014-9-22-11-3a58-3a50.png)

1. Scegliete l’operatore di scelta e immettete un valore di scelta. Questo imposta i criteri o la scelta.

   ![](assets/image2014-9-22-11-3a58-3a54.png)

1. Immettete un valore per il passaggio di flusso per la scelta.

   ![](assets/image2014-9-22-11-3a58-3a57.png)

   >[!CAUTION]
   >
   >I token **non** funzioneranno nella parte di condizione di un passaggio di flusso di scelta.

1. Ripetete i passaggi indicati sopra per aggiungere più opzioni, quindi aggiungete o regolate il valore predefinito.

   ![](assets/image2014-9-22-11-3a58-3a59.png)

   >[!TIP]
   >
   >Potete impostare uno qualsiasi dei passaggi di flusso su —Do Nothing—, nel qual caso non verrà eseguita alcuna azione su tale scelta.

   >[!CAUTION]
   >
   >Al passaggio di flusso viene applicata solo la prima scelta corrispondente. Scopri come [riordinare &quot;Add Choice&quot; in un’azione](reorder-add-choice-in-a-flow-step.md)di flusso.

   >[!NOTE]
   >
   >**Articoli correlati**
   >
   >    
   >    
   >    * [Riordinare &quot;Add Choice&quot; in un passaggio di flusso](reorder-add-choice-in-a-flow-step.md)


Fantastico! Ora puoi creare una singola campagna intelligente con scelte di passaggi di flusso invece di creare più campagne intelligenti per ogni scelta.