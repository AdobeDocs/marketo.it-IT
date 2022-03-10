---
unique-page-id: 2360358
description: Limitare l’accesso dell’utente solo all’accesso SSO - Documenti Marketo - Documentazione del prodotto
title: Limita accesso utente solo a SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
source-git-commit: a21db1586166b7530bbbb18759752ef834cdc46a
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# Limita accesso utente solo a SSO {#restrict-user-login-to-sso-only}

Se sei [utilizzo di SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) e per assicurarsi che gli utenti non possano ignorare la sicurezza SSO, seguire queste istruzioni.

>[!IMPORTANT]
>
>Il presente articolo non si applica a [Adobe IMS abilitato](/help/marketo/product-docs/administration/marketo-with-adobe-identity/overview.md) Abbonamenti Marketo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai a **Amministratore** e fai clic su **Impostazioni di accesso**.

   ![](assets/image2014-9-24-14-3a44-3a40.png)

1. Fai clic su **Modifica impostazioni di protezione**.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Espandi le impostazioni avanzate, seleziona **Richiedi SSO** e fai clic su **Salva**.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!NOTE]
>
>Si consiglia agli utenti di essere invitati e di accettare l’invito. _Dopo_ l&#39;invito viene accettato, gli amministratori devono quindi impostarlo su &quot;Richiedi SSO&quot;.

>[!TIP]
>
>Se si seleziona **Richiedi SSO**, puoi escludere un [ruolo utente](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) da questa restrizione controllando il **Ignora Single Sign-On** durante la configurazione del ruolo. In questo modo gli utenti possono accedere normalmente. Ad esempio, gli utenti amministratori potrebbero comunque dover accedere a Marketo tramite la schermata di accesso.

>[!CAUTION]
>
>Quando i nuovi utenti vengono invitati, ricevono le e-mail di invito. Tuttavia, se **Richiedi SSO** è selezionato, non riceveranno tali e-mail, a meno che non siano assegnate a un ruolo impostato su **Ignora Single Sign-On**.

Tutto qui! Ora tutti gli utenti (ad eccezione degli utenti con l&#39;autorizzazione di bypassare il single sign-on) saranno limitati all&#39;utilizzo solo dell&#39;accesso SSO.

>[!MORELIKETHIS]
>
>* [Aggiungere Single Sign-On a un portale](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Utilizzo di un ID universale per l’accesso all’abbonamento](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Invitare gli utenti Marketo a due istanze con ID universale](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

