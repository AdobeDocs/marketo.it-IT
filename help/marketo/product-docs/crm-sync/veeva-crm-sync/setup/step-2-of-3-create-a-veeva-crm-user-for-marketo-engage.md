---
description: Passaggio 2 di 3 - Creazione di un utente CRM Veeva per il Marketo Engage - Documentazione Marketo - Documentazione del prodotto
title: Passaggio 2 di 3 - Creazione di un utente Veeva CRM per il Marketo Engage
exl-id: 78945192-36b0-4e0b-830a-f37eb0b83484
feature: Veeva CRM
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 4%

---

# Passaggio 2 di 3: creazione di un utente Veeva CRM per il Marketo Engage {#step-2-of-3-create-a-veeva-crm-user-for-marketo-engage}

>[!NOTE]
>
>I passaggi descritti in questo articolo devono essere completati da un amministratore CRM Veeva.

>[!PREREQUISITES]
>
>[Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Professional)](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target="_blank"}

In questo articolo personalizzerai le autorizzazioni del campo con un layout di pagina CRM Veeva e creerai un utente di sincronizzazione CRM Marketo-Veeva.

## Imposta layout di pagina {#set-page-layouts}

La procedura seguente consente all&#39;utente di Marketo Sync di aggiornare i campi personalizzati.

1. Fare clic sui layout di pagina Account (account persona) nella barra di ricerca di navigazione senza premere Invio, quindi fare clic su **[!UICONTROL Layout di pagina]** in Contatti.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. Fare clic su **[!UICONTROL Layout di pagina]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. Fare clic su **[!UICONTROL HCP - Professional]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. Fai clic su e trascina una nuova **[!UICONTROL sezione]** nel layout della pagina.

1. Immettere &quot;Marketo&quot; per Nome sezione e fare clic su **[!UICONTROL OK]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. Fai clic su e trascina il campo Punteggio nella sezione Marketo.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-5.png)

1. Ripeti il passaggio precedente per i campi seguenti:

   * Città dedotta
   * Azienda in oggetto
   * Paese in oggetto
   * Area metropolitana dedotta
   * Prefisso telefonico dedotto
   * Codice postale dedotto
   * Area geografica dello stato dedotta

   >[!NOTE]
   >
   >Questi campi devono trovarsi nel layout di pagina in modo che Marketo possa leggerli/scrivervi.

   >[!TIP]
   >
   >Per creare due colonne per i campi, trascinare verso il basso il lato destro della pagina. È possibile spostare i campi da un lato all&#39;altro per bilanciare la lunghezza delle colonne.

1. Al termine, fare clic su **[!UICONTROL Salva]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

   >[!NOTE]
   >
   >Ripetere l&#39;operazione per altri layout della pagina Account.

## Creare un profilo {#create-a-profile}

1. Fare clic su **[!UICONTROL Configurazione]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. Digita &quot;profiles&quot; nella barra di ricerca di navigazione e fai clic sul collegamento **[!UICONTROL Profili]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. Fare clic su **[!UICONTROL Nuovo]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. Seleziona Utente Standard, denomina il profilo &quot;Marketo-Salesforce Sync&quot; e fai clic su **[!UICONTROL Salva]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## Imposta autorizzazioni profilo {#set-profile-permissions}

1. Fai clic su **[!UICONTROL Modifica]** per impostare le autorizzazioni di protezione.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. Nella sezione Autorizzazioni amministrative, assicurati che sia selezionato **[!UICONTROL API Enabled]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >Seleziona la casella Password Never Expires (Password senza scadenza).

1. Nella sezione Autorizzazioni utente generali, assicurati che siano selezionati **[!UICONTROL Modifica eventi]** e **[!UICONTROL Modifica attività]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. Nella sezione Autorizzazioni oggetto standard, assicurati che le autorizzazioni **[!UICONTROL Lettura]**, **[!UICONTROL Creazione]**, **[!UICONTROL Modifica]** e **[!UICONTROL Elimina]** siano verificate per account e contatti.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. Nella sezione Autorizzazioni oggetto personalizzato verificare che le autorizzazioni di lettura siano verificate per **[!UICONTROL Chiamata]**, **[!UICONTROL Messaggio chiave chiamata]** e per qualsiasi altro oggetto personalizzato desiderato.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. Al termine, fare clic su **[!UICONTROL Salva]** nella parte inferiore della pagina.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## Imposta autorizzazioni campo {#set-field-permissions}

1. Rivolgiti ai tuoi esperti di marketing per scoprire quali campi personalizzati sono necessari per la sincronizzazione.

   >[!NOTE]
   >
   >Questo passaggio impedisce la visualizzazione dei campi non necessari in Marketo, riducendo il disordine e velocizzando la sincronizzazione.

1. Nella pagina dei dettagli del profilo, vai alla sezione [!UICONTROL Sicurezza a livello di campo]. Fare clic su **[!UICONTROL Visualizza]** per modificare l&#39;accessibilità per gli oggetti Contatto e Account.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

   >[!TIP]
   >
   >Puoi configurare altri oggetti in base alle esigenze della tua organizzazione.

1. Per ogni oggetto, fare clic su **[!UICONTROL Modifica]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

1. Individuare i campi non necessari, assicurarsi che Accesso in lettura e Accesso in modifica siano _deselezionati_. Al termine, fai clic su **[!UICONTROL Salva]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

   >[!NOTE]
   >
   >Modifica solo l’accessibilità per i campi personalizzati.

1. Dopo aver disattivato tutti i campi non necessari, selezionare Accesso in lettura e Accesso in modifica per i campi oggetto seguenti. Al termine, fai clic su **[!UICONTROL Salva]**.

<table>
 <tbody>
  <tr>
   <th>Oggetto
   <th>Campi
  </tr>
  <tr>
   <td>Account</td>
   <td>Campo tipo</td>
  </tr>
  <tr>
   <td>Evento</td>
   <td>Tutti i campi</td>
  </tr>
  <tr>
   <td>Attività</td>
   <td>Tutti i campi</td>
  </tr>
 </tbody>
</table>

## Crea utente di sincronizzazione {#create-sync-user}

Marketo richiede le credenziali per accedere a Veeva CRM. Questa operazione può essere eseguita con un utente dedicato creato con i passaggi seguenti.

>[!NOTE]
>
>Se la tua organizzazione non dispone di licenze CRM aggiuntive per Veeva, puoi utilizzare un utente Marketing esistente con il profilo Amministratore di sistema.

1. Immetti &quot;users&quot; (Utenti) nella barra di ricerca di navigazione e fai clic su **[!UICONTROL Users]** in Manage Users (Gestisci utenti).

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. Fare clic su **[!UICONTROL Nuovo utente]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. Compila i campi obbligatori, seleziona la Licenza utente: Salesforce, imposta il profilo: Utente Marketo Sync e fai clic su **[!UICONTROL Salva]**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>Verifica che l’indirizzo e-mail inserito sia valido. Per reimpostare la password è necessario accedere come utente di sincronizzazione.

Eccellente! Ora hai un account che il Marketo Engage può utilizzare per connettersi a Veeva CRM. Facciamolo.

>[!MORELIKETHIS]
>
>[Passaggio 3 di 3: connettere Marketo e Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target="_blank"}
