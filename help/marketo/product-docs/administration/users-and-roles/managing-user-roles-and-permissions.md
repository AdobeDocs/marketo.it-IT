---
unique-page-id: 2359909
description: Gestione di ruoli utente e autorizzazioni - Documenti Marketo - Documentazione del prodotto
title: Gestione di ruoli e autorizzazioni utente
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
source-git-commit: a360b46ab1cd7149f609d139590124dcfcda8dad
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Gestione di ruoli e autorizzazioni utente {#managing-user-roles-and-permissions}

Imposta, crea e modifica i ruoli utente e assegnali agli utenti. Questo consente di controllare le aree e le funzionalità a cui ogni utente Marketo ha accesso.

Ad esempio, un utente di marketing in genere ha bisogno di un accesso ampio all’interno dell’applicazione per creare, modificare e distribuire e-mail, pagine di destinazione e programmi. Un web designer, invece, trascorre quasi tutto il tempo in Design Studio, creando risorse da utilizzare nelle e-mail e nelle pagine di destinazione. E mentre i leader aziendali utilizzano ampiamente i rapporti di Marketo nell’area di Analytics, potrebbero non dover creare o guidare direttamente le risorse o i programmi.

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

Se utilizzi Marketo con Adobe Identity, l’elenco delle descrizioni del profilo [si trova qui](/help/marketo/product-docs/administration/marketo-with-adobe-identity/overview.md#profile-levels).

## Assegnare ruoli a un utente {#assign-roles-to-a-user}

Puoi assegnare ruoli a un utente quando [creare utenti per la prima volta](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) o [modifica di un utente esistente](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. Per modificare un utente esistente, vai a **Amministratore** e fai clic su **Utenti e ruoli**.

   ![](assets/image2014-9-9-18-3a7-3a32.png)

1. Dall’elenco, seleziona l’utente da modificare e fai clic su **Modifica utente**.

   ![](assets/image2014-9-9-18-3a7-3a42.png)

1. Sotto **Ruoli**, seleziona i ruoli da assegnare all’utente in base alle autorizzazioni necessarie e fai clic su **Salva**.

   ![](assets/image2014-9-9-18-3a7-3a57.png)

   >[!NOTE]
   >
   >Per informazioni su ciascun ruolo, consulta  [Descrizioni delle autorizzazioni del ruolo](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md).

## Creare un nuovo ruolo {#create-a-new-role}

A volte, la tua organizzazione dispone di dipendenti con ruoli molto specifici che richiedono una combinazione personalizzata di autorizzazioni.

1. Per creare un nuovo ruolo utente, vai ad Amministratore e fai clic su **Utenti e ruoli**.

   ![](assets/image2014-9-9-18-3a8-3a12.png)

1. Fai clic sul pulsante **Ruoli** scheda .

   ![](assets/image2014-9-9-18-3a8-3a22.png)

1. Fai clic su **Nuovo ruolo**.

   ![](assets/image2014-9-9-18-3a8-3a38.png)

1. Inserisci un **Nome del ruolo**, **Descrizione** (facoltativo) e seleziona le autorizzazioni necessarie agli utenti di questo ruolo.

   ![](assets/image2014-9-9-18-3a9-3a3.png)

## Modificare un ruolo {#edit-a-role}

Se devi modificare le autorizzazioni associate a un ruolo esistente, puoi modificare il ruolo.

1. Vai a **Amministratore** e fai clic su **Utenti e ruoli**.

   ![](assets/image2014-9-9-18-3a9-3a15.png)

1. Fai clic sul pulsante **Ruoli** scheda .

   ![](assets/image2014-9-9-18-3a9-3a26.png)

1. Dall’elenco, seleziona il ruolo da modificare e fai clic su **Modifica ruolo**.

   ![](assets/image2014-9-9-18-3a9-3a40.png)

1. Modificare la **Nome del ruolo** e **Descrizione** se necessario, quindi modificare la selezione di **Autorizzazioni**.

   ![](assets/image2014-9-9-18-3a10-3a3.png)

   >[!NOTE]
   >
   >Gli utenti con il ruolo modificato riceveranno le autorizzazioni modificate dopo la disconnessione e il nuovo accesso.

## Eliminare un ruolo {#delete-a-role}

Se un ruolo non è necessario, è possibile eliminarlo.

1. Vai ad Amministratore e fai clic su **Utenti e ruoli**.

   ![](assets/image2014-9-9-18-3a10-3a15.png)

1. Fai clic sul pulsante **Ruoli** scheda .

   ![](assets/image2014-9-9-18-3a10-3a27.png)

1. Dall’elenco, seleziona il ruolo da eliminare e fai clic su **Elimina ruolo**.

   ![](assets/image2014-9-9-18-3a10-3a39.png)

1. Fai clic su **Elimina** per confermare.

   ![](assets/image2014-9-9-18-3a10-3a50.png)
