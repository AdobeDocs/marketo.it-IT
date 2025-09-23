---
description: Scadenza risorse locali - Documentazione Marketo - Documentazione del prodotto
title: Scadenza risorsa locale
exl-id: 603e3eee-0531-4139-a8f5-279831ad011f
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 4%

---

# Scadenza risorsa locale {#local-asset-expiration}

Imposta una data/ora di scadenza per annullare la pubblicazione delle pagine di destinazione, disattivare le campagne di attivazione o interrompere le campagne batch ricorrenti.

## Concedi autorizzazione scadenza cespite programmata {#grant-schedule-asset-expiration-permission}

Prima di poter pianificare la scadenza di una risorsa, il ruolo Marketo deve disporre dell’autorizzazione appropriata abilitata.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Nell&#39;area [!UICONTROL Admin] fare clic su **[!UICONTROL Users & Roles]**.

   ![](assets/local-asset-expiration-1.png)

1. Fare clic sulla scheda **[!UICONTROL Roles]**, selezionare l&#39;utente a cui si desidera concedere l&#39;accesso, quindi fare clic su **[!UICONTROL Edit Role]**.

   ![](assets/local-asset-expiration-2.png)

1. In [!UICONTROL Access Marketing Activities], seleziona **[!UICONTROL Schedule Local Asset Expiration]** e fai clic su **[!UICONTROL Save]**.

   ![](assets/local-asset-expiration-3.png)

## Impostare una data di scadenza {#set-an-expiration-date}

1. Fare clic con il pulsante destro del mouse sul programma desiderato e selezionare **[!UICONTROL Set local asset expiration]**.

   ![](assets/local-asset-expiration-4.png)

1. Controlla le risorse per le quali vuoi impostare una data di scadenza, quindi fai clic su **[!UICONTROL Set expiration]**.

   ![](assets/local-asset-expiration-5.png)

1. Scegli una data di scadenza.

   ![](assets/local-asset-expiration-6.png)

1. Imposta un orario. È necessario pianificare un orario di almeno 15 minuti in futuro (non dimenticare di immettere AM/PM). Al termine, fai clic su **[!UICONTROL Confirm]**.

   ![](assets/local-asset-expiration-7.png)

>[!NOTE]
>
>* Per modificare una data di scadenza esistente, controlla le risorse e fai clic su **[!UICONTROL Set expiration]**.
>* Una volta scaduta, una risorsa non viene più visualizzata sulla griglia di scadenza. Nella griglia vengono visualizzate solo le pagine di destinazione pubblicate, le campagne di attivazione attive e le campagne batch ricorrenti.
>* Le scadenze pianificate verranno rimosse se la risorsa viene spostata in un altro programma.

## Rimuovere una data di scadenza {#remove-an-expiration-date}

1. Per rimuovere una data di scadenza, controlla le risorse e fai clic su **[!UICONTROL Remove expiration]**.

   ![](assets/local-asset-expiration-8.png)

1. Verificare le risorse interessate, quindi fare clic su **[!UICONTROL Confirm]**.

   ![](assets/local-asset-expiration-9.png)

>[!NOTE]
>
>Non è possibile rimuovere date di scadenza entro i 15 minuti successivi. Per &quot;rimuovere&quot; la scadenza, devi attendere la scadenza della risorsa, quindi approvarla nuovamente o riattivarla.
