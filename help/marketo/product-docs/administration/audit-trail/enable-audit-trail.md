---
unique-page-id: 11382122
description: Abilita Audit Trail - Documenti Marketo - Documentazione del prodotto
title: Abilita traccia di audit
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Abilita traccia di audit {#enable-audit-trail}

Audit Trail è disponibile per tutti i clienti e controllato da due autorizzazioni di amministratore.

>[!NOTE]
>
>Per impostazione predefinita, tutti i ruoli amministratore di sistema dispongono di entrambe le autorizzazioni abilitate.

## Abilitare Audit Trail per un ruolo {#enable-audit-trail-for-a-role}

1. Fai clic su **Amministratore**.

   ![](assets/one-2.png)

1. Seleziona **Utenti e ruoli** e fai clic su **Ruoli**.

   ![](assets/two-2.png)

1. Seleziona il ruolo per cui desideri abilitare Audit Trail e fai clic su **Modifica ruolo**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >In questo caso puoi anche creare un nuovo ruolo e concedergli l’accesso a Audit Trail.

1. Espandi l’autorizzazione **Accedi ad Amministratore** . Seleziona **Access Audit Trail** e/o **Access Login History**, a seconda delle tue esigenze. Fare clic su **Salva**.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >**Definizione**
   >
   >**Accedi a Audit Trail:** consente agli utenti di accedere sia a Asset Audit Trail che ad Admin Audit Trail.
   >
   >**Cronologia accessi:** consente agli utenti di accedere alla cronologia degli accessi  [utente](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Assegnare il ruolo Audit Trail a un utente {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) Crea o  [](#enable-audit-trail) abilita un ruolo esistente, assegnandogli le autorizzazioni Audit Trail.

1. In **Utenti e ruoli**, fai clic su **Utenti**.

   ![](assets/five-1.png)

1. Selezionare l&#39;utente a cui si desidera concedere l&#39;accesso a Audit Trail e fare clic su **Modifica utente**.

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >Questo processo si applica anche quando si crea un nuovo utente.

1. Selezionare i ruoli Audit Trail creati. In questo esempio abbiamo creato &quot;Audit Trail - Asset and Admin&quot; e &quot;Audit Trail - With Login History&quot;.

   ![](assets/seven-1.png)

   >[!CAUTION]
   >
   >Se le aree di lavoro sono abilitate, controlla la casella di controllo del ruolo, che seleziona tutte le aree di lavoro. Deselezionando una singola area di lavoro, verrà nascosta la traccia di controllo. Ciò significa che vedrai i dati di Audit Trail per ogni area di lavoro. È possibile nascondere le aree di lavoro durante il [filtraggio](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Fare clic su **Salva**.

   ![](assets/eight-1.png)
