---
unique-page-id: 13796466
description: Guida introduttiva a Sales Connect - Marketo Docs - Documentazione del prodotto
title: Guida introduttiva a Sales Connect
exl-id: 8c5b1f65-449c-4304-b904-fc6442a47e5a
translation-type: tm+mt
source-git-commit: 20ccc6ba2b26b869776ed88ed6fe76a67f74400a
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Guida introduttiva a Sales Connect {#getting-started-with-sales-connect}

Se preferisci guardare questi passaggi piuttosto che leggerli, passa direttamente alle [Istruzioni video qui sotto](#video).

>[!AVAILABILITY]
>
>Non tutti i clienti hanno acquistato questa funzionalità. Contatta il tuo Customer Success Manager per ulteriori informazioni.

## Informazioni necessarie per iniziare {#what-you-need-to-get-started}

* abbonamento Marketo
* Abbonamento a Sales Connect
* Abbonamento Salesforce (con chiamate API e classi Apex abilitate)

## Informazioni necessarie {#who-you-need-to-get-started}

* Utente amministratore Marketo
* Utente amministratore di Sales Connect
* Amministratore Salesforce
* Utenti di Sales Connect

## Amministratori di vendita Connect {#sales-connect-admins}

Riceverai un’e-mail da Marketo con un collegamento per reimpostare la password. Dopo aver creato una nuova password, accedi a Sales Connect.

Per completare la configurazione, è necessario effettuare le seguenti operazioni:

* [Connetti vendita e Salesforce](#connect-your-sales-connect-account-to-salesforce)
* [Acquisire le credenziali prima di collegare le vendite Connetti con Marketo](#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo)
* [Connetti le vendite a Marketo](#connect-sales-connect-to-marketo)
* [Invita/Provisioning utenti](#invite-provision-users)

Facoltativamente, puoi anche:

* [Test di vendita Connect nella sandbox](#test-sales-connect-in-your-sandbox)

## Collega il tuo account di vendita Connect a Salesforce {#connect-your-sales-connect-account-to-salesforce}

Per collegare il tuo account Sales Connect al tuo account Salesforce, in qualità di Amministratore o come non amministratore, segui i passaggi descritti in [questo articolo](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md).

>[!NOTE]
>
>L’istanza di Salesforce a cui ci si connette deve essere la stessa istanza che è (o sarà) connessa a Marketo.

## Acquisizione delle credenziali prima della connessione delle vendite Connetti con Marketo {#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}

Sarà necessario ottenere un set di credenziali da Marketo. Queste credenziali verranno utilizzate successivamente dall&#39;amministratore di Sales Connect per collegare Marketo a Sales Connect.

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/one.png)

1. Nella struttura fare clic su **Connetti vendite**.

   ![](assets/two.png)

1. Seleziona e invia le seguenti credenziali Marketo all&#39;amministratore di Sales Connect: ID Munchkin, ID client, segreto client.

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >Quando copi e incolla le informazioni di cui sopra, assicurati che non vengano aggiunti spazi.

## Connetti le vendite a Marketo {#connect-sales-connect-to-marketo}

1. In Sales Connect, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/four.png)

1. In Impostazioni amministratore, seleziona **Marketo**.

   ![](assets/eight.png)

1. Immetti le credenziali Marketo fornite dall&#39;amministratore Marketo e fai clic su **Connetti**.

   ![](assets/credentials.png)

## Invita/Provisioning utenti {#invite-provision-users}

Se sul tuo account sono già presenti utenti (precedentemente da ToutApp), questi verranno visualizzati nella scheda **Accesso al team** della sezione Marketo di Sales Connect.

È possibile eseguire il provisioning del team come utente Marketo Sales Connect da questa pagina. Se non hai mai utilizzato ToutApp o non hai ancora invitato gli utenti, segui i passaggi descritti in [questo articolo](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md).

>[!CAUTION]
>
>Attendere dieci minuti dopo aver collegato Sales Connect con Marketo prima di eseguire questi passaggi.

1. Seleziona uno o più utenti, quindi fai clic su **Connetti**.

   >[!NOTE]
   >
   >È possibile eseguire l&#39;assegnazione dell&#39;area di lavoro solo una volta al momento dell&#39;invito degli utenti. Una volta impostato, sarà necessario disconnettere l&#39;utente per modificarlo.

   ![](assets/users.png)

1. Se l’abbonamento a Marketo dispone di aree di lavoro abilitate, potrai assegnare aree di lavoro a ogni utente o set di utenti in blocco. Se non è selezionata alcuna area di lavoro, verranno assegnate all’area di lavoro Marketo predefinita.

   ![](assets/nine.jpg)

1. Fai clic sull&#39;elenco a discesa Area di lavoro, seleziona le aree di lavoro desiderate e fai clic su **Connetti**.

   ![](assets/ten.png)

   >[!NOTE]
   >
   >Se desideri aggiungere nuovi utenti, vai alla sezione Gestione team di Impostazioni amministratore e fai clic sul pulsante **Invita utenti** .

Puoi aggiungere altri utenti dalla pagina Gestione team e seguire i passaggi descritti sopra per collegarli.

## Test di vendita Connetti alla sandbox {#test-sales-connect-in-your-sandbox}

Per i team che desiderano testare Marketo Sales Connect con la propria Sandbox Marketo, è possibile effettuare il provisioning di un account aggiuntivo Sales Connect su richiesta. Questo vale solo per i clienti che hanno acquistato una Sandbox Marketo o per quelli che la hanno come parte del loro bundle Marketo. Se sei interessato ad acquisire un Sandbox, contatta il tuo Marketo Account Manager.

>[!NOTE]
>
>Non è possibile fornire a più istanze un account Sales Connect con lo stesso ID e-mail. Ciò significa che se desideri avere un account di vendita Connect aggiuntivo da testare con la tua istanza Sandbox di Marketo, dovrai utilizzare un ID e-mail diverso in ciascuno degli account.
