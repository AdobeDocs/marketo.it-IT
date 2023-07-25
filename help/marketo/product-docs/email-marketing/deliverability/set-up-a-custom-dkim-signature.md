---
unique-page-id: 2360219
description: Configurare una firma DKIM personalizzata - Documentazione Marketo - Documentazione del prodotto
title: Impostare una firma DKIM personalizzata
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# Impostare una firma DKIM personalizzata {#set-up-a-custom-dkim-signature}

Per garantire un recapito messaggi di prima qualità, firmiamo automaticamente tutti i messaggi in uscita con una firma DKIM di Marketo condivisa.

>[!NOTE]
>
>Potrebbe essere necessario l’aiuto del team IT per completare alcuni dei passaggi descritti in questo articolo.

Puoi personalizzare la firma DKIM per riflettere i domini selezionati. Ecco come.

1. Vai a **Amministratore** sezione.

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >Se imposti una firma DKIM personalizzata secondo la vecchia modalità, questa continuerà a funzionare e dovrebbe essere visualizzata qui.

1. Clic **E-mail**, quindi **DKIM** e infine **Aggiungi dominio**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. Immetti il dominio da utilizzare nelle e-mail Marketo come indirizzo del mittente e fai clic su **Aggiungi**.

   >[!TIP]
   >
   >Se utilizzi un dominio diverso nell’indirizzo Da, verrà utilizzata la firma DKIM condivisa di Marketo.

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. Invia il **Record host** e **Valore TXT** al tuo IT. Chiedere loro di creare il record e assicurarsi che venga propagato a tutti i server dei nomi associati al dominio di origine. La verifica DKIM di Marketo richiede che la chiave DKIM venga propagata a tutti i server dei nomi associati al dominio con firma DKIM.

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. Dopo aver confermato la creazione del record, torna a Marketo, seleziona il dominio e fai clic su **Controlla DNS**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >Se la conferma non riesce e il reparto di IT ha creato correttamente il record, potrebbe trattarsi di una questione di propagazione DNS. Riprova più tardi.

   >[!CAUTION]
   >
   >La modifica o la rimozione del record DNS corrispondente compromette il recapito messaggi. Assicurati di eliminare la voce in Marketo prima di apportare modifiche DNS.

   Questo ti sarà di grande aiuto per il recapito dei messaggi e-mail. Dovresti ottenere la convalida che il record sia presente e corretto.
