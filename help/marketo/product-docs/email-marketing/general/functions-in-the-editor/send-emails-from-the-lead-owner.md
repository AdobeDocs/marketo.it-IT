---
unique-page-id: 1147340
description: Inviare e-mail dal proprietario lead - Documenti Marketo - Documentazione del prodotto
title: Invia e-mail dal proprietario lead
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Invia e-mail dal proprietario lead {#send-emails-from-the-lead-owner}

Cosa succede se desideri inviare un’e-mail a un lead per conto del proprietario lead?  Ecco come.

1. Trova il tuo messaggio e-mail, selezionalo e fai clic su **Modifica bozza**.

   ![](assets/one.png)

1. Fai clic in **Da** (eliminare un nome esistente), quindi fare clic sul pulsante **Inserisci token** pulsante .

   ![](assets/two.png)

1. Inizia a digitare &quot;`{{lead.Lead Owner`&quot; e seleziona la **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Immetti un valore predefinito nel caso in cui il lead non disponga ancora di un proprietario di lead e fai clic su **Inserisci**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Fai clic dopo il primo token, aggiungi uno spazio, quindi fai clic sul **Inserisci token** pulsante .

   ![](assets/five.png)

1. Inizia a digitare &quot;`{{lead.Lead Owner`&quot; e seleziona la **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Immetti un valore predefinito nel caso in cui il lead non disponga ancora di un proprietario di lead e fai clic su **Inserisci**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Assicurati di aver aggiunto uno spazio tra i token del nome e del cognome.

1. Fai clic nel campo Da e-mail (elimina qualsiasi indirizzo e-mail esistente) e fai clic sul pulsante Inserisci token .

   ![](assets/eight.png)

1. Inizia a digitare &quot;`{{lead.Lead Owner`&quot; e seleziona la **`{{lead.Lead Owner Email Address}}`** token.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Immetti un valore predefinito nel caso in cui il lead non disponga ancora di un proprietario di lead e fai clic su **Inserisci**.

   ![](assets/ten.png)

1. Assicurati che **Risposta** e **Oggetto** i campi sono popolati e hai finito!

   ![](assets/eleven.png)
