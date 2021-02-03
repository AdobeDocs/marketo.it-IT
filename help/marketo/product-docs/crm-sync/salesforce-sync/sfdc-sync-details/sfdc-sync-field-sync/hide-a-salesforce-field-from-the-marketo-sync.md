---
unique-page-id: 4719306
description: Nascondere un campo Salesforce dalla sincronizzazione Marketo - Marketo Docs - Documentazione del prodotto
title: Nascondere un campo Salesforce dalla sincronizzazione Marketo
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---


# Nascondere un campo Salesforce dalla sincronizzazione di Marketo {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Non tutti i campi di Salesforce sono utili per Marketing. Potete ottimizzare le prestazioni di sincronizzazione includendo solo i campi necessari. Ecco come si può nascondere un campo da Marketo.

1. Fare clic sul menu del nome e selezionare **Configurazione**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Immettere **profili** nella barra di ricerca e fare clic su **Profili** in **Gestisci utenti**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Fate clic sul profilo dell&#39;utente per la sincronizzazione.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Nella sezione **Sicurezza a livello di campo**, fare clic su **Visualizza** accanto all&#39;oggetto che contiene il campo di destinazione.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Fare clic su **Modifica**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Deselezionare la casella di controllo **Visibile** accanto al campo da nascondere. Fare clic su **Salva**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Se il campo nascosto in Salesforce è già stato sincronizzato con Marketo, dovrai nasconderlo anche in Marketo, se non vuoi usarlo.

   È tutto! Questo campo non verrà più visualizzato in Marketo al termine della sincronizzazione successiva.

   >[!MORELIKETHIS]
   >
   >[Nascondere e visualizzare un campo](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
