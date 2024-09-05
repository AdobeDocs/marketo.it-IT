---
unique-page-id: 2360358
description: Limita l’accesso degli utenti solo all’SSO - Documentazione di Marketo - Documentazione del prodotto
title: Limita l'accesso degli utenti solo all'SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: a12e4e420c01623305a0fa34b1e3973162e24d68
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# Limita l&#39;accesso degli utenti solo all&#39;SSO {#restrict-user-login-to-sso-only}

Se [utilizzi SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) e vuoi essere certo che gli utenti non possano ignorare la sicurezza SSO, segui queste istruzioni.

>[!IMPORTANT]
>
>Questo articolo non è applicabile alle [sottoscrizioni Marketo abilitate per Adobe IMS](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md).

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Fare clic su **[!UICONTROL Impostazione accesso]s**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Fare clic su **[!UICONTROL Modifica impostazioni di protezione]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Espandi le impostazioni **[!UICONTROL Avanzate]**, seleziona **[!UICONTROL Richiedi SSO]** e fai clic su **[!UICONTROL Salva]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>Si consiglia di invitare e accettare l’invito gli utenti. _Dopo_ l&#39;invito è accettato, gli amministratori devono quindi impostarli su &quot;[!UICONTROL Richiedi SSO].&quot;

>[!TIP]
>
>Se si seleziona **[!UICONTROL Richiedi SSO]**, è possibile escludere un [ruolo utente](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) da questa restrizione selezionando l&#39;opzione **[!UICONTROL Ignora Single Sign-On]** durante la configurazione del ruolo. In questo modo gli utenti potranno accedere normalmente. Ad esempio, gli utenti Admin potrebbero dover ancora accedere a Marketo tramite la schermata di accesso. Se sono abilitati sia SSO che Universal ID, è necessario disporre dell&#39;autorizzazione &quot;Bypass Single Signed On&quot; (Ignora Single Sign On) per attivare o disattivare le sottoscrizioni.

>[!CAUTION]
>
>Quando nuovi utenti vengono invitati, ricevono le e-mail di invito. Tuttavia, se è selezionato **[!UICONTROL Richiedi SSO]**, questi messaggi non verranno ricevuti a meno che non siano assegnati a un ruolo impostato su **[!UICONTROL Ignora Single Sign-On]**.

Tutto qui. Ora tutti gli utenti (ad eccezione di quelli che dispongono dell&#39;autorizzazione per ignorare il Single Sign-On) saranno limitati a utilizzare solo l&#39;accesso SSO.

>[!MORELIKETHIS]
>
>* [Aggiungi Single Sign-On a un portale](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Utilizzo di un ID universale per l&#39;accesso all&#39;abbonamento](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Invito di utenti Marketo a due istanze con ID universale](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
