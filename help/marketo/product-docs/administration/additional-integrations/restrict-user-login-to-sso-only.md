---
unique-page-id: 2360358
description: Limita l’accesso degli utenti solo all’SSO - Documentazione di Marketo - Documentazione del prodotto
title: Limita l'accesso degli utenti solo all'SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Limita l&#39;accesso degli utenti solo all&#39;SSO {#restrict-user-login-to-sso-only}

Se sei [utilizzo di SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) e desideri garantire che gli utenti non possano ignorare la sicurezza SSO, segui queste istruzioni.

>[!IMPORTANT]
>
>Il presente articolo non si applica a [Adobe IMS abilitato](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) abbonamenti Marketo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Clic **[!UICONTROL Impostazione di accesso]s**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Clic **[!UICONTROL Modifica impostazioni di protezione]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Espandi **[!UICONTROL Avanzate]** impostazioni, verifica **[!UICONTROL Richiedi SSO]** e fai clic su **[!UICONTROL Salva]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>Si consiglia di invitare e accettare l’invito gli utenti. _Dopo_ l’invito è accettato, gli amministratori devono quindi impostarlo su &quot;[!UICONTROL Richiedi SSO].&quot;

>[!TIP]
>
>Se si seleziona **[!UICONTROL Richiedi SSO]**, è possibile escludere un [ruolo utente](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) da questa restrizione controllando il **[!UICONTROL Ignora Single Sign-On]** durante la configurazione del ruolo. In questo modo gli utenti potranno accedere normalmente. Ad esempio, gli utenti Admin potrebbero dover ancora accedere a Marketo tramite la schermata di accesso.

>[!CAUTION]
>
>Quando nuovi utenti vengono invitati, ricevono le e-mail di invito. Tuttavia, se **[!UICONTROL Richiedi SSO]** , a meno che non siano assegnati a un ruolo impostato su **[!UICONTROL Ignora Single Sign-On]**.

Tutto qui! Ora tutti gli utenti (ad eccezione di quelli che dispongono dell&#39;autorizzazione per ignorare il Single Sign-On) saranno limitati a utilizzare solo l&#39;accesso SSO.

>[!MORELIKETHIS]
>
>* [Aggiungere il Single Sign-On a un portale](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Utilizzo di un ID universale per l’accesso in abbonamento](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Invito degli utenti di Marketo a due istanze con ID universale](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
