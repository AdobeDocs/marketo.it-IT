---
unique-page-id: 2359909
description: Gestione di ruoli utente e autorizzazioni - Documenti Marketo - Documentazione del prodotto
title: Gestione di ruoli e autorizzazioni utente
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
source-git-commit: 3bb7e8155491f810cc0e71637482e6da788dc068
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Gestione di ruoli e autorizzazioni utente {#managing-user-roles-and-permissions}

Imposta, crea e modifica i ruoli utente e assegnali agli utenti. Questo consente di controllare le aree e le funzionalità a cui ogni utente Marketo ha accesso.

Ad esempio, un utente di marketing in genere ha bisogno di un accesso ampio all’interno dell’applicazione per creare, modificare e distribuire e-mail, pagine di destinazione e programmi. Un web designer, invece, trascorre quasi tutto il tempo in Design Studio, creando risorse da utilizzare nelle e-mail e nelle pagine di destinazione. E mentre i leader aziendali utilizzano ampiamente i rapporti di Marketo nell’area Analytics, potrebbero non dover creare o guidare direttamente le risorse o i programmi.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Marketo fornisce diversi ruoli incorporati, con diversi livelli di accesso:

* **Amministratore** - tutte le parti dell&#39;applicazione, inclusa la sezione Amministratore
* **Utente standard** - tutte le parti dell&#39;applicazione, ad eccezione della sezione Amministratore
* **Utente marketing** - tutte le parti dell&#39;applicazione, ad eccezione della sezione Amministratore
* **Progettazione web** - solo Design Studio
* **Utente di Analytics** - solo la sezione Analytics

Non puoi modificare i ruoli Amministratore e Utente standard, ma puoi modificarli. Puoi anche creare nuovi ruoli personalizzati per adattarli alle strutture organizzative specifiche della tua azienda.

## Marketo con identità Adobe {#marketo-with-adobe-identity}

Se utilizzi Marketo con Adobe Identity, l’elenco delle descrizioni del profilo [si trova qui](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md#profile-levels).

## Assegnare ruoli a un utente {#assign-roles-to-a-user}

Puoi assegnare ruoli a un utente quando [creare utenti per la prima volta](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) o [modifica di un utente esistente](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. Vai a **Amministratore** area.

   ![](assets/managing-user-roles-and-permissions-1.png)

1. Fai clic su **Utenti e ruoli**.

   ![](assets/managing-user-roles-and-permissions-2.png)

1. Dall’elenco, seleziona l’utente da modificare e fai clic su **Modifica utente**.

   ![](assets/managing-user-roles-and-permissions-3.png)

1. Sotto **Ruoli**, seleziona i ruoli da assegnare all’utente in base alle autorizzazioni necessarie e fai clic su **Salva**.

   ![](assets/managing-user-roles-and-permissions-4.png)

   >[!NOTE]
   >
   >Per informazioni su ciascun ruolo, consulta  [Descrizioni delle autorizzazioni del ruolo](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md).

## Creare un nuovo ruolo {#create-a-new-role}

A volte, la tua organizzazione dispone di dipendenti con ruoli molto specifici che richiedono una combinazione personalizzata di autorizzazioni.

1. Vai a **Amministratore** area.

   ![](assets/managing-user-roles-and-permissions-5.png)

1. Fai clic su **Utenti e ruoli**.

   ![](assets/managing-user-roles-and-permissions-6.png)

1. Fai clic sul pulsante **Ruoli** scheda .

   ![](assets/managing-user-roles-and-permissions-7.png)

1. Fai clic su **Nuovo ruolo**.

   ![](assets/managing-user-roles-and-permissions-8.png)

1. Inserisci un **Nome del ruolo**, **Descrizione** (facoltativo) e seleziona le autorizzazioni necessarie agli utenti di questo ruolo.

   ![](assets/managing-user-roles-and-permissions-9.png)

## Modificare un ruolo {#edit-a-role}

Se devi modificare le autorizzazioni associate a un ruolo esistente, puoi modificare il ruolo.

1. Vai a **Amministratore** area.

   ![](assets/managing-user-roles-and-permissions-10.png)

1. Fai clic su **Utenti e ruoli**.

   ![](assets/managing-user-roles-and-permissions-11.png)

1. Fai clic sul pulsante **Ruoli** scheda .

   ![](assets/managing-user-roles-and-permissions-12.png)

1. Dall’elenco, seleziona il ruolo da modificare e fai clic su **Modifica ruolo**.

   ![](assets/managing-user-roles-and-permissions-13.png)

1. Modificare la **Nome del ruolo** e **Descrizione** se necessario, quindi modificare la selezione di **Autorizzazioni**.

   ![](assets/managing-user-roles-and-permissions-14.png)

   >[!NOTE]
   >
   >Gli utenti con il ruolo modificato riceveranno le autorizzazioni modificate dopo la disconnessione e il nuovo accesso.

## Eliminare un ruolo {#delete-a-role}

Se un ruolo non è necessario, è possibile eliminarlo.

1. Vai a **Amministratore** area.

   ![](assets/managing-user-roles-and-permissions-15.png)

1. Fai clic su **Utenti e ruoli**.

   ![](assets/managing-user-roles-and-permissions-16.png)

1. Fai clic sul pulsante **Ruoli** scheda .

   ![](assets/managing-user-roles-and-permissions-17.png)

1. Dall’elenco, seleziona il ruolo da eliminare e fai clic su **Elimina ruolo**.

   ![](assets/managing-user-roles-and-permissions-18.png)

1. Fai clic su **Elimina** per confermare.

   ![](assets/managing-user-roles-and-permissions-19.png)
