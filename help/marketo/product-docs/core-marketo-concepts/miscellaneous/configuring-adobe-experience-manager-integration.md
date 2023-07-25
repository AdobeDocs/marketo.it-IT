---
unique-page-id: 30081815
description: Configurazione dell’integrazione di Adobe Experience Manager - Documentazione di Marketo - Documentazione del prodotto
title: Configurazione dell’integrazione di Adobe Experience Manager
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Configurazione dell’integrazione di Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configura Adobe Experience Manager (AEM) in modo da poter accedere, selezionare e importare le risorse AEM in Marketi Engage Design Studio.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!IMPORTANT]
>
>* Questa integrazione funziona solo con le implementazioni on-premise dell’AEM e non è supportata per le implementazioni AEM Cloud Service.
>
>* Attualmente, questa funzione è completamente supportata solo in Firefox. Non è supportato in Safari e potrebbe non funzionare nella versione più recente di Chrome, a seconda delle impostazioni del cookie SameSite.

1. Passa a Adobe Experience Manager (l’URL è specifico per la tua azienda).

   ![](assets/one.png)

1. Puoi accedere con Adobe o localmente. In questo esempio, effettueremo l’accesso localmente.

   ![](assets/two.png)

1. In entrata **Strumenti**, fai clic su **Operazioni** e seleziona **Console web**.

   ![](assets/2a.png)

1. Nel browser, cerca (Ctrl+F su Windows, Comando+F su Mac) per &quot;Adobe di criteri di condivisione risorse tra le origini di Granite&quot;.

   ![](assets/three.png)

1. Fai clic su **+** accedi a destra.

   ![](assets/four.png)

1. In **Origini consentite (Regexp)** casella di testo, digitare `https://.*\.marketo\.com` e fai clic su **Salva**.

   ![](assets/five-psd.png)

1. Nell’intestazione nella parte superiore della pagina, fai clic su **Console web** e seleziona **Informazioni di sistema**.

   ![](assets/six.png)

1. In Informazioni server fare clic su **Riavvia** pulsante.

   ![](assets/seven.png)

1. Clic **OK** per confermare.

   ![](assets/eight.png)

1. In Marketo Engage, fai clic su **Amministratore**.

   ![](assets/nine.png)

1. In Integrazione, seleziona **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Clic **Modifica**.

   ![](assets/eleven.png)

1. Inserisci l’URL dell’AEM e fai clic su **OK**.

   ![](assets/twelve.png)
