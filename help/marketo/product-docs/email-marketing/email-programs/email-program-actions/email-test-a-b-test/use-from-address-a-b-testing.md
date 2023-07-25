---
unique-page-id: 2359504
description: Utilizzare il test A/B "From Address" - Documentazione di Marketo - Documentazione del prodotto
title: Utilizza test A/B "Indirizzo Da"
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Utilizza test A/B &quot;Indirizzo Da&quot; {#use-from-address-a-b-testing}

Puoi testare facilmente le e-mail tramite test A/B. Un test interessante è **Indirizzo mittente** test. Ecco come configurarlo.

>[!PREREQUISITES]
>
>[Aggiungere un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Sotto **E-mail** riquadro, con l’e-mail selezionata, fai clic su **Aggiungi test A/B**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Viene visualizzata una nuova finestra e seleziona **Indirizzo mittente** per **Tipo di test**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Se disponi di informazioni precedenti sul test (come un test dell’oggetto), puoi fare clic su **Ripristina test**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Inserisci il secondo **Indirizzo mittente** informazioni da verificare.

   >[!NOTE]
   >
   >La scelta A verrà precompilata con le informazioni contenute nell’e-mail selezionata.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Puoi fare clic sul pulsante **+** per aggiungere tutti gli indirizzi da desiderati.

1. Utilizza il cursore per scegliere la percentuale di pubblico desiderata nel test A/B e fai clic su **Successivo**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >Le diverse varianti vengono inviate a parti uguali delle dimensioni del campione di test scelte.

   >[!CAUTION]
   >
   >**Si consiglia di evitare di impostare la dimensione del campione su 100%**. Se utilizzi un elenco statico, impostando la dimensione del campione su 100%, l’e-mail viene inviata a tutti gli utenti del pubblico e il vincitore non viene recapitato a nessuno. Se utilizzi un **intelligente** , impostando la dimensione del campione su 100%, invia l’e-mail a tutti gli utenti del pubblico _allora_. Quando il programma e-mail viene eseguito nuovamente in una data successiva, anche le nuove persone che si qualificano per l’elenco avanzato riceveranno l’e-mail, in quanto ora sono incluse nel pubblico.

   Ok, ci siamo quasi. Ora dobbiamo [definire i criteri dei vincitori del test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
