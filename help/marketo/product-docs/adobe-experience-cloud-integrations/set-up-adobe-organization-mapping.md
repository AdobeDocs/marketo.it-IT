---
unique-page-id: 42762511
description: Configurare Adobe Organization Mapping - Documentazione Marketo - Documentazione del prodotto
title: Configurare la mappatura dell’organizzazione Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 5%

---

# Configurare la mappatura dell’organizzazione Adobe {#set-up-adobe-organization-mapping}

Per eseguire la sincronizzazione con le applicazioni Adobe, come Audience Manager, il connettore Marketo di CDP B2B, [!DNL Dynamic Chat] e così via, è necessario innanzitutto immettere le credenziali dell’organizzazione Adobe IMS in Marketo Engage.

>[!NOTE]
>
>* Una distribuzione compatibile con HIPAA di un’istanza Marketo non può utilizzare questa integrazione.
>* Affinché l’integrazione funzioni, Marketo e le altre applicazioni Adobe devono trovarsi nella stessa organizzazione.

>[!IMPORTANT]
>
>Per coloro che hanno effettuato l’onboarding in Adobe Business Platform e Identity Management System, l’ID organizzazione associato all’abbonamento sarà già popolato ed è un campo di sola lettura. Di conseguenza, le disposizioni del presente articolo non si applicano.

1. In Marketo, fare clic su **[!UICONTROL Admin]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. In Integrazione fare clic su **[!UICONTROL Adobe Organization Mapping]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Fai clic su **[!UICONTROL Edit]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Immetti l&#39;ID organizzazione Adobe IMS (scopri come trovare [qui](https://experienceleague.adobe.com/docs/control-panel/using/faq.html){target="_blank"}) e fai clic su **[!UICONTROL OK]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Fai clic su **[!UICONTROL Confirm]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Fai clic su **[!UICONTROL Close]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Per motivi di sicurezza, devi essere un amministratore organizzazione per l’organizzazione Adobe a cui desideri mappare. In caso contrario, l’azione avrà esito negativo. Inoltre, l’utente di Adobe e l’utente di Marketo devono utilizzare lo stesso indirizzo e-mail al momento dell’accesso.

1. Se _non_ hai già effettuato l&#39;accesso, verrà visualizzato un pop-up in una nuova scheda/finestra. Accedi all’organizzazione Adobe (questa azione convalida l’accesso all’organizzazione).

È ora possibile [condividere i dati del pubblico](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} o [sincronizzare un pubblico](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} da Adobe Experience Cloud.
