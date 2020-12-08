---
unique-page-id: 1147340
description: Invia e-mail dal proprietario principale - Documenti Marketo - Documentazione prodotto
title: Invia e-mail dal proprietario principale
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Invia e-mail dal proprietario principale {#send-emails-from-the-lead-owner}

Cosa succede se si desidera inviare un&#39;e-mail a un lead per conto del proprietario principale?  Ecco come.

1. Individuate il messaggio e-mail, selezionatelo e fate clic su **Modifica bozza**.

   ![](assets/one.png)

1. Fate clic nel campo **Da** (eliminate il nome esistente), quindi fate clic sul pulsante **Inserisci token** .

   ![](assets/two.png)

1. Iniziate a digitare &quot;`{{lead.Lead Owner`&quot; e selezionate il **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Immettete un valore predefinito nel caso in cui il lead non disponga ancora di un proprietario per lead e fate clic su **Inserisci**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Fate clic dopo il primo token, aggiungete uno spazio, quindi fate clic sul pulsante **Inserisci token** .

   ![](assets/five.png)

1. Iniziate a digitare &quot;`{{lead.Lead Owner`&quot; e selezionate il **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Immettete un valore predefinito nel caso in cui il lead non disponga ancora di un proprietario per lead e fate clic su **Inserisci**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Accertatevi di aver aggiunto uno spazio tra i token del nome e del cognome.

   Fate clic nel campo Da e-mail (eliminate eventuali indirizzi e-mail esistenti), quindi fate clic sul pulsante Inserisci token.
   ![](assets/eight.png)

1. Iniziate a digitare &quot;`{{lead.Lead Owner`&quot; e selezionate il **`{{lead.Lead Owner Email Address}}`** token.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Immettete un valore predefinito nel caso in cui il lead non disponga ancora di un proprietario per lead e fate clic su **Inserisci**.

   ![](assets/ten.png)

1. Accertatevi che i campi **Rispondi** e **Oggetto** siano popolati e che sia fatto!

   ![](assets/eleven.png)

