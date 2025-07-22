---
description: Aggiungere l’accesso di Insight alle vendite ai profili - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere l’accesso di Sales Insight ai profili
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Aggiungi accesso [!DNL Sales Insight] ai profili {#add-sales-insight-access-to-profiles}

Ecco come creare un profilo con accesso a [!DNL Sales Insight] rimuovendo l&#39;accesso per gli altri profili. Questo è per gli utenti che hanno già installato il [[!DNL Sales Insight] pacchetto AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>Se in precedenza hai concesso a [!DNL Sales Insight] l&#39;accesso a tutti i profili, devi [rimuovere l&#39;accesso a livello di profilo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} per utilizzare questo set di autorizzazioni.

## Crea un nuovo profilo per [!DNL Sales Insight] {#create-a-new-profile-for-sales-insight}

Se disponi di un profilo dedicato per gli utenti di [!DNL Sales Insight], puoi saltare questo passaggio.

1. In [!DNL Salesforce], passare alla pagina Configurazione.

1. Cercare i profili in Ricerca rapida e selezionare l&#39;opzione **[!UICONTROL Profile]**.

1. Fare clic sul pulsante **[!UICONTROL New Profile]** nella parte superiore della pagina.

1. Selezionare un profilo da clonare e assegnargli un nome (ad esempio, Utente Insight vendite).

1. Al termine, fai clic su **[!UICONTROL Save]**.

## Aggiungi autorizzazioni [!DNL Sales Insight] {#add-sales-insight-permissions}

1. Torna all’elenco dei profili.

1. Fai clic sul collegamento **[!UICONTROL Edit]** per il nuovo profilo appena creato (o per qualsiasi altro profilo esistente a cui desideri concedere l&#39;accesso [!DNL Sales Insight]).

1. Nella pagina di modifica, dovrai modificare alcune impostazioni.

   **Per i profili a cui è consentito l&#39;accesso[!DNL Sales Insight]**:

   * In Impostazioni scheda, modifica le schede di Marketo in Attivato predefinito
   * In Autorizzazioni oggetto personalizzato, selezionare Lettura, Crea, Modifica ed Elimina nella configurazione [!DNL Marketo Sales Insight] (se l&#39;utente deve avere accesso alle impostazioni di configurazione, utilizzate in genere per gli amministratori)

   **Per i profili che non sono autorizzati ad accedere a[!DNL Sales Insight]**:

   * In Impostazioni scheda, modifica le schede di Marketo in Nascosto per scheda
   * In Autorizzazioni oggetto personalizzato, deselezionare Leggi, Crea, Modifica ed Elimina nella configurazione [!DNL Marketo Sales Insight]

1. Al termine, fai clic su **[!UICONTROL Save]**.

## Crea layout per [!DNL Sales Insight] {#create-layout-for-sales-insight}

1. Vai alla pagina di configurazione, quindi fai clic su **[!UICONTROL App Setup]** > **[!UICONTROL Customize]** > **[!UICONTROL Leads]** > **[!UICONTROL Page Layouts]**. Quindi fare clic sul pulsante **[!UICONTROL New]**.

1. Clonate il layout desiderato e assegnate al layout un nome appropriato, ad esempio Layout Insight vendite.

1. Al termine, fai clic su **[!UICONTROL Save]**.

1. Ripeti questi passaggi per i layout di pagina [!UICONTROL Contacts], [!UICONTROL Opportunities] e [!UICONTROL Accounts].

## Assegna profilo a layout {#assign-profile-to-layout}

1. Tornare alla sezione Layout di pagina e fare clic sul pulsante **[!UICONTROL Page Layout Assignment]**.

1. Seleziona **[!UICONTROL Edit Assignment]**.

1. Selezionare il profilo [!DNL Sales Insight] dall&#39;elenco, quindi selezionare il layout [!DNL Sales insight] dal menu a discesa &quot;[!UICONTROL Select Page Layout]&quot;.

1. Al termine, fai clic su **[!UICONTROL Save]**.

1. Ripeti questi passaggi per i layout di pagina [!UICONTROL Contacts], [!UICONTROL Opportunities] e [!UICONTROL Accounts].

## Altre modifiche {#other-changes}

Di seguito sono riportati alcuni altri punti in cui potrebbero essere visualizzati [!DNL Sales Insight] elementi. Dovrai rimuoverli subito poiché non puoi utilizzare i Profili per limitarne l’accesso:

* Rimuovi [!DNL Sales Insight] pulsanti dai layout di ricerca per [!UICONTROL Contacts], [!UICONTROL Leads] e [!UICONTROL Accounts]
* Rimuovi [!DNL Sales Insight] colonne dagli elenchi Contatti e Lead
