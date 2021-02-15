---
unique-page-id: 13796466
description: Guida introduttiva a Sales Connect - Marketo Docs - Documentazione prodotto
title: Guida introduttiva a Sales Connect
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---


# Guida introduttiva a Sales Connect {#getting-started-with-sales-connect}

Se preferisci seguire questi passaggi piuttosto che leggerli, passa direttamente alle [Istruzioni video riportate di seguito](#video).

>[!AVAILABILITY]
>
>Non tutti i clienti hanno acquistato questa funzionalità. Per ulteriori informazioni, contatta il tuo Customer Success Manager.

## Informazioni necessarie per iniziare {#what-you-need-to-get-started}

* Iscrizione Marketo
* Iscrizione a Sales Connect
* Iscrizione Salesforce (con le chiamate API e le classi Apex abilitate)

## Chi è necessario per iniziare {#who-you-need-to-get-started}

* Utente amministratore marketing
* Amministratore di Sales Connect
* Amministratore Salesforce
* Utenti di Sales Connect

## Amministratori Connect di vendita {#sales-connect-admins}

Riceverai un&#39;e-mail da Marketo con un collegamento per reimpostare la password. Dopo aver creato una nuova password, accedete a Sales Connect.

Per completare la configurazione, è necessario effettuare le seguenti operazioni:

* [Connect Sales Connect e Salesforce](#sfdc)
* [Acquisisci credenziali prima di collegare il collegamento delle vendite con Marketo](#acquire)
* [Connect Sales Connect con Marketo](#mkto)
* [Invita/Provisioning utenti](#IPU)

Facoltativamente, potete anche:

* [Test di Sales Connect nella sandbox](#sandbox)

## Collega l&#39;account di vendita a Salesforce {#connect-your-sales-connect-account-to-salesforce}

Per collegare il tuo account di Sales Connect al tuo account Salesforce, in qualità di Amministratore o non Amministratore, segui i passaggi descritti in [questo articolo](https://docs.marketo.com/x/JwDb).

>[!NOTE]
>
>L&#39;istanza di Salesforce a cui ci si connette deve essere la stessa istanza che è (o sarà) connessa a Marketo.

## Acquisizione delle credenziali prima della connessione di Sales Connect con Marketo {#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}

Dovrai ottenere una serie di credenziali da Marketo. Queste credenziali verranno utilizzate in seguito dall&#39;amministratore di Sales Connect per collegare Marketo con Sales Connect.

1. In Marketo, fare clic su **Admin**.

   ![](assets/one.png)

1. Nella struttura ad albero, fare clic su **Sales Connect**.

   ![](assets/two.png)

1. Seleziona e invia le seguenti credenziali Marketo all&#39;amministratore di Sales Connect: Munchkin ID, Client ID, Client Secret.

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >Quando copiate e incollate le informazioni di cui sopra, accertatevi che non vengano aggiunti spazi.

## Connetti alle vendite per Marketo {#connect-sales-connect-to-marketo}

1. In Sales Connect, fate clic sull&#39;icona a forma di ingranaggio e selezionate **Settings**.

   ![](assets/four.png)

1. In Impostazioni amministratore, seleziona **Marketo**.

   ![](assets/eight.png)

1. Immettete le credenziali Marketo fornite dall&#39;amministratore di Marketo e fate clic su **Connect**.

   ![](assets/credentials.png)

## Invita/Provisioning utenti {#invite-provision-users}

Se sul tuo account sono già presenti utenti (in precedenza da ToutApp), questi verranno visualizzati nella scheda **Accesso team** della sezione Marketo di Sales Connect.

Da questa pagina potete eseguire il provisioning del team come utente di Marketing Cloud Sales Connect. Se non avete mai utilizzato ToutApp o dovete ancora invitare gli utenti, seguite i passaggi descritti in [questo articolo](https://docs.marketo.com/display/TOUT/Invite+Team+Members).

>[!CAUTION]
>
>Attendere dieci minuti dalla connessione di Sales Connect con Marketo prima di eseguire questi passaggi.

1. Selezionate uno o più utenti, quindi fate clic su **Connect**.

   >[!NOTE]
   >
   >Potete eseguire l’assegnazione dell’area di lavoro solo una volta al momento di invitare gli utenti. Una volta impostato, sarà necessario disconnettere l&#39;utente per modificarlo.

   ![](assets/users.png)

1. Se l’iscrizione a Marketo include aree di lavoro abilitate, potrete assegnare aree di lavoro a ciascun utente o gruppo di utenti in gruppo. Se non è selezionata alcuna area di lavoro, verrà assegnata all’area di lavoro Marketo predefinito.

   ![](assets/nine.jpg)

1. Fate clic sul menu a discesa Area di lavoro, selezionate le aree di lavoro desiderate e fate clic su **Connect**.

   ![](assets/ten.png)

   >[!NOTE]
   >
   >Se desiderate aggiungere nuovi utenti, andate alla sezione Gestione team di Admin Settings e fate clic sul pulsante **Invita utenti**.

Puoi aggiungere altri utenti dalla pagina Gestione team e seguire i passaggi descritti sopra per collegarli.

## Test di Connect di vendita nella sandbox {#test-sales-connect-in-your-sandbox}

Per i team che desiderano sottoporre a test Marketo Sales Connect con la propria sandbox Marketo, è possibile effettuare il provisioning di un account aggiuntivo di Sales Connect su richiesta. Questo vale solo per i clienti che hanno acquistato una sandbox Marketo, o per quelli che la dispongono come parte del loro bundle Marketo. Se siete interessati ad acquisire una sandbox, contattate il vostro Account Manager Marketo.

>[!NOTE]
>
>Non potete fornire a più istanze un account di vendita Connect con lo stesso ID e-mail. Questo significa che se desiderate avere un account aggiuntivo di Sales Connect da verificare con l&#39;istanza di Marketing Sandbox, dovrete utilizzare un ID e-mail diverso in ciascuno degli account.
