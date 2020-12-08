---
unique-page-id: 2360219
description: Imposta una firma DKIM personalizzata - Documenti Marketo - Documentazione prodotto
title: Impostazione di una firma DKIM personalizzata
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Impostazione di una firma DKIM personalizzata {#set-up-a-custom-dkim-signature}

Al fine di garantire la massima recapito, tutti i messaggi in uscita vengono automaticamente firmati con una firma DKIM Marketo condivisa.

>[!NOTE]
>
>Potrebbe essere necessario l&#39;aiuto del team IT per completare alcuni dei passaggi descritti in questo articolo.

È possibile personalizzare la firma DKIM in modo da riflettere i domini di propria scelta. Ecco come.

1. Andate alla sezione **Admin** .

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >
   >Se imposti una firma DKIM personalizzata nel modo precedente, continuerà a funzionare e dovrebbe comparire qui.

1. Fate clic su **E-mail**, quindi sulla scheda **DKIM** e infine su **Aggiungi dominio**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. Immettete il dominio che verrà utilizzato nelle e-mail di Marketo come indirizzo Da e fate clic su **Aggiungi**.

   >[!TIP]
   >
   >
   >Se utilizzi un dominio diverso nell’indirizzo Da, utilizzeremo la firma DKIM condivisa da Marketo.

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. Inviate il record **** host e il valore **** TXT all&#39;IT. Chiedete loro di creare il record e assicuratevi che si propaghi a tutti i server dei nomi associati al dominio da. La verifica DKIM di Marketo richiede che la chiave DKIM venga propagata a tutti i server dei nomi associati al dominio in cui è firmata DKIM.

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. Dopo aver confermato di aver creato il record, tornare a Marketo, selezionare il dominio e fare clic su **Controlla DNS**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >**Promemoria**
   >
   >Se la conferma non riesce e l&#39;IT ha creato correttamente il record, potrebbe trattarsi di una questione di propagazione DNS. Riprova più tardi.

   >[!CAUTION]
   >
   >
   >Modificando/rimuovendo il record DNS corrispondente si verificherà un danneggiamento della recapito. Assicurarsi di eliminare la voce in Marketo prima di apportare modifiche DNS.

   In questo modo sarà assolutamente utile gestire la tua recapito delle e-mail. È necessario ottenere la convalida che il record è presente e corretto.

