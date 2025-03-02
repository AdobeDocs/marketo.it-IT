---
unique-page-id: 2359909
description: Gestione di ruoli e autorizzazioni utente - Documentazione di Marketo - Documentazione del prodotto
title: Gestione di ruoli utente e autorizzazioni
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
feature: Users and Roles
source-git-commit: c10ecc0ccad28f2e480343acefe10f5eca2ae578
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Gestione di ruoli utente e autorizzazioni {#managing-user-roles-and-permissions}

Imposta, crea e modifica i ruoli utente e assegnali agli utenti. Questo consente di controllare le aree e le funzionalità a cui ogni utente di Marketo ha accesso.

Ad esempio, un utente marketing in genere ha bisogno di un ampio accesso in tutta l’applicazione per creare, modificare e distribuire e-mail, pagine di destinazione e programmi. Un web designer, invece, trascorre quasi tutto il suo tempo in Design Studio, creando risorse da utilizzare nelle e-mail e nelle pagine di destinazione. Inoltre, anche se i leader aziendali fanno ampio uso dei rapporti di Marketo nell’area di Analytics, potrebbero non dover creare o gestire direttamente le risorse o i programmi.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Marketo fornisce diversi ruoli incorporati, con diversi livelli di accesso:

* **Amministratore** - Tutte le parti dell&#39;applicazione, inclusa la sezione Amministratore
* **Utente standard** - tutte le parti dell&#39;applicazione, ad eccezione della sezione Admin
* **Utente marketing** - tutte le parti dell&#39;applicazione, tranne la sezione Amministratore
* **Web Designer** - solo Design Studio
* **Utente Analytics** - solo la sezione Analytics

Non puoi modificare i ruoli Amministratore e Utente standard, ma puoi modificare gli altri. Puoi anche creare nuovi ruoli personalizzati che corrispondano alle specifiche strutture organizzative della tua azienda.

## Marketo con identità Adobe {#marketo-with-adobe-identity}

Se utilizzi Marketo con Adobe Identity, l&#39;elenco delle descrizioni del profilo [si trova qui](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md#profile-levels).

## Assegnare ruoli a un utente {#assign-roles-to-a-user}

Puoi assegnare ruoli a un utente quando [crei utenti per la prima volta](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) o [modificando un utente esistente](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/managing-user-roles-and-permissions-1.png)

1. Fai clic su **[!UICONTROL Utenti e ruoli]**.

   ![](assets/managing-user-roles-and-permissions-2.png)

1. Dall&#39;elenco, selezionare l&#39;utente che si desidera modificare e fare clic su **[!UICONTROL Modifica utente]**.

   ![](assets/managing-user-roles-and-permissions-3.png)

1. In **[!UICONTROL Ruoli]**, seleziona i ruoli da assegnare all&#39;utente in base alle autorizzazioni necessarie e fai clic su **[!UICONTROL Salva]**.

   ![](assets/managing-user-roles-and-permissions-4.png)

   >[!NOTE]
   >
   >Per informazioni su ciascun ruolo, vedere [Descrizioni delle autorizzazioni per il ruolo](/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md).

## Crea un nuovo ruolo {#create-a-new-role}

Talvolta all’interno dell’organizzazione sono presenti dipendenti con ruoli molto specifici che richiedono una combinazione personalizzata di autorizzazioni.

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/managing-user-roles-and-permissions-5.png)

1. Fai clic su **[!UICONTROL Utenti e ruoli]**.

   ![](assets/managing-user-roles-and-permissions-6.png)

1. Fare clic sulla scheda **[!UICONTROL Ruoli]**.

   ![](assets/managing-user-roles-and-permissions-7.png)

1. Fai clic su **[!UICONTROL Nuovo ruolo]**.

   ![](assets/managing-user-roles-and-permissions-8.png)

1. Immetti un **[!UICONTROL Nome ruolo]**, una **[!UICONTROL Descrizione]** (facoltativo) e seleziona le autorizzazioni necessarie per gli utenti con questo ruolo.

   ![](assets/managing-user-roles-and-permissions-9.png)

## Modifica un Ruolo {#edit-a-role}

Se è necessario modificare le autorizzazioni associate a un ruolo esistente, è possibile modificare il ruolo.

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/managing-user-roles-and-permissions-10.png)

1. Fai clic su **[!UICONTROL Utenti e ruoli]**.

   ![](assets/managing-user-roles-and-permissions-11.png)

1. Fare clic sulla scheda **[!UICONTROL Ruoli]**.

   ![](assets/managing-user-roles-and-permissions-12.png)

1. Selezionare dall&#39;elenco il ruolo che si desidera modificare e fare clic su **[!UICONTROL Modifica ruolo]**.

   ![](assets/managing-user-roles-and-permissions-13.png)

1. Se necessario, modifica il **[!UICONTROL Nome ruolo]** e la **[!UICONTROL Descrizione]**, modifica la selezione delle **[!UICONTROL Autorizzazioni]** associate e al termine fai clic su **[!UICONTROL Salva]**.

   ![](assets/managing-user-roles-and-permissions-14.png)

   >[!NOTE]
   >
   >Gli utenti che dispongono del ruolo modificato riceveranno le autorizzazioni modificate dopo aver eseguito nuovamente l&#39;accesso e la disconnessione.

## Eliminare un ruolo {#delete-a-role}

Se un ruolo non è più necessario, è possibile eliminarlo.

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/managing-user-roles-and-permissions-15.png)

1. Fai clic su **[!UICONTROL Utenti e ruoli]**.

   ![](assets/managing-user-roles-and-permissions-16.png)

1. Fare clic sulla scheda **[!UICONTROL Ruoli]**.

   ![](assets/managing-user-roles-and-permissions-17.png)

1. Dall&#39;elenco, selezionare il ruolo che si desidera eliminare e fare clic su **[!UICONTROL Elimina ruolo]**.

   ![](assets/managing-user-roles-and-permissions-18.png)

1. Fai clic su **[!UICONTROL Elimina]** per confermare.

   ![](assets/managing-user-roles-and-permissions-19.png)
