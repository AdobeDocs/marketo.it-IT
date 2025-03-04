---
unique-page-id: 11382122
description: Abilitare Audit Trail - Documentazione Marketo - Documentazione del prodotto
title: Abilita Audit Trail
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
feature: Audit Trail
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 1%

---

# Abilita Audit Trail {#enable-audit-trail}

Audit Trail è disponibile per tutti i clienti ed è controllato da due autorizzazioni amministratore.

>[!NOTE]
>
>Per impostazione predefinita, per tutti i ruoli di amministratore di sistema sono abilitate entrambe le autorizzazioni.

## Abilita Audit Trail per un ruolo {#enable-audit-trail-for-a-role}

1. Fai clic su **[!UICONTROL Amministratore]**.

   ![](assets/enable-audit-trail-1.png)

1. Seleziona **[!UICONTROL Utenti e ruoli]** e fai clic su **[!UICONTROL Ruoli]**.

   ![](assets/enable-audit-trail-2.png)

1. Selezionare il ruolo per il quale si desidera abilitare Audit Trail e fare clic su **[!UICONTROL Modifica ruolo]**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >In questo caso puoi anche creare un nuovo ruolo e concedergli l’accesso a Audit Trail.

1. Espandi l&#39;autorizzazione **[!UICONTROL Accesso amministratore]**. Seleziona **[!UICONTROL Accedi a prova di verifica]** e/o **[!UICONTROL Accedi alla cronologia]**, in base alle tue esigenze. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**Definizione**
   >
   >**[!UICONTROL Accesso Audit Trail]**: consente agli utenti di accedere sia a [!UICONTROL Asset Audit Trail] che a [!UICONTROL Admin Audit Trail].
   >
   >**[!UICONTROL Cronologia accesso]**: consente agli utenti di accedere a [Cronologia accesso utenti](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Assegna ruolo Audit Trail a un utente {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[Crea](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) o [abilita](#enable-audit-trail) un ruolo esistente, assegnandogli le autorizzazioni Audit Trail.

1. In **[!UICONTROL Utenti e ruoli]**, fare clic su **[!UICONTROL Utenti]**.

   ![](assets/enable-audit-trail-5.png)

1. Selezionare l&#39;utente a cui si desidera concedere l&#39;accesso Audit Trail e fare clic su **[!UICONTROL Modifica utente]**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >Questo processo si applica anche quando si crea un nuovo utente.

1. Seleziona i ruoli Audit Trail creati. In questo esempio abbiamo creato &quot;Audit Trail - Risorse e amministratore&quot; e &quot;Audit Trail - Con cronologia di accesso&quot;.

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >Se sono state abilitate aree di lavoro, assicurarsi di selezionare la casella di controllo del ruolo, che seleziona tutte le aree di lavoro. Deselezionando una singola area di lavoro, verrà nascosto Audit Trail. Ciò significa che vedrai i dati di Audit Trail per ogni area di lavoro. È possibile nascondere le aree di lavoro quando [si filtra](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/enable-audit-trail-8.png)
