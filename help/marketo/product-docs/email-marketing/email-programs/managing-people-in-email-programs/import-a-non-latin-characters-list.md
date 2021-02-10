---
unique-page-id: 5472678
description: Importa un elenco di caratteri non latini - Documenti Marketo - Documentazione prodotto
title: Importa elenco caratteri non latini
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Importa un elenco di caratteri non latini {#import-a-non-latin-characters-list}

Stai tentando di importare un file non in inglese? L&#39;elenco è perfetto quando viene aperto con Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Ma quando lo importate in Marketo, potreste vedere che i caratteri non inglesi non vengono presi correttamente.

![](assets/image2015-2-10-9-3a35-3a49.png)

Questo perché il file non viene salvato correttamente affinché Marketo riconosca tutti i caratteri non latini. La buona notizia è che ci sono alcuni semplici passi da seguire per ripararlo.

1. Selezionare **Salva con nome...** dal menu **File** in Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Scegliete **UTF-16 Unicode Text (.txt)** come opzione **Format**. Questo codificherà il file nel modo in cui Marketo può visualizzarlo.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo supporta anche UTF-8, Shift-JIS o EUC-JP.

1. Il nuovo file verrà salvato come file di testo con estensione .txt. Ma converte anche tutte le virgole nel file in schede. Dobbiamo rimetterlo in sesto.

   >[!TIP]
   >
   >È possibile aprire il file di testo utilizzando **Blocco note** se si utilizza Windows o **TextEdit** se si utilizza Mac.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Selezionare una scheda dal documento e copiarla.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Selezionare **Trova e sostituisci...** dal menu **Modifica**.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >L&#39;azione equivalente per gli utenti Windows è: **Modifica > Sostituisci...**

1. Incollare la scheda copiata al punto 4 nella prima casella (da sostituire) e digitare una virgola nella seconda casella (sostituire con). Fare clic su **All**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. E voilà, tutte le virgole sono tornate e siamo pronti a partire.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importa il nuovo file in Marketo, e le informazioni devono essere visualizzate correttamente questa volta.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Tutti i campi data/ora importati vengono considerati come Ora centrale. Se i campi data/ora si trovano in un fuso orario diverso, è possibile utilizzare una formula Excel per trasformarla in Ora centrale (America/Chicago).

Sappiamo che questo è strano, ma funziona. Felice Importare!
