---
unique-page-id: 10096683
description: Aggiornamenti alla registrazione di eventi ON24 - Documentazione di Marketo - Documentazione del prodotto
title: Aggiornamenti alla registrazione dell'evento ON24
exl-id: 1d194ef2-b6ca-4e2d-b476-beb5bccd3c5f
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Aggiornamenti alla registrazione dell&#39;evento ON24 {#on-event-registration-updates}

## Approvazione manuale dei dichiaranti {#manually-approving-registrants}

Puoi approvare manualmente i tuoi iscritti prima di inviare loro un messaggio e-mail di conferma. A tal fine, dovrai configurare le campagne per gestire questo passaggio aggiuntivo:

1. Per la campagna Trigger registrazione:

   * In [!UICONTROL Smart List], impostare il trigger su **[!UICONTROL Fills Out Form]**.
   * Nel flusso, impostare [!UICONTROL Status in Progression] su **[!UICONTROL Pending Approval]**.

1. Passare all&#39;evento e fare clic sulla scheda **[!UICONTROL Members]**. In questa scheda vengono visualizzate tutte le persone che hanno compilato il modulo. Il loro stato deve essere impostato su **[!UICONTROL Pending Approval]**.
1. Utilizzare il filtro nella parte superiore della griglia per visualizzare solo le persone con stato **[!UICONTROL Pending Approval]**.
1. Selezionare le persone da registrare (Maiusc-clic, Ctrl-clic o Seleziona tutto).
1. Scegliere **[!UICONTROL Change Status]** dal menu. Selezionare **[!UICONTROL Registered]**, **[!UICONTROL Rejected]** o qualsiasi altro stato applicabile.

## Gestione delle persone con un errore di registrazione {#handling-people-with-a-registration-error}

Se una persona alla fine non viene registrata, ma impostata sullo stato [!UICONTROL Registration Error], non è troppo tardi per il ripristino.

1. Dalla scheda [!UICONTROL Members], filtra l&#39;elenco di persone con lo stato **[!UICONTROL Registration Error]**.
1. Prima di continuare, accertati di aver determinato e risolto il problema con l&#39;integrazione (verifica che non vi siano errori in **[!UICONTROL Event Partners]** in Admin).
1. Una volta risolto il problema, selezionare tutte le persone con lo stato [!UICONTROL Registration Error] e cambiarne lo stato in **[!UICONTROL Registered]**. Verrà eseguito un nuovo tentativo di registrazione con ON24.

## Aggiornamento dello stato del membro da ON24 {#updating-member-status-from-on}

Marketo richiama automaticamente le informazioni sulla frequenza alle 23:00 circa (Pacifico) di ogni notte. Per aggiornare manualmente le informazioni sulle presenze, fare clic su **[!UICONTROL Refresh from Webinar Provider]** in **[!UICONTROL Event Actions]**.

>[!MORELIKETHIS]
>
>[Informazioni sugli eventi della scheda di rete Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
