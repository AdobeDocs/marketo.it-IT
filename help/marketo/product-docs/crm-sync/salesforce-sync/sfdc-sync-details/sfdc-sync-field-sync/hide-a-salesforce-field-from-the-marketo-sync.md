---
unique-page-id: 4719306
description: Nascondere un campo Salesforce dalla Marketo Sync - Marketo Docs - Documentazione del prodotto
title: Nascondere un campo Salesforce dalla sincronizzazione Marketo
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Nascondere un campo Salesforce dalla sincronizzazione Marketo {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Non tutti i campi di Salesforce sono utili per il marketing. Puoi ottimizzare le prestazioni di sincronizzazione includendo solo i campi necessari. Ecco come nascondere un campo da Marketo.

1. Fai clic sul menu del nome e seleziona **Configurazione**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Inserisci **profili** nella barra di ricerca e fai clic su **Profili** in **Gestisci utenti**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Fai clic sul profilo dell’utente di sincronizzazione.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Nella sezione **Sicurezza a livello di campo**, fare clic su **Visualizza** accanto all&#39;oggetto contenente il campo di destinazione.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Fare clic su **Modifica**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Deseleziona la casella di controllo **Visibile** accanto al campo da nascondere. Fare clic su **Salva**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Se il campo nascosto in Salesforce è già stato sincronizzato con Marketo, dovrai nasconderlo anche in Marketo, se non lo desideri.

   Tutto qui! Questo campo non verrà più visualizzato in Marketo al termine della sincronizzazione successiva.

   >[!MORELIKETHIS]
   >
   >[Nascondere e visualizzare un campo](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
