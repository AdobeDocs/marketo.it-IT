---
unique-page-id: 2359504
description: Utilizzare il test A/B "Da indirizzo" - Documenti Marketo - Documentazione del prodotto
title: Utilizzare il test A/B "Da indirizzo"
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Utilizzare il test A/B &quot;Da indirizzo&quot; {#use-from-address-a-b-testing}

Puoi testare facilmente le tue e-mail tramite A/B. Un test interessante è **Indirizzo mittente** test. Ecco come configurarlo.

>[!PREREQUISITES]
>
>[Aggiungere un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Sotto la **E-mail** con l’e-mail selezionata, fai clic su **Aggiungi test A/B**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Viene visualizzata una nuova finestra, seleziona **Indirizzo mittente** per **Tipo di test**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Se disponi di informazioni di test precedenti (come un test del soggetto), puoi tranquillamente fare clic su **Ripristina test**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Inserisci il secondo **Indirizzo mittente** informazioni da verificare.

   >[!NOTE]
   >
   >La scelta A si precompila con le informazioni contenute nell’e-mail selezionata.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Puoi fare clic sul pulsante **+** per aggiungere tutti gli indirizzi da desiderati.

1. Utilizza il cursore per scegliere la percentuale di pubblico desiderato nel test A/B e fai clic su **Successivo**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >Le diverse varianti invieranno a parti uguali della dimensione del campione di prova selezionata.

   >[!CAUTION]
   >
   >**Evita di impostare la dimensione del campione su 100%**. Se utilizzi un elenco statico, l’impostazione della dimensione del campione su 100% invia l’e-mail a tutti i tipi di pubblico e il vincitore non arriva a nessuno. Se utilizzi un **intelligente** elenco , se imposti la dimensione del campione su 100% , invia l’e-mail a tutti gli utenti del pubblico _a quell&#39;ora_. Quando il programma e-mail viene eseguito di nuovo in una data successiva, anche tutte le nuove persone che si qualificano per l’elenco smart riceveranno l’e-mail in quanto ora sono incluse nel pubblico.

   OK, siamo quasi lì. Ora dobbiamo [definire i criteri del vincitore del test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
