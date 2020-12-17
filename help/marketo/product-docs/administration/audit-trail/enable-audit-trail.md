---
unique-page-id: 11382122
description: Abilita traccia di controllo - Documenti Marketo - Documentazione prodotto
title: Abilita traccia di controllo
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---


# Abilita traccia di controllo {#enable-audit-trail}

Audit Trail è disponibile per tutti i clienti e controllato da due autorizzazioni di amministratore.

>[!NOTE]
>
>Per impostazione predefinita, tutti i ruoli amministratore di sistema dispongono di entrambe le autorizzazioni abilitate.

## Abilita traccia di controllo per un ruolo {#enable-audit-trail-for-a-role}

1. Fare clic su **Admin**.

   ![](assets/one-2.png)

1. Selezionare **Utenti e ruoli** e fare clic su **Ruoli**.

   ![](assets/two-2.png)

1. Selezionare il ruolo per il quale si desidera abilitare la traccia di controllo e fare clic su **Modifica ruolo**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >È inoltre disponibile l&#39;opzione per creare un nuovo ruolo e concedergli l&#39;accesso a Audit Trail.

1. Espandi l&#39;autorizzazione **Accedi ad Amministratore**. Selezionare **Access Audit Trail** e/o **Access Login History**, a seconda delle esigenze. Fare clic su **Salva**.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >**Definizione**
   >
   >
   >**Accesso alla traccia di audit:** consente agli utenti di accedere sia alla traccia di audit delle risorse che alla traccia di audit dell’amministratore.
   >
   >
   >**Cronologia di accesso:** consente agli utenti di accedere alla cronologia [ di accesso ](user-login-history.md)utente.

## Assegna ruolo traccia di controllo a un utente {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[](http://docs.marketo.com/display/DOCS/Create,+Delete,+Edit+and+Change+a+User+Role#Create,Delete,EditandChangeaUserRole-CreateaRole) Creazione o  [](#Enable) abilitazione di un ruolo esistente, assegnando ad esso le autorizzazioni Audit Trail.

1. In **Utenti e ruoli**, fare clic su **Utenti**.

   ![](assets/five-1.png)

1. Selezionare l&#39;utente a cui si desidera consentire l&#39;accesso alla traccia di audit e fare clic su **Edit User**.

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >Questo processo si applica anche quando create un nuovo utente.

1. Selezionare i ruoli Audit Trail creati. In questo esempio abbiamo creato &quot;Audit Trail - Asset and Admin,&quot; e &quot;Audit Trail - With Login History&quot;.

   ![](assets/seven-1.png)

   >[!CAUTION]
   >
   >Se le aree di lavoro sono abilitate, selezionate la casella di controllo del ruolo, che seleziona tutte le aree di lavoro. Se si deseleziona una singola area di lavoro, verrà nascosta la traccia di controllo. Questo significa che vedrai i dati della traccia di controllo per ogni area di lavoro. È possibile nascondere le aree di lavoro durante il [filtraggio](http://docs.marketo.com/display/DOCS/Filtering+in+Audit+Trail).

1. Fare clic su **Salva**.

   ![](assets/eight-1.png)

