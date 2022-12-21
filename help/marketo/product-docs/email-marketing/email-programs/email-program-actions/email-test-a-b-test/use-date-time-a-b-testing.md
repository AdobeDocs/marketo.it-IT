---
unique-page-id: 2359520
description: Utilizzare i test A/B "Data/ora" - Documenti Marketo - Documentazione del prodotto
title: Utilizzare il test A/B "Data/ora"
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Utilizzare il test A/B &quot;Data/ora&quot; {#use-date-time-a-b-testing}

Puoi testare facilmente le tue e-mail tramite A/B. Un test è **Data/ora** test. Questo verifica quale ora del giorno o giorno della settimana è meglio inviare e-mail. Ecco come configurarlo.

>[!PREREQUISITES]
>
>[Aggiungere un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Sotto la **E-mail** riquadro, fai clic su **Aggiungi test A/B**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. Si apre una nuova finestra. Seleziona **Data/ora** per **Tipo di test**.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. Se disponi di informazioni di test precedenti (come un test del soggetto), puoi tranquillamente fare clic su **Ripristina test**.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. Seleziona la data della prima data/ora.

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. Seleziona l’ora della tua prima data/ora.

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. Fai lo stesso per la tua seconda data/ora.

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. Utilizza il cursore per scegliere la percentuale di pubblico desiderato nel test A/B e fai clic su **Successivo**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >Le diverse varianti si applicano a parti uguali della dimensione del campione di prova selezionata.

   >[!CAUTION]
   >
   >**Evita di impostare la dimensione del campione su 100%**. Se utilizzi un elenco statico, l’impostazione della dimensione del campione su 100% invia l’e-mail a tutti i tipi di pubblico e il vincitore non arriva a nessuno. Se utilizzi un **intelligente** elenco , se imposti la dimensione del campione su 100% , invia l’e-mail a tutti gli utenti del pubblico _a quell&#39;ora_. Quando il programma e-mail viene eseguito di nuovo in una data successiva, anche tutte le nuove persone che si qualificano per l’elenco smart riceveranno l’e-mail in quanto ora sono incluse nel pubblico.

   Ok, siamo un passo più vicini. Ora dobbiamo [definire i criteri del vincitore del test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
