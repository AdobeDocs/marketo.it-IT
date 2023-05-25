---
description: "Modificare i limiti di recupero degli oggetti personalizzati in [!DNL Velocity Scripting] - Documentazione di Marketo - Documentazione del prodotto"
title: "Modificare i limiti di recupero degli oggetti personalizzati in [!DNL Velocity Scripting]"
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
source-git-commit: 81ee349dbbe48c70b040751cae750c3684b71c78
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Modificare i limiti di recupero degli oggetti personalizzati in [!DNL Velocity Scripting] {#change-custom-object-retrieval-limits-in-velocity-scripting}

Se usa [!DNL Velocity Script] per visualizzare i dati degli oggetti personalizzati nelle e-mail, questa funzione potrebbe essere adatta a te. Per impostazione predefinita, puoi accedere a 10 oggetti personalizzati principali dallo script Velocity. Se hai bisogno di accedervi di più, continua a leggere.

## Cos’è [!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) è una lingua basata su [!DNL Java] progettato per la creazione di modelli e la creazione di script per contenuti HTML. Marketo consente di utilizzarlo nel contesto delle e-mail tramite l’utilizzo di [token di script](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Questo consente, tra l’altro, di accedere ai dati memorizzati negli oggetti personalizzati.

È possibile fare riferimento a oggetti personalizzati padre e figlio che sono direttamente connessi al lead o al contatto, ma non a oggetti personalizzati di terzo livello. Per ogni oggetto personalizzato, i 10 record aggiornati più di recente per persona/contatto sono disponibili in fase di esecuzione e vengono ordinati dall’ultimo aggiornamento (in corrispondenza di 0) a quello più recente (in corrispondenza di 9).

## Come modificare il limite {#how-to-change-the-limit}

1. Vai a **[!UICONTROL Amministratore]** sezione.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Clic **[!UICONTROL E-mail]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. In [!UICONTROL Limiti di recupero degli oggetti personalizzati] tabella, immettere un nuovo [!UICONTROL Limite di recupero principale] e fai clic su **[!UICONTROL Salva modifiche]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>Il [!UICONTROL Limite di recupero principale] il valore deve essere compreso tra 10 e 100. Il [!UICONTROL Limite di recupero figlio] viene impostato automaticamente. Questo viene fatto dividendo 1000 per [!UICONTROL Limite di recupero principale]. Ad esempio, se si imposta il limite Padre su 50, il limite Figlio diventa 20 (1000 ÷ 50 = 20).

Bello! Ora puoi accedere a più oggetti personalizzati da [!DNL Velocity script].
