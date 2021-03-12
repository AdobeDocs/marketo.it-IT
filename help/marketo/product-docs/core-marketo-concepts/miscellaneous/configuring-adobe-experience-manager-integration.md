---
unique-page-id: 30081815
description: Configurazione dell’integrazione di Adobe Experience Manager - Documenti Marketo - Documentazione del prodotto
title: Configurazione dell’integrazione di Adobe Experience Manager
translation-type: tm+mt
source-git-commit: cfefff241b34571b9778cbd827f45d1b468d121e
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Configurazione dell&#39;integrazione di Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configura AEM in modo da poter accedere, selezionare e importare risorse AEM in Design Studio di Marketo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!CAUTION]
>
>Attualmente, questa funzione è supportata solo in Firefox. Non è supportato in Safari e potrebbe non funzionare nell’ultima versione di Chrome (v. 80), a seconda delle impostazioni dei cookie SameSite.

1. Passa a Adobe Experience Manager (l’URL è specifico per la tua azienda).

   ![](assets/one.png)

1. Puoi accedere con Adobe o localmente. In questo esempio effettueremo l’accesso localmente.

   ![](assets/two.png)

1. In **Strumenti**, fai clic su **Operazioni** e seleziona **Console web**.

   ![](assets/2a.png)

1. Nel browser, cerca (ctrl+f su Windows, cmd+f su Mac) &quot;Adobe Granite Cross-Origin Resource Sharing Policy&quot;.

   ![](assets/three.png)

1. Fai clic sul segno **+** a destra.

   ![](assets/four.png)

1. Nella casella di testo **Origini consentite (Regexp)**, digitare `https://.*\.marketo\.com` e fare clic su **Salva**.

   ![](assets/five-psd.png)

1. Nell&#39;intestazione nella parte superiore della pagina, fai clic su **Console web** e seleziona **Informazioni di sistema**.

   ![](assets/six.png)

1. In Informazioni server fare clic sul pulsante **Restart** .

   ![](assets/seven.png)

1. Fare clic su **OK** per confermare.

   ![](assets/eight.png)

1. In Marketo Classic fare clic su **Amministratore**.

   ![](assets/nine.png)

1. In Integrazione, seleziona **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Fare clic su **Modifica**.

   ![](assets/eleven.png)

1. Inserisci l&#39;URL AEM e fai clic su **OK**.

   ![](assets/twelve.png)

   Siete pronti! È ora possibile [importare AEM risorse in Design Studio in Marketo Sky](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/importing-assets-with-adobe-experience-manager.html?lang=en#design-studio).
