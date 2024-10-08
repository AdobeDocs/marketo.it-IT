---
description: Passaggio 2 di 4 - Configurare la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa - Documenti Marketo - Documentazione del prodotto
title: Passaggio 2 di 4 - Configurare la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
feature: Microsoft Dynamics
source-git-commit: 2eb61d43f2f470d42e1b50ab8edc99e4e25c23cf
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Passaggio 2 di 4: configurare la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa {#step-2-of-4-set-up-the-marketo-solution-ropc}

Iniziamo creando un account utente.

>[!PREREQUISITES]
>
>[Passaggio 1 di 4: installare la soluzione Marketo con la connessione di controllo password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}

## Crea un nuovo utente {#create-a-new-user}

1. Accedi a Dynamics. Fai clic sull&#39;icona Impostazioni e seleziona **[!UICONTROL Impostazioni avanzate]**.

   ![](assets/one.png)

1. Fare clic su **[!UICONTROL Impostazioni]** e selezionare **[!UICONTROL Sicurezza]**.

   ![](assets/two.png)

1. Fare clic su **[!UICONTROL Utenti]**.

   ![](assets/three.png)

1. Fare clic su **[!UICONTROL Nuovo]**.

   ![](assets/four.png)

1. Fare clic su **[!UICONTROL Aggiungi e concedi la licenza agli utenti]** nella nuova finestra.

   ![](assets/five.png)

1. Viene visualizzata una nuova scheda. Fai clic su **[!UICONTROL Amministratore]** nella parte superiore della pagina.

   ![](assets/six.png)

1. Viene visualizzata un’altra nuova scheda. Fare clic su **[!UICONTROL Aggiungi un utente]**.

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >L&#39;utente Sync deve disporre dell&#39;autorizzazione di lettura per la configurazione di Marketo.

1. Immettere tutte le informazioni. Al termine, fare clic su **[!UICONTROL Aggiungi]**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Questo nome deve essere un utente di sincronizzazione dedicato e non un account utente CRM esistente. Non deve essere un indirizzo e-mail effettivo.

1. Immetti l&#39;indirizzo e-mail per ricevere le nuove credenziali utente e fai clic su **[!UICONTROL Invia e-mail e chiudi]**.

   ![](assets/nine.png)

## Assegna ruolo utente di sincronizzazione {#assign-sync-user-role}

Assegnare il ruolo Utente di sincronizzazione Marketo solo all&#39;utente di sincronizzazione Marketo. Non è necessario assegnarla ad altri utenti.

>[!NOTE]
>
>Questo vale per Marketo versione 4.0.0.14 e successive. Per le versioni precedenti, tutti gli utenti devono avere il ruolo utente di sincronizzazione. Per aggiornare Marketo, vedere [Aggiorna soluzione Marketo per Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>L&#39;impostazione della lingua dell&#39;utente di sincronizzazione [ deve essere inglese](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Torna alla scheda **[!UICONTROL Utenti abilitati]** e aggiorna l&#39;elenco degli utenti.

   ![](assets/ten.png)

1. Passa il puntatore del mouse accanto al nuovo utente di Marketo Sync creato, quindi viene visualizzata una casella di controllo. Fai clic su per selezionarlo.

   ![](assets/eleven.png)

1. Fai clic su **[!UICONTROL Gestisci ruoli]**.

   ![](assets/twelve.png)

1. Controlla **[!UICONTROL Utente Marketo Sync]** e fai clic su **[!UICONTROL OK]**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Eventuali aggiornamenti apportati nel CRM dall&#39;utente di sincronizzazione _non_ verranno sincronizzati di nuovo in Marketo.

## Configurare la soluzione Marketo {#configure-marketo-solution}

Ci siamo quasi! Tutto ciò che ci rimane è informare Marketo Solution sul nuovo utente creato.

1. Torna alla sezione Impostazioni avanzate e fai clic sull&#39;icona ![](assets/image2015-5-13-15-3a49-3a19.png) accanto a Impostazioni, quindi seleziona **[!UICONTROL Configurazione Marketo]**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Se non vedi **[!UICONTROL Configurazione Marketo]** nel menu Impostazioni, aggiorna la pagina. Se non funziona, prova a [pubblicare di nuovo la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"} oppure esci e accedi di nuovo.

1. Fare clic su **[!UICONTROL Predefinito]**.

   ![](assets/fifteen.png)

1. Fai clic sul pulsante Cerca nel campo **[!UICONTROL Utente Marketo]** e seleziona l&#39;utente di sincronizzazione creato.

   ![](assets/sixteen.png)

1. Fai clic sull&#39;icona ![](assets/image2015-3-13-15-3a10-3a11.png) nell&#39;angolo in basso a destra per salvare le modifiche.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Fai clic su **X** in alto a destra per chiudere la schermata.

   ![](assets/seventeen.png)

1. Fai clic sull&#39;icona ![](assets/image2015-5-13-15-3a49-3a19-1.png) accanto a Impostazioni e seleziona **[!UICONTROL Soluzioni]**.

   ![](assets/eighteen.png)

1. Fai clic sul pulsante **[!UICONTROL Tutte le personalizzazioni di Publish]**.

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[Passaggio 3 di 4: connettere la soluzione Marketo con la connessione di controllo password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}
