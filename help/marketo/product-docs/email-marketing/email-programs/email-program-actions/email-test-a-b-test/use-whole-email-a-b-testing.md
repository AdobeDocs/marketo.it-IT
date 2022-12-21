---
unique-page-id: 2359502
description: Utilizzare test A/B "all’intero messaggio e-mail" - Documenti Marketo - Documentazione del prodotto
title: Utilizzare il test A/B per "E-mail intera"
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Utilizzare il test A/B per &quot;E-mail intera&quot; {#use-whole-email-a-b-testing}

Puoi testare facilmente le tue e-mail tramite A/B. Un grande test è il **E-mail completa** test. Ecco come configurarlo.

>[!PREREQUISITES]
>
>[Aggiungere un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Nella sezione E-mail, con l’e-mail selezionata, fai clic su **Aggiungi test A/B**.

![](assets/image2014-9-12-15-3a22-3a12.png)

1. Si apre una nuova finestra. Fai clic sul pulsante **Tipo di test** a discesa e seleziona **E-mail intere**.

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. Se disponi di informazioni di test precedenti (come un test del soggetto), puoi tranquillamente fare clic su **Ripristina test**.

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. Seleziona il tuo primo messaggio e-mail.

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. Fai clic su **Aggiungi** per applicare l’e-mail.

   ![](assets/image2014-9-12-15-3a23-3a20.png)

   >[!TIP]
   >
   >Puoi aggiungere più e-mail. Tuttavia, se ne aggiungi troppi, può rallentare il processo di test molto in basso.

1. Seleziona il tuo secondo messaggio e-mail.

   [](assets/image2014-9-12-15-3a23-3a49.png)

1. Fai clic su **Aggiungi** per applicare il secondo messaggio e-mail. Trascina il cursore per scegliere la percentuale di pubblico che desideri ricevere il test A/B e fai clic su **Successivo**.

   [](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >Le diverse varianti invieranno a parti uguali della scelta **Dimensione del campione del test**.

   >[!CAUTION]
   >
   >**Evita di impostare la dimensione del campione su 100%**. Se utilizzi un elenco statico, l’impostazione della dimensione del campione su 100% invia l’e-mail a tutti i tipi di pubblico e il vincitore non arriva a nessuno. Se utilizzi un **intelligente** elenco , se imposti la dimensione del campione su 100% , invia l’e-mail a tutti gli utenti del pubblico _a quell&#39;ora_. Quando il programma e-mail viene eseguito di nuovo in una data successiva, anche tutte le nuove persone che si qualificano per l’elenco smart riceveranno l’e-mail in quanto ora sono incluse nel pubblico.

   Ok, ci siamo quasi. Ora dobbiamo [definire i criteri del vincitore del test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
