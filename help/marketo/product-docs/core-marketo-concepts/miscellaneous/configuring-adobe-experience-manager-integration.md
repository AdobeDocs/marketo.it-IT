---
unique-page-id: 30081815
description: Configurazione dell’integrazione di Adobe Experience Manager - Documentazione di Marketo - Documentazione del prodotto
title: Configurazione dell’integrazione di Adobe Experience Manager
hide: true
hidefromtoc: true
exl-id: 06b2c214-1afb-443f-ae01-0c00fed77dce
source-git-commit: 2a94e4b3b034eac821a82a84db65c09e503c52f4
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Configurazione dell’integrazione di Adobe Experience Manager {#configuring-adobe-experience-manager-integration}

Configura Adobe Experience Manager (AEM) per accedere, selezionare e importare AEM risorse nel Marketo Engage Design Studio.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!IMPORTANT]
>
>* Questa integrazione funziona solo con le implementazioni on-premise di AEM e non è supportata per le implementazioni AEM Cloud Service.
>
>* Attualmente, questa funzione è supportata solo in Firefox. Non è supportato in Safari e potrebbe non funzionare nell’ultima versione di Chrome, a seconda delle impostazioni dei cookie SameSite.


1. Passa ad Adobe Experience Manager (l’URL è specifico per la tua azienda).

   ![](assets/one.png)

1. Puoi accedere con Adobe o localmente. In questo esempio, effettueremo l’accesso localmente.

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

1. In Marketo Engage, fai clic su **Amministratore**.

   ![](assets/nine.png)

1. In Integrazione, seleziona **Adobe Experience Manager**.

   ![](assets/ten.png)

1. Fai clic su **Modifica**.

   ![](assets/eleven.png)

1. Inserisci l&#39;URL AEM e fai clic su **OK**.

   ![](assets/twelve.png)
