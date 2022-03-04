---
unique-page-id: 30081815
description: Configurazione dell’integrazione di Adobe Experience Manager - Documentazione di Marketo - Documentazione del prodotto
title: Configurazione dell’integrazione di Adobe Experience Manager
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
source-git-commit: 47b0f31b410f0bf4b41740aa6440c2a0484ab835
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Configurazione dell’integrazione di Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configura AEM per accedere, selezionare e importare AEM risorse in Marketo Design Studio.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!CAUTION]
>
>Attualmente, questa funzione è supportata solo in Firefox. Non è supportato in Safari e potrebbe non funzionare nell’ultima versione di Chrome, a seconda delle impostazioni dei cookie SameSite.

1. Passa ad Adobe Experience Manager (l’URL è specifico per la tua azienda).

   ![](assets/one.png)

1. Puoi accedere con Adobe o localmente. In questo esempio effettueremo l’accesso localmente.

   ![](assets/two.png)

1. In **Strumenti**, fai clic su **Operazioni** e seleziona **Console web**.

   ![](assets/2a.png)

1. Nel browser, cerca (ctrl+f su Windows, cmd+f su Mac) per &quot;Criteri di condivisione risorse multiorigine di Adobe Granite&quot;.

   ![](assets/three.png)

1. Fai clic sul pulsante **+** firma a destra.

   ![](assets/four.png)

1. In **Origini consentite (Regexp)** casella di testo, digitare `https://.*\.marketo\.com` e fai clic su **Salva**.

   ![](assets/five-psd.png)

1. Nell’intestazione nella parte superiore della pagina, fai clic su **Console web** e seleziona **Informazioni di sistema**.

   ![](assets/six.png)

1. In Informazioni server , fai clic sul pulsante **Riavvia** pulsante .

   ![](assets/seven.png)

1. Fai clic su **OK** per confermare.

   ![](assets/eight.png)

1. In Marketo Classic, fai clic su **Amministratore**.

   ![](assets/nine.png)

1. In Integrazione, seleziona **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Fai clic su **Modifica**.

   ![](assets/eleven.png)

1. Inserisci l&#39;URL AEM e fai clic su **OK**.

   ![](assets/twelve.png)

   Siete pronti! Ora puoi [importare AEM risorse in Design Studio in Marketo Sky](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/importing-assets-with-adobe-experience-manager.html?lang=en#design-studio).
