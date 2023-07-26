---
unique-page-id: 42762511
description: Configurare la mappatura dell’organizzazione Adobe - Documenti Marketo - Documentazione del prodotto
title: Imposta mapping organizzazione Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Imposta mapping organizzazione Adobe {#set-up-adobe-organization-mapping}

Per sincronizzarsi con applicazioni Adobe, come Audienci Manager, il connettore Marketo CDP B2B, [!DNL Dynamic Chat], ecc., devi prima immettere le credenziali dell’organizzazione Adobe IMS in Marketo.

>[!NOTE]
>
>Una distribuzione compatibile con HIPAA di un’istanza Marketo non può utilizzare questa integrazione.

>[!CAUTION]
>
>Per i clienti che effettuano l’onboarding in Adobe Business Platform e Identity Management System, l’ID organizzazione associato all’abbonamento sarà già popolato ed è un campo di sola lettura.

1. In Marketo, fai clic su **[!UICONTROL Amministratore]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. In Integrazione, fai clic su **[!UICONTROL Mappatura organizzazione Adobe]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Clic **[!UICONTROL Modifica]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Immetti l’ID organizzazione Adobe IMS (scopri come trovare [qui](https://experienceleague.adobe.com/docs/control-panel/using/faq.html){target="_blank"}) e fai clic su **[!UICONTROL OK]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Clic **[!UICONTROL Conferma]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Fai clic su **[!UICONTROL Chiudi]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Per motivi di sicurezza, devi essere un amministratore organizzazione per l’organizzazione Adobe a cui desideri mappare. In caso contrario, l’azione avrà esito negativo. Inoltre, l’utente Adobe e l’utente Marketo devono utilizzare lo stesso indirizzo e-mail al momento dell’accesso.

1. Se sei _non_ già connesso, verrà visualizzato un pop-up in una nuova scheda/finestra. Accedi all’organizzazione di Adobe (questa azione convalida l’accesso all’organizzazione).

Ed è tutto! Ora puoi [condividere i dati sul pubblico](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} to, or [sync an audience](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} da Adobe Experience Cloud.
