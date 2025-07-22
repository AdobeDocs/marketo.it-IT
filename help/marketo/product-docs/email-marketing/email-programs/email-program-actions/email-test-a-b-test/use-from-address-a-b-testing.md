---
unique-page-id: 2359504
description: Utilizzare il test A/B "From Address" - Documentazione di Marketo - Documentazione del prodotto
title: Utilizza test A/B "Indirizzo Da"
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Usa test A/B [!UICONTROL From Address] {#use-from-address-a-b-testing}

Puoi testare facilmente le e-mail tramite test A/B. Un test interessante è il test **[!UICONTROL From Address]**. Ecco come configurarlo.

>[!PREREQUISITES]
>
>[Aggiungi un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Nella sezione **[!UICONTROL Email]**, con l&#39;e-mail selezionata, fai clic su **[!UICONTROL Add A/B Test]**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Viene visualizzata una nuova finestra. Selezionare **[!UICONTROL From Address]** per **[!UICONTROL Test Type]**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Se si dispone di informazioni di test precedenti, ad esempio un test dell&#39;oggetto, è possibile fare clic su **[!UICONTROL Reset Test]**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Immettere le seconde informazioni di **[!UICONTROL From Address]** che si desidera verificare.

   >[!NOTE]
   >
   >La scelta A verrà precompilata con le informazioni contenute nell’e-mail selezionata.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >È possibile fare clic su **+** per aggiungere tutti gli indirizzi da desiderati.

1. Utilizza il cursore per scegliere la percentuale di pubblico desiderata nel test A/B e fai clic su **[!UICONTROL Next]**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >Le diverse varianti vengono inviate a parti uguali delle dimensioni del campione di test scelte.

   >[!CAUTION]
   >
   >**Si consiglia di evitare di impostare la dimensione del campione su 100%**. Se utilizzi un elenco statico, impostando la dimensione del campione su 100%, l’e-mail viene inviata a tutti gli utenti del pubblico e il vincitore non viene recapitato a nessuno. Se utilizzi un elenco **smart**, l&#39;impostazione della dimensione del campione su 100% invia l&#39;e-mail a tutti gli utenti del pubblico _in quel momento_. Quando il programma e-mail viene eseguito nuovamente in una data successiva, anche le nuove persone che si qualificano per l’elenco avanzato riceveranno l’e-mail, in quanto ora sono incluse nel pubblico.

   Ok, ci siamo quasi. Ora è necessario [definire i criteri del vincitore del test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
