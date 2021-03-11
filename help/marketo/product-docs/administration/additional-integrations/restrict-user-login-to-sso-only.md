---
unique-page-id: 2360358
description: Limita l’accesso dell’utente solo all’SSO - Documenti Marketo - Documentazione del prodotto
title: Limita accesso utente solo a SSO
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---


# Limita l&#39;accesso dell&#39;utente a SSO solo {#restrict-user-login-to-sso-only}

Se utilizzi [SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) e desideri garantire che gli utenti non possano ignorare la sicurezza SSO, segui queste istruzioni.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai a **Amministratore** e fai clic su **Impostazioni di accesso**.

   ![](assets/image2014-9-24-14-3a44-3a40.png)

1. Fare clic su **Modifica impostazioni di protezione**.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Espandi le impostazioni avanzate, seleziona **Richiedi SSO** e fai clic su **Salva**.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!NOTE]
>
>Si consiglia agli utenti di essere invitati e di accettare l’invito. __ Una volta accettato l’invito, gli amministratori devono impostarlo su &quot;Richiedi SSO&quot;.

>[!TIP]
>
>Se selezioni **Richiedi SSO**, puoi escludere un [ruolo utente](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) da questa restrizione selezionando l&#39;opzione **Ignora Single Sign-On** durante la configurazione del ruolo. In questo modo gli utenti possono accedere normalmente. Ad esempio, gli utenti amministratori potrebbero comunque dover accedere a Marketo tramite la schermata di accesso.

>[!CAUTION]
>
>Quando i nuovi utenti vengono invitati, ricevono le e-mail di invito. Tuttavia, se è selezionato **Richiedi SSO**, questi messaggi e-mail non vengono ricevuti, a meno che non siano assegnati a un ruolo impostato su **Ignora Single Sign-On**.

Tutto qui! Ora tutti gli utenti (ad eccezione degli utenti con l&#39;autorizzazione di bypassare il single sign-on) saranno limitati all&#39;utilizzo solo dell&#39;accesso SSO.

>[!MORELIKETHIS]
>
>* [Aggiungere Single Sign-On a un portale](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Utilizzo di un ID universale per l’accesso all’abbonamento](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Invitare gli utenti di Marketo a due istanze con ID universale](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

