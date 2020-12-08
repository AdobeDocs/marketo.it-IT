---
unique-page-id: 3571827
description: Passaggio 2 di 3 - Imposta Marketo Sync User in Dynamics - Marketo Docs - Documentazione prodotto
title: Passaggio 2 di 3 - Configurare Marketo Sync User in Dynamics
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Passaggio 2 di 3: Impostazione di Marketo Sync User in Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}

Cominciamo con la creazione di un account utente.

>[!NOTE]
>
>**Prerequisiti**
>
>[Passaggio 1 di 3: Installazione della soluzione Marketo (online)](step-1-of-3-install.md)

## Creare un nuovo utente {#create-a-new-user}

1. Accedi a Dynamics. Fate clic sull&#39;icona Impostazioni e selezionate Impostazioni **avanzate**.

   ![](assets/one.png)

1. Fare clic su** Settings** e selezionare **Security**.

   ![](assets/two.png)

1. Fate clic su **Utenti**.

   ![](assets/three.png)

1. Fate clic su **Nuovo.**

   ![](assets/four.png)

1. Fate clic su **Aggiungi utenti** e ottieni la licenza nella nuova finestra.

   ![](assets/five.png)

1. Si apre una nuova scheda. Fate clic su **Admin** nella parte superiore della pagina.

   ![](assets/six.png)

1. Si apre un&#39;altra nuova scheda. Fate clic su **Aggiungi un utente**.

   ![](assets/seven.png)

1. Immettete tutte le informazioni. Al termine, fate clic su **Aggiungi**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Questo nome deve essere un utente di sincronizzazione dedicato e non un account utente CRM esistente. Non deve essere un indirizzo e-mail effettivo.

1. Inserite il messaggio e-mail per ricevere le nuove credenziali utente e fate clic su **Invia e-mail e chiudete**.

   ![](assets/nine.png)

## Assegna ruolo utente sincronizzazione {#assign-sync-user-role}

Assegnate il ruolo di sincronizzazione utente Marketo solo all’utente di sincronizzazione Marketo. Non è necessario assegnarlo ad altri utenti.

>[!NOTE]
>
>Questo vale per Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo di utente di sincronizzazione. Per aggiornare Marketo, consulta [Aggiornamento della soluzione Marketo per Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Tornate alla scheda Utenti abilitati e aggiornate l&#39;elenco degli utenti.

   ![](assets/ten.png)

1. Passate il puntatore del mouse accanto all’utente Marketing Cloud appena creato per la sincronizzazione, quindi compare una casella di controllo. Fate clic per selezionarlo.

   ![](assets/eleven.png)

1. Fate clic su **Gestisci ruoli**.

   ![](assets/twelve.png)

1. Selezionate **Marketo per sincronizzare l’utente** e fate clic su **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Eventuali aggiornamenti apportati in CRM dall&#39;utente di sincronizzazione **non** verranno sincronizzati di nuovo su Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Quasi lì! Ci resta solo da informare Marketo Solution sul nuovo utente creato.

1. Tornate alla sezione Impostazioni avanzate e fate clic sull&#39; ![](assets/image2015-5-13-15-3a49-3a19.png)icona accanto a Impostazioni, quindi selezionate **Configurazione** marketing.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Se non trovi **Configurazione** Marketo nel menu Impostazioni, aggiorna la pagina. Se questo non funziona, prova a [pubblicare di nuovo la soluzione](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) [](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) Marketo oppure disconnettiti ed effettua nuovamente l&#39;accesso.

1. Fate clic su **Predefinito**.

   ![](assets/fifteen.png)

1. Fate clic sul pulsante di ricerca nel campo **Marketing User** (Utente marketing) e selezionate l&#39;utente di sincronizzazione che avete creato.

   ![](assets/sixteen.png)

1. Fate clic sull’ ![](assets/image2015-3-13-15-3a10-3a11.png)icona nell’angolo in basso a destra per salvare le modifiche.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Fate clic sulla **X** in alto a destra per chiudere lo schermo.

   ![](assets/seventeen.png)

1. Fate clic sull&#39; ![](assets/image2015-5-13-15-3a49-3a19-1.png)icona accanto a Impostazioni, quindi selezionate **Soluzioni**.

   ![](assets/eighteen.png)

1. Fate clic sul pulsante **Pubblica tutte le personalizzazioni** .

   ![](assets/nineteen.png)

## Prima di procedere allo stadio 3 {#before-proceeding-to-step}

    * Se si desidera limitare il numero di record sincronizzati, [impostare un filtro di sincronizzazione personalizzato](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) ora.
    * Eseguire il processo [Validate Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Verifica che le impostazioni iniziali siano state eseguite correttamente.
    * Accedere all&#39;utente di sincronizzazione Marketo in Microsoft Dynamics CRM.

>[!NOTE]
>
>**Articoli correlati**
>
>
>[Passaggio 3 di 3: Connetti Microsoft Dynamics con Marketo (online)](step-3-of-3-connect.md)
