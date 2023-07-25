---
unique-page-id: 2359520
description: Utilizzare il test A/B "Date/Time" (Data/Ora) - Documentazione di Marketo - Documentazione del prodotto
title: Utilizza test A/B "Data/ora"
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Utilizza test A/B &quot;Data/ora&quot; {#use-date-time-a-b-testing}

Puoi testare facilmente le e-mail tramite test A/B. Un test è **Data/ora** test. Questo verifica a quale ora del giorno o della settimana è meglio inviare le e-mail. Ecco come configurarlo.

>[!PREREQUISITES]
>
>[Aggiungere un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)
>

1. Sotto **E-mail** riquadro, fai clic su **Aggiungi test A/B**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. Viene visualizzata una nuova finestra. Seleziona **Data/ora** per **Tipo di test**.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. Se disponi di informazioni precedenti sul test (come un test dell’oggetto), puoi fare clic su **Ripristina test**.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. Seleziona la data per la prima data/ora.

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. Seleziona l’ora della prima data/ora.

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. Effettua la stessa operazione per il secondo giorno/ora.

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. Utilizza il cursore per scegliere la percentuale di pubblico desiderata nel test A/B e fai clic su **Successivo**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >Le diverse varianti vengono applicate alle parti uguali delle dimensioni del campione di test scelte.

   >[!CAUTION]
   >
   >**Si consiglia di evitare di impostare la dimensione del campione su 100%**. Se utilizzi un elenco statico, impostando la dimensione del campione su 100%, l’e-mail viene inviata a tutti gli utenti del pubblico e il vincitore non viene recapitato a nessuno. Se utilizzi un **intelligente** , impostando la dimensione del campione su 100%, invia l’e-mail a tutti gli utenti del pubblico _allora_. Quando il programma e-mail viene eseguito nuovamente in una data successiva, anche le nuove persone che si qualificano per l’elenco avanzato riceveranno l’e-mail, in quanto ora sono incluse nel pubblico.

   Ok, ci siamo avvicinati un passo. Ora dobbiamo [definire i criteri dei vincitori del test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
