---
unique-page-id: 14746470
description: Impostazione di un canale di consegna personalizzato - Documenti Marketo - Documentazione del prodotto
title: Impostazione di un canale di consegna personalizzato
exl-id: a31f7bfd-a4ee-4948-9bdc-b49d47054d40
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Impostazione di un canale di consegna personalizzato {#setting-up-a-custom-delivery-channel}

Marketo Sales Connect consente di integrarsi con un server SMTP personalizzato per la consegna delle e-mail. Questa è una grande opzione per coloro che non desiderano inviare e-mail in blocco dal proprio canale di consegna Gmail o Exchange.

Gli utenti possono impostare un server SMTP personalizzato per il proprio utilizzo, oppure gli amministratori possono impostare un SMTP del team da condividere tra tutti gli utenti di Sales Connect della tua istanza.

>[!NOTE]
>
>* Oltre a configurare il server SMTP, [l’identità e-mail deve essere verificata](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) prima di poter inviare e-mail.
>* È consigliabile collaborare con il team IT o il fornitore del server SMTP per ottenere le credenziali corrette per il server SMTP.
>* Non è possibile collegare il server Gmail ed Exchange utilizzando le credenziali del server SMTP. Utilizza il nostro servizio di connessione e-mail per integrarsi con questi provider.


## SMTP personalizzato {#custom-smtp}

1. Accedi a [applicazione web](https://toutapp.com/login), fai clic sull’icona a forma di ingranaggio in alto a destra e scegli **Impostazioni**.

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. In Il mio account, fai clic su **Impostazioni e-mail**.

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. Fai clic su **Canale di consegna personalizzato**.

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. Immetti le credenziali del server SMTP e fai clic su **Connetti**.

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >Se questo è il tuo unico canale di consegna, viene automaticamente assegnato a tutte le tue identità e-mail, e hai finito qui. Se questo non è l&#39;unico canale di consegna, continua a seguire il passaggio 5.

1. Sempre in Impostazioni e-mail, fai clic su **Indirizzo e firma**.

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. Trova l’identità e-mail per la quale desideri scegliere un canale di consegna e fai clic su **Scegli il canale di consegna**.

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. Nella scheda Consegna, fai clic su **Modifica**.

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. Fai clic sull’elenco a discesa Canale e scegli il canale di consegna personalizzato appena aggiunto. Fai clic su **Salva**.

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >Se l’amministratore del team imposta il server SMTP del team, questo verrà automaticamente applicato solo all’identità e-mail predefinita e sarà disponibile come opzione per le altre identità e-mail.

## Server SMTP del team {#team-smtp-server}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Accedi a [applicazione web](https://toutapp.com/login), fai clic sull’icona a forma di ingranaggio in alto a destra e scegli **Impostazioni**.

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. In Impostazioni amministratore, fai clic su **Generale**.

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. Fai clic su **Canale di consegna team**.

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. Immetti le credenziali del server SMTP e fai clic su **Connetti**.

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >Il server SMTP del team sarà il canale di consegna predefinito dell&#39;identità e-mail predefinita per tutti i membri del team. Inoltre, sarà disponibile come opzione del canale di consegna per tutte le altre identità e-mail.

   >[!MORELIKETHIS]
   >
   >* [Connessione e-mail per utenti Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
   >
   >* [Connessione e-mail per utenti di Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

