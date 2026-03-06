---
description: Aumenta o diminuisce il limite di recupero degli oggetti personalizzati padre per lo script  [!DNL Velocity]  nelle e-mail (da 10 a 100).
title: Modifica dei limiti di recupero degli oggetti personalizzati in [!DNL Velocity Scripting]
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# Modifica dei limiti di recupero degli oggetti personalizzati in [!DNL Velocity Scripting] {#change-custom-object-retrieval-limits-in-velocity-scripting}

Se utilizzi [!DNL Velocity Script] per visualizzare i dati degli oggetti personalizzati nelle e-mail, questa funzione potrebbe essere adatta a te. Per impostazione predefinita, puoi accedere a 10 oggetti personalizzati principali dallo script Velocity. Se hai bisogno di accedervi di più, continua a leggere.

## Cos&#39;è [!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) è un linguaggio basato su [!DNL Java] progettato per la creazione di modelli e lo scripting del contenuto di HTML. Marketo consente di utilizzarlo nel contesto delle e-mail tramite [token di script](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Questo consente, tra l’altro, di accedere ai dati memorizzati negli oggetti personalizzati.

È possibile fare riferimento a oggetti personalizzati padre e figlio che sono direttamente connessi al lead o al contatto, ma non a oggetti personalizzati di terzo livello. Per ogni oggetto personalizzato, i 10 record aggiornati più di recente per persona/contatto sono disponibili in fase di esecuzione e vengono ordinati dall’ultimo aggiornamento (in corrispondenza di 0) a quello più recente (in corrispondenza di 9).

## Come modificare il limite {#how-to-change-the-limit}

1. Passare alla sezione **[!UICONTROL Admin]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Fai clic su **[!UICONTROL Email]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Nella tabella [!UICONTROL Custom Object Retrieval Limits], immettere un nuovo [!UICONTROL Parent Retrieval Limit] e fare clic su **[!UICONTROL Save Changes]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>Il valore [!UICONTROL Parent Retrieval Limit] deve essere compreso tra 10 e 100. [!UICONTROL Child Retrieval Limit] viene impostato automaticamente. A tale scopo, dividere 1000 per [!UICONTROL Parent Retrieval Limit]. Ad esempio, se si imposta il limite Padre su 50, il limite Figlio diventa 20 (1000 ÷ 50 = 20).

Bello! È ora possibile accedere a più oggetti personalizzati da [!DNL Velocity script].
