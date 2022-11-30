---
unique-page-id: 11382122
description: Abilita Audit Trail - Documenti Marketo - Documentazione del prodotto
title: Abilita traccia di audit
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
source-git-commit: 73d41904ca74ae265648c3ed91805be7c4d24fe0
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Abilita traccia di audit {#enable-audit-trail}

Audit Trail è disponibile per tutti i clienti e controllato da due autorizzazioni di amministratore.

>[!NOTE]
>
>Per impostazione predefinita, tutti i ruoli amministratore di sistema dispongono di entrambe le autorizzazioni abilitate.

## Abilitare Audit Trail per un ruolo {#enable-audit-trail-for-a-role}

1. Fai clic su **Amministratore**.

   ![](assets/enable-audit-trail-1.png)

1. Seleziona **Utenti e ruoli** e fai clic su **Ruoli**.

   ![](assets/enable-audit-trail-2.png)

1. Seleziona il ruolo per il quale desideri abilitare Audit Trail e fai clic su **Modifica ruolo**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >In questo caso puoi anche creare un nuovo ruolo e concedergli l’accesso a Audit Trail.

1. Espandi la **Amministratore di accesso** autorizzazione. Seleziona **Accedi a Audit Trail** e/o **Cronologia accessi**, a seconda delle tue esigenze. Fai clic su **Salva**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**Definizione**
   >
   >**Accesso a Audit Trail:** Consente agli utenti di accedere sia a Asset Audit Trail che ad Admin Audit Trail.
   >
   >**Cronologia accesso:** Consente agli utenti di accedere a [Cronologia accessi utente](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Assegnare il ruolo Audit Trail a un utente {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[Crea](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) o [abilita](#enable-audit-trail) un ruolo esistente, assegnandogli le autorizzazioni Audit Trail.

1. In **Utenti e ruoli**, fai clic su **Utenti**.

   ![](assets/enable-audit-trail-5.png)

1. Selezionare l&#39;utente a cui si desidera concedere l&#39;accesso a Audit Trail e fare clic su **Modifica utente**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >Questo processo si applica anche quando si crea un nuovo utente.

1. Selezionare i ruoli Audit Trail creati. In questo esempio abbiamo creato &quot;Audit Trail - Asset and Admin&quot; e &quot;Audit Trail - With Login History&quot;.

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >Se le aree di lavoro sono abilitate, controlla la casella di controllo del ruolo, che seleziona tutte le aree di lavoro. Deselezionando una singola area di lavoro, verrà nascosta la traccia di controllo. Ciò significa che vedrai i dati di Audit Trail per ogni area di lavoro. È possibile nascondere le aree di lavoro quando [filtro](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Fai clic su **Salva**.

   ![](assets/enable-audit-trail-8.png)
