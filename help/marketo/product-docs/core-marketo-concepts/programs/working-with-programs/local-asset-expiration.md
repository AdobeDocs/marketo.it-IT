---
description: Scadenza risorse locali - Documenti Marketo - Documentazione del prodotto
title: Scadenza risorse locali
exl-id: 603e3eee-0531-4139-a8f5-279831ad011f
source-git-commit: 48a49faa6a1fde1e9ac391c2bf0800123f6a5bac
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Scadenza risorse locali {#local-asset-expiration}

Imposta una data/ora di scadenza per annullare la pubblicazione delle pagine di destinazione, disattivare l’attivazione delle campagne o interrompere le campagne batch ricorrenti.

## Autorizzazione per la scadenza della risorsa della pianificazione {#grant-schedule-asset-expiration-permission}

Prima di pianificare la scadenza di una risorsa, è necessario che il ruolo Marketo disponga dell’autorizzazione appropriata abilitata.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. In [!UICONTROL Admin] area, fai clic su **[!UICONTROL Users & Roles]**.

   ![](assets/local-asset-expiration-1.png)

1. Fai clic sul pulsante **[!UICONTROL Roles]** selezionare l&#39;utente a cui si desidera concedere l&#39;accesso, quindi fare clic su **[!UICONTROL Edit Role]**.

   ![](assets/local-asset-expiration-2.png)

1. Sotto [!UICONTROL Access Marketing Activities], seleziona **[!UICONTROL Schedule Local Asset Expiration]** e fai clic su **[!UICONTROL Save]**.

   ![](assets/local-asset-expiration-3.png)

## Imposta una data di scadenza {#set-an-expiration-date}

1. Fai clic con il pulsante destro del mouse sul programma desiderato e seleziona **[!UICONTROL Set Local Asset Expiration]**.

   ![](assets/local-asset-expiration-4.png)

1. Controlla le risorse per le quali vuoi impostare una data di scadenza, quindi fai clic su **[!UICONTROL Set Expiration]**.

   ![](assets/local-asset-expiration-5.png)

1. Scegli una data di scadenza.

   ![](assets/local-asset-expiration-6.png)

1. Imposta un&#39;ora. È necessario pianificare un orario di almeno 20 minuti in futuro (non dimenticare di inserire AM/PM). Fai clic su **[!UICONTROL Confirm]** al termine.

   ![](assets/local-asset-expiration-7.png)

>[!NOTE]
>
>* Per modificare una data di scadenza esistente, controlla semplicemente le risorse e fai clic su **[!UICONTROL Set Expiration]**.
>* Una volta scaduta, la risorsa non verrà più visualizzata nella griglia di scadenza. La griglia visualizza solo le pagine di destinazione pubblicate, le campagne attive e le campagne batch ricorrenti.
>* Le scadenze pianificate verranno rimosse se la risorsa viene spostata in un altro programma.


## Rimuovere una data di scadenza {#remove-an-expiration-date}

1. Per rimuovere una data di scadenza, controlla le risorse e fai clic su **[!UICONTROL Remove Expiration]**.

   ![](assets/local-asset-expiration-8.png)

1. Esamina le risorse interessate, quindi fai clic su **[!UICONTROL Confirm]**.

   ![](assets/local-asset-expiration-9.png)

>[!NOTE]
>
>Non è possibile rimuovere le date di scadenza inferiori a 15 minuti nel futuro. Per &quot;rimuovere&quot; la scadenza, è necessario attendere che la risorsa scada, quindi riapprovarla o riattivarla.
