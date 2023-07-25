---
unique-page-id: 4719306
description: Nascondere un campo Salesforce da Marketo Sync - Marketo Docs - Documentazione del prodotto
title: Nascondere un campo Salesforce da Marketo Sync
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Nascondere un campo Salesforce da Marketo Sync {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Non tutti i campi in Salesforce sono utili per il Marketing. È possibile ottimizzare le prestazioni di sincronizzazione includendo solo i campi necessari. Ecco come nascondere un campo da Marketo.

1. Fai clic sul menu del nome e seleziona **Configurazione**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Invio **profili** nella barra di ricerca e fai clic su **Profili** in **Gestisci utenti**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Fai clic sul profilo dell’utente di sincronizzazione.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Sotto **Sicurezza a livello di campo** , fare clic su **Visualizza** accanto all&#39;oggetto che contiene il campo di destinazione.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Clic **Modifica**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Deseleziona la **Visibile** accanto al campo da nascondere. Clic **Salva**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Se il campo nascosto in Salesforce è già stato sincronizzato con Marketo, dovrai nasconderlo anche in Marketo se non desideri utilizzarlo.

   Tutto qui! Questo campo non verrà più visualizzato in Marketo al termine della prossima sincronizzazione.

   >[!MORELIKETHIS]
   >
   >[Nascondere e scoprire un campo](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
