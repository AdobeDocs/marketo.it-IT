---
unique-page-id: 42762511
description: Impostare Adobe Organization Mapping - Marketo Docs - Documentazione del prodotto
title: Configurare la mappatura dell'organizzazione Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: c396c205d3cececc752f9b563c0d2ab41ff92b6a
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Configurare la mappatura dell&#39;organizzazione Adobe {#set-up-adobe-organization-mapping}

Per eseguire la sincronizzazione con applicazioni di Adobe, ad Audience Manager il connettore Marketo CDP B2B, la chat dinamica e così via, è necessario prima immettere le credenziali dell’organizzazione Adobe IMS in Marketo.

>[!NOTE]
>
>Impossibile utilizzare questa integrazione in una distribuzione HIPAA di un&#39;istanza Marketo.

>[!CAUTION]
>
>Per i clienti che hanno effettuato l’accesso ad Adobe Business Platform e al sistema Identity Management, l’ID organizzazione associato all’abbonamento sarà già popolato ed è un campo di sola lettura.

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. In Integrazione, fai clic su **Mappatura dell&#39;organizzazione di Adobe**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Fai clic su **Modifica**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Immetti il tuo ID organizzazione Adobe IMS (scopri come trovarlo) [qui](https://experienceleague.adobe.com/docs/control-panel/using/faq.html)) e fai clic su **OK**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Fai clic su **Conferma**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Fai clic su **Chiudi**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Per motivi di sicurezza, devi essere un amministratore organizzazione per l’organizzazione Adobe a cui desideri eseguire la mappatura. In caso contrario, l’azione avrà esito negativo. Inoltre, l’utente Adobe e l’utente Marketo devono utilizzare lo stesso indirizzo e-mail al momento dell’accesso.

1. Se sei _not_ già connesso, un pop-up apparirà in una nuova scheda/finestra. Accedi alla tua organizzazione Adobe (questa azione convalida l&#39;accesso all&#39;organizzazione).

Ed è tutto! Ora puoi [condividere dati sul pubblico](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target=&quot;_blank&quot;} su o [sincronizzare un pubblico](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/sync-an-audience-from-adobe-experience-cloud.md){target=&quot;_blank&quot;} da Adobe Experience Cloud.
