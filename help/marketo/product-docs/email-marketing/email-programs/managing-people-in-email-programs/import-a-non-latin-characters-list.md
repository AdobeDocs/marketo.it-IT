---
unique-page-id: 5472678
description: Importare un elenco di caratteri non latini - Marketo Docs - Documentazione del prodotto
title: Importare un elenco di caratteri non latini
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Importare un elenco di caratteri non latini {#import-a-non-latin-characters-list}

Stai cercando di importare un file che non è in inglese? L&#39;elenco appare perfetto quando lo si apre con Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Ma quando lo importi in Marketo, potresti notare che i caratteri non inglesi non vengono presi correttamente.

![](assets/image2015-2-10-9-3a35-3a49.png)

Questo perché il file non viene salvato correttamente affinché Marketo riconosca tutti i caratteri non latini. La buona notizia è che ci sono alcuni semplici passi che puoi seguire per ripararlo.

1. Seleziona **Salva con nome...** dal **File** in Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Scegli **Testo Unicode UTF-16 (.txt)** come **Formato** opzione . In questo modo il file verrà codificato come Marketo può visualizzarlo.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo supporta anche UTF-8, Shift-JIS o EUC-JP.

1. Il nuovo file verrà salvato come file di testo con estensione .txt. Ma converte anche tutte le virgole nel file in schede. Dobbiamo cambiarlo di nuovo.

   >[!TIP]
   >
   >È possibile aprire il file di testo utilizzando **Blocco note** se si utilizza Windows o **TextEdit** se utilizzi un Mac.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Selezionare una scheda dal documento e copiarla.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Seleziona **Trova e sostituisci...** dal **Modifica** menu.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >L&#39;azione equivalente per gli utenti Windows è: **Modifica > Sostituisci..**

1. Incolla la scheda copiata al punto 4 nella prima casella (da sostituire) e digita una virgola nella seconda casella (sostituisci con). E fai clic su **Tutto**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. E voila, tutte le virgole sono tornate e siamo pronti a partire.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importa il nuovo file in Marketo e le informazioni devono essere visualizzate correttamente questa volta.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Tutti i campi data/ora da importare vengono trattati come Ora centrale. Se si dispone di campi data/ora in un fuso orario diverso, è possibile utilizzare una formula Excel per trasformarla in Ora centrale (America/Chicago).

Sappiamo che è strano, ma funziona. Felice importazione!
