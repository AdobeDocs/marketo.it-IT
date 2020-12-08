---
unique-page-id: 30081815
description: Configurazione dell'integrazione Adobe Experience Manager - Marketo Docs - Documentazione prodotto
title: Configurazione dell'integrazione Adobe Experience Manager
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Configurazione dell&#39;integrazione Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configura AEM per accedere, selezionare e importare risorse AEM in Design Studio di Marketo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!CAUTION]
>
>Al momento, questa funzione è supportata solo in Firefox. Non è supportato in Safari e potrebbe non funzionare nella versione più recente di Chrome (v. 80), a seconda delle impostazioni del cookie SameSite.

1. Passate all’Adobe Experience Manager (l’URL è specifico per la società).

   ![](assets/one.png)

1. Potete accedere con  Adobe o accedere localmente. In questo esempio, l&#39;accesso verrà eseguito localmente.

   ![](assets/two.png)

1. In **Strumenti**, fare clic su **Operazioni** e selezionare Console **** Web.

   ![](assets/2a.png)

1. Nel browser, cercate (Ctrl+F su Windows, Comando+F su Mac) &quot; Adobe Granite Cross-Origin Resource Sharing Policy&quot; (Criterio di condivisione risorse tra le origini granite).

   ![](assets/three.png)

1. Fare clic sul segno **+** a destra.

   ![](assets/four.png)

1. Nella casella di testo Origini **consentite (Regexp)** , digitare &quot;https://.*\.marketo\.com&quot; (senza le virgolette) e fate clic su **Salva**.

   ![](assets/five-psd.png)

1. Nell’intestazione nella parte superiore della pagina, fate clic su Console **** Web e selezionate Informazioni **** sul sistema.

   ![](assets/six.png)

1. In Informazioni sul server, fate clic sul pulsante **Riavvia** .

   ![](assets/seven.png)

1. Fate clic su **OK** per confermare.

   ![](assets/eight.png)

1. In Marketing Classic, fai clic su **Admin**.

   ![](assets/nine.png)

1. In Integrazione, selezionare **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Fate clic su **Modifica**.

   ![](assets/eleven.png)

1. Inserite l’URL AEM e fate clic su **OK**.

   ![](assets/twelve.png)

   Siete tutti pronti! Ora potete [importare AEM risorse in Design Studio in Marketo Sky](http://help.marketo.com/hc/en-us/articles/360036765993).

