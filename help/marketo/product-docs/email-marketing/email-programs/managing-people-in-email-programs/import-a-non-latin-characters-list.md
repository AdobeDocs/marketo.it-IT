---
unique-page-id: 5472678
description: Importare un elenco di caratteri non latini - Documenti Marketo - Documentazione del prodotto
title: Importa un elenco di caratteri non latini
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Importa un elenco di caratteri non latini {#import-a-non-latin-characters-list}

Si sta tentando di importare un file non in inglese? L’elenco si presenta perfetto quando lo si apre con Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Ma quando lo importi in Marketo, potresti notare che i caratteri non inglesi non vengono rilevati correttamente.

![](assets/image2015-2-10-9-3a35-3a49.png)

Questo perché il file non viene salvato correttamente affinché Marketo possa riconoscere tutti i caratteri non latini. La buona notizia è che ci sono alcuni semplici passaggi che puoi seguire per risolvere il problema.

1. Seleziona **Salva con nome...** dal **File** in Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Scegli **Testo Unicode UTF-16 (.txt)** come **Formato** opzione. In questo modo il file verrà codificato nel modo in cui Marketo può visualizzarlo.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo supporta anche UTF-8, Shift-JIS o EUC-JP.

1. Il nuovo file verrà salvato come file di testo con estensione .txt. Ma converte anche tutte le virgole nel file in schede. Dobbiamo ripristinarla.

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
   >L&#39;azione equivalente per gli utenti di Windows è: **Modifica > Sostituisci...**

1. Incollare la scheda copiata al punto 4 nella prima casella (da sostituire) e digitare una virgola nella seconda casella (sostituisci con). E fai clic su **Tutti**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. E voilà, sono tornate tutte le virgole e siamo pronti a muoverci.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importa il nuovo file in Marketo e le informazioni devono essere visualizzate correttamente in questo momento.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Tutti i campi data/ora importati vengono trattati come ora centrale. Se sono presenti campi data/ora in un fuso orario diverso, è possibile utilizzare una formula di Excel per trasformarla in Ora centrale (America/Chicago).

Sappiamo che è strano, ma funziona. Buona Importazione!
