---
unique-page-id: 3571827
description: 'Passaggio 2 di 3: configurare Marketo Sync User in Dynamics - Marketo Docs - Documentazione del prodotto'
title: 'Passaggio 2 di 3: configurare Marketo Sync User in Dynamics'
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Passaggio 2 di 3: Configurazione dell’utente di sincronizzazione Marketo in Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}

Cominciamo creando un account utente.

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: Installare la soluzione Marketo (online)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)

## Crea un nuovo utente {#create-a-new-user}

1. Accedi a Dynamics. Fai clic sull&#39;icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Fare clic su **Impostazioni** e selezionare **Protezione**.

   ![](assets/two.png)

1. Fare clic su **Utenti**.

   ![](assets/three.png)

1. Fare clic su **Nuovo.**

   ![](assets/four.png)

1. Fai clic su **Aggiungi e rilascia la licenza agli utenti** nella nuova finestra.

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

1. Immetti l&#39;e-mail per ricevere le nuove credenziali utente e fai clic su **Invia e-mail e chiudi**.

   ![](assets/nine.png)

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegna il ruolo utente di sincronizzazione Marketo solo all&#39;utente di sincronizzazione Marketo. Non è necessario assegnarlo ad altri utenti.

>[!NOTE]
>
>Questo vale per la versione 4.0.0.14 e successive di Marketo. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare Marketo, consulta [Aggiornare la soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

1. Torna alla scheda Utenti abilitati e aggiorna l’elenco degli utenti.

   ![](assets/ten.png)

1. Passa il puntatore del mouse accanto all’utente Marketo Sync appena creato e viene visualizzata una casella di controllo. Fai clic su per selezionarlo.

   ![](assets/eleven.png)

1. Fare clic su **Gestisci ruoli**.

   ![](assets/twelve.png)

1. Controlla **Marketo Sync User** e fai clic su **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Eventuali aggiornamenti effettuati nel CRM dall&#39;utente di sincronizzazione **non** verranno sincronizzati nuovamente in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi lì! Tutto quello che ci rimane è quello di informare Marketo Solution sul nuovo utente creato.

1. Torna alla sezione Impostazioni avanzate e fai clic sull&#39;icona ![](assets/image2015-5-13-15-3a49-3a19.png) accanto a Impostazioni e seleziona **Configurazione Marketo**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Se non trovi **Configurazione Marketo** nel menu Impostazioni, aggiorna la pagina. Se questo non funziona, prova a [pubblicare nuovamente la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) oppure disconnettiti e accedi di nuovo.

1. Fare clic su **Predefinito**.

   ![](assets/fifteen.png)

1. Fai clic sul pulsante di ricerca nel campo **Marketo User** e seleziona l&#39;utente di sincronizzazione che hai creato.

   ![](assets/sixteen.png)

1. Fai clic sull’icona ![](assets/image2015-3-13-15-3a10-3a11.png) nell’angolo in basso a destra per salvare le modifiche.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Fai clic su **X** in alto a destra per chiudere lo schermo.

   ![](assets/seventeen.png)

1. Fai clic sull&#39;icona ![](assets/image2015-5-13-15-3a49-3a19-1.png) accanto a Impostazioni e seleziona **Soluzioni**.

   ![](assets/eighteen.png)

1. Fai clic sul pulsante **Pubblica tutte le personalizzazioni** .

   ![](assets/nineteen.png)

## Prima di procedere al passaggio 3 {#before-proceeding-to-step}

    * Se desideri limitare il numero di record sincronizzati, ora [imposta un filtro di sincronizzazione personalizzato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
    * Esegui il processo [Validate Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) . Verifica che le impostazioni iniziali siano state eseguite correttamente.
    * Accedi all&#39;utente di sincronizzazione Marketo in Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Passaggio 3 di 3: Connettere Microsoft Dynamics con Marketo (online)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md)
