---
unique-page-id: 2360358
description: Limita accesso utente solo a SSO - Documenti Marketo - Documentazione prodotto
title: Limita accesso utente solo a SSO
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# Limita accesso utente solo a SSO {#restrict-user-login-to-sso-only}

Se si [utilizza SSO](add-single-sign-on-to-a-portal.md) e si desidera garantire che gli utenti non possano ignorare la sicurezza SSO, seguire queste istruzioni.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai ad Admin e fai clic su Impostazioni di accesso.

![](assets/image2014-9-24-14-3a44-3a40.png)

1. Fate clic su Modifica impostazioni di protezione.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Espandete le impostazioni avanzate, selezionate Richiedi SSO e fate clic su Salva.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!TIP]
>
>Se selezionate **Richiedi SSO**, potete escludere un ruolo [](../../../product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) utente da questa restrizione selezionando l&#39;opzione **Ignora Single Sign-On** durante la configurazione del ruolo. In questo modo gli utenti potranno effettuare normalmente l&#39;accesso. Ad esempio, gli utenti Admin potrebbero comunque dover accedere a Marketo tramite la schermata di accesso.

>[!CAUTION]
>
>Quando i nuovi utenti vengono invitati, ricevono e-mail di invito. Tuttavia, se è selezionata l&#39;opzione **Richiedi SSO** , questi messaggi e-mail non vengono ricevuti, a meno che non siano assegnati a un ruolo impostato su **Ignora Single Sign-On**.

È tutto! Ora tutti gli utenti (ad eccezione degli utenti con l&#39;autorizzazione per bypassare il single sign-on) saranno limitati a utilizzare solo l&#39;accesso SSO.