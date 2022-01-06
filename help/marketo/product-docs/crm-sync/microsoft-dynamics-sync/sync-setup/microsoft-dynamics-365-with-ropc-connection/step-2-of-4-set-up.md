---
unique-page-id: 3571827
description: Passaggio 2 di 3 - Configurare la soluzione Marketo con la connessione Controllo password proprietario risorsa - Marketo Docs - Documentazione del prodotto
title: 'Passaggio 2 di 3: configurare la soluzione Marketo con la connessione per il controllo della password del proprietario della risorsa'
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
source-git-commit: 8b4d86f2dd5f19abb56451403cd2638b1a852d79
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Passaggio 2 di 3: Configurare la soluzione Marketo con la connessione Controllo password proprietario risorsa {#step-2-of-3-set-up-the-marketo-solution-ropc}

Cominciamo creando un account utente.

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: Installare la soluzione Marketo con la connessione Controllo password proprietario risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)

## Crea un nuovo utente {#create-a-new-user}

1. Accedi a Dynamics. Fai clic sull’icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Fai clic su **Impostazioni** e seleziona **Sicurezza**.

   ![](assets/two.png)

1. Fai clic su **Utenti**.

   ![](assets/three.png)

1. Fai clic su **Novità.**

   ![](assets/four.png)

1. Fai clic su **Aggiungere e concedere licenze agli utenti** nella nuova finestra.

   ![](assets/five.png)

1. Viene visualizzata una nuova scheda. Fai clic su **Amministratore** nella parte superiore della pagina.

   ![](assets/six.png)

1. Viene visualizzata un’altra nuova scheda. Fai clic su **Aggiungi un utente**.

   ![](assets/seven.png)

1. Inserisci tutte le informazioni. Al termine, fai clic su **Aggiungi**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Questo nome deve essere un utente di sincronizzazione dedicato e non un account utente CRM esistente. Non deve essere un indirizzo e-mail effettivo.

1. Immetti l’e-mail per ricevere le nuove credenziali utente e fai clic su **Invia e-mail e chiudi**.

   ![](assets/nine.png)

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegna il ruolo utente di sincronizzazione Marketo solo all&#39;utente di sincronizzazione Marketo. Non è necessario assegnarlo ad altri utenti.

>[!NOTE]
>
>Questo vale per la versione 4.0.0.14 e successive di Marketo. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare Marketo, vedi [Aggiornare la soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Impostazione della lingua dell&#39;utente di sincronizzazione [deve essere impostato su Inglese](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Torna alla scheda Utenti abilitati e aggiorna l’elenco degli utenti.

   ![](assets/ten.png)

1. Passa il puntatore del mouse accanto all’utente Marketo Sync appena creato e viene visualizzata una casella di controllo. Fai clic su per selezionarlo.

   ![](assets/eleven.png)

1. Fai clic su **Gestisci ruoli**.

   ![](assets/twelve.png)

1. Controlla **Marketo Sync User** e fai clic su **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Eventuali aggiornamenti effettuati nel CRM dall&#39;utente di sincronizzazione verranno **not** essere sincronizzati di nuovo in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi lì! Tutto quello che ci rimane è quello di informare Marketo Solution sul nuovo utente creato.

1. Torna alla sezione Impostazioni avanzate e fai clic su ![](assets/image2015-5-13-15-3a49-3a19.png) accanto a Impostazioni e seleziona **Configurazione Marketo**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Se non vedi **Configurazione Marketo** nel menu Impostazioni , aggiorna la pagina. Se non funziona, prova a [pubblicare la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) di nuovo o disconnettiti e accedi di nuovo.

1. Fai clic su **Predefinito**.

   ![](assets/fifteen.png)

1. Fai clic sul pulsante di ricerca nel **Utente Marketo** e seleziona l’utente di sincronizzazione creato.

   ![](assets/sixteen.png)

1. Fai clic sul pulsante ![](assets/image2015-3-13-15-3a10-3a11.png) nell’angolo in basso a destra per salvare le modifiche.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Fai clic sul pulsante **X** in alto a destra per chiudere lo schermo.

   ![](assets/seventeen.png)

1. Fai clic sul pulsante ![](assets/image2015-5-13-15-3a49-3a19-1.png) accanto a Impostazioni e seleziona **Soluzioni**.

   ![](assets/eighteen.png)

1. Fai clic sul pulsante **Pubblica tutte le personalizzazioni** pulsante .

   ![](assets/nineteen.png)

## Prima di procedere al passaggio 3 {#before-proceeding-to-step}

    * Per limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ora.
    * Esegui il processo [Validate Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) . Verifica che le impostazioni iniziali siano state eseguite correttamente.
    * Accedi all’utente di sincronizzazione Marketo in Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Passaggio 3 di 3: Connessione della soluzione Marketo con la connessione del controllo password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)
