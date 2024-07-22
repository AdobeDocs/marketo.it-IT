---
unique-page-id: 1147340
description: Inviare e-mail dal proprietario del lead - Documentazione Marketo - Documentazione del prodotto
title: Invia e-mail dal proprietario del lead
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Invia e-mail dal proprietario del lead {#send-emails-from-the-lead-owner}

Cosa succede se desideri inviare un’e-mail a un lead per conto del proprietario del lead?  Ecco come.

1. Trova il tuo indirizzo e-mail, selezionalo e fai clic su **Modifica bozza**.

   ![](assets/one.png)

1. Fai clic nel campo **Da** (elimina eventuali nomi esistenti) e fai clic sul pulsante **Inserisci token**.

   ![](assets/two.png)

1. Inizia a digitare &quot;`{{lead.Lead Owner`&quot; e seleziona il token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Immettere un valore predefinito nel caso in cui il lead non disponga ancora di un proprietario lead e fare clic su **Inserisci**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Fare clic dopo il primo token, aggiungere uno spazio, quindi fare clic sul pulsante **Inserisci token**.

   ![](assets/five.png)

1. Inizia a digitare &quot;`{{lead.Lead Owner`&quot; e seleziona il token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Immettere un valore predefinito nel caso in cui il lead non disponga ancora di un proprietario lead e fare clic su **Inserisci**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Assicurati di aver aggiunto uno spazio tra i token di nome e cognome.

1. Fai clic nel campo Da e-mail (elimina eventuali indirizzi e-mail esistenti), quindi fai clic sul pulsante Inserisci token.

   ![](assets/eight.png)

1. Inizia a digitare &quot;`{{lead.Lead Owner`&quot; e seleziona il token **`{{lead.Lead Owner Email Address}}`**.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Immettere un valore predefinito nel caso in cui il lead non disponga ancora di un proprietario lead e fare clic su **Inserisci**.

   ![](assets/ten.png)

1. Completati con i campi **Rispondi a** e **Oggetto**.

   ![](assets/eleven.png)
