---
unique-page-id: 2359502
description: Utilizzare il test A/B "E-mail intera" - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzare il test A/B “E-mail intera”
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
feature: Email Programs, A/B Testing
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 6%

---

# Utilizzare il test A/B “E-mail intera” {#use-whole-email-a-b-testing}

Puoi testare facilmente le e-mail tramite test A/B. Un ottimo test è il test **E-mail intera**. Ecco come configurarlo.

>[!PREREQUISITES]
>
>[Aggiungi un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Nel riquadro E-mail, con l&#39;e-mail selezionata, fai clic su **[!UICONTROL Add A/B Test]**.

![](assets/image2014-9-12-15-3a22-3a12.png)

1. Viene visualizzata una nuova finestra. Fai clic sul menu a discesa **[!UICONTROL Test Type]** e seleziona **[!UICONTROL Whole Emails]**.

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. Se si dispone di informazioni di test precedenti, ad esempio un test dell&#39;oggetto, è possibile fare clic su **[!UICONTROL Reset Test]**.

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. Seleziona la prima e-mail.

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. Fare clic su **[!UICONTROL Add]** per applicare l&#39;e-mail.

   ![](assets/image2014-9-12-15-3a23-3a20.png)

   >[!TIP]
   >
   >Puoi aggiungere più e-mail. Tuttavia, se ne aggiungi troppi, il processo di test potrebbe risultare rallentato.

1. Seleziona la seconda e-mail.

   [&#128279;](assets/image2014-9-12-15-3a23-3a49.png)

1. Fare clic su **[!UICONTROL Add]** per applicare la seconda e-mail. Trascina il cursore per scegliere la percentuale del pubblico che desideri ricevere il test A/B e fai clic su **[!UICONTROL Next]**.

   [&#128279;](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >Le diverse varianti invieranno parti uguali delle **dimensioni campione test** scelte.

   >[!CAUTION]
   >
   >**Si consiglia di evitare di impostare la dimensione del campione su 100%**. Se utilizzi un elenco statico, impostando la dimensione del campione su 100%, l’e-mail viene inviata a tutti gli utenti del pubblico e il vincitore non viene recapitato a nessuno. Se utilizzi un elenco **smart**, l&#39;impostazione della dimensione del campione su 100% invia l&#39;e-mail a tutti gli utenti del pubblico _in quel momento_. Quando il programma e-mail viene eseguito nuovamente in una data successiva, anche le nuove persone che si qualificano per l’elenco avanzato riceveranno l’e-mail, in quanto ora sono incluse nel pubblico.

   Ok, ci siamo quasi. Ora è necessario [definire i criteri del vincitore del test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
