---
unique-page-id: 1147340
description: Scopri come inviare e-mail dall’indirizzo del proprietario del lead. Utilizza l’opzione Invia da proprietario lead per visualizzare il mittente corretto nelle e-mail.
title: Inviare e-mail dal proprietario del lead
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
TQID: 'https://experienceleague.adobe.com/iOBonqrup6ZV9QGhW-i1FpabLVBOKrNxz4xqThcexZ8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: eeae636f-f283-4051-94f0-4d74945464fb
    internal-label: Email Editor
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 7%
---
# Inviare e-mail dal proprietario del lead {#send-emails-from-the-lead-owner}

Cosa succede se desideri inviare un’e-mail a un lead per conto del proprietario del lead?  Ecco come.

1. Trova il tuo indirizzo e-mail, selezionalo e fai clic su **[!UICONTROL Edit Draft]**.

   ![](assets/one.png)

1. Fai clic nel campo **[!UICONTROL From]** (elimina eventuali nomi esistenti), quindi fai clic sul pulsante **Inserisci token**.

   ![](assets/two.png)

1. Inizia a digitare &quot;`{{lead.Lead Owner`&quot; e seleziona il token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Immettere un valore predefinito nel caso in cui il lead non disponga ancora di un proprietario lead e fare clic su **[!UICONTROL Insert]**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Fare clic dopo il primo token, aggiungere uno spazio, quindi fare clic sul pulsante **Inserisci token**.

   ![](assets/five.png)

1. Inizia a digitare &quot;`{{lead.Lead Owner`&quot; e seleziona il token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Immettere un valore predefinito nel caso in cui il lead non disponga ancora di un proprietario lead e fare clic su **[!UICONTROL Insert]**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Assicurati di aver aggiunto uno spazio tra i token di nome e cognome.

1. Fai clic nel campo **[!UICONTROL From Address]** (elimina eventuali indirizzi e-mail esistenti), quindi fai clic sul pulsante **Inserisci token**.

   ![](assets/eight.png)

1. Inizia a digitare &quot;`{{lead.Lead Owner`&quot; e seleziona il token **`{{lead.Lead Owner Email Address}}`**.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Immettere un valore predefinito nel caso in cui il lead non disponga ancora di un proprietario lead e fare clic su **[!UICONTROL Insert]**.

   ![](assets/ten.png)

1. Completare i campi **[!UICONTROL Reply-to]** e **[!UICONTROL Subject]**.

   ![](assets/eleven.png)
