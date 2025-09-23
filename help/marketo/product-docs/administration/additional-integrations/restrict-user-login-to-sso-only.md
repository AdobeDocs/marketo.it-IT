---
unique-page-id: 2360358
description: Limita l’accesso degli utenti solo all’SSO - Documentazione di Marketo - Documentazione del prodotto
title: Limitare l’accesso utente solo al SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 8%

---

# Limitare l’accesso utente solo al SSO {#restrict-user-login-to-sso-only}

Se [utilizzi SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) e vuoi essere certo che gli utenti non possano ignorare la sicurezza SSO, segui queste istruzioni.

>[!IMPORTANT]
>
>Questo articolo non è applicabile alle [sottoscrizioni Marketo abilitate per Adobe IMS](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md).

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Fai clic su **[!UICONTROL Login Settings]**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Fai clic su **[!UICONTROL Edit Security Settings]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Espandere le impostazioni di **[!UICONTROL Advanced]**, selezionare **[!UICONTROL Require SSO]** e fare clic su **[!UICONTROL Save]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>Si consiglia di invitare e accettare l’invito gli utenti. _Dopo_ l&#39;invito è accettato, gli amministratori devono quindi impostarli su &quot;[!UICONTROL Require SSO]&quot;.

>[!TIP]
>
>Se si seleziona **[!UICONTROL Require SSO]**, è possibile escludere un [ruolo utente](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) da questa restrizione selezionando l&#39;opzione **[!UICONTROL Bypass Single Sign-On]** durante la configurazione del ruolo. In questo modo gli utenti potranno accedere normalmente. Ad esempio, gli utenti Admin potrebbero dover ancora accedere a Marketo tramite la schermata di accesso. Se sono abilitati sia SSO che Universal ID, è necessario disporre dell&#39;autorizzazione &quot;Bypass Single Signed On&quot; (Ignora Single Sign On) per attivare o disattivare le sottoscrizioni.

>[!CAUTION]
>
>Quando nuovi utenti vengono invitati, ricevono le e-mail di invito. Tuttavia, se **[!UICONTROL Require SSO]** è selezionato, non riceverà queste e-mail, a meno che non sia assegnato a un ruolo impostato su **[!UICONTROL Bypass Single Sign-On]**.

Tutto qui. Ora tutti gli utenti (ad eccezione di quelli che dispongono dell&#39;autorizzazione per ignorare il Single Sign-On) saranno limitati a utilizzare solo l&#39;accesso SSO.

>[!MORELIKETHIS]
>
>* [Aggiungi Single Sign-On a un portale](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Utilizzo di un ID universale per l&#39;accesso all&#39;abbonamento](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Invito di utenti Marketo a due istanze con ID universale](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
