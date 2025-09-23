---
unique-page-id: 2359646
description: Configurare la profilatura progressiva dei moduli - Documentazione di Marketo - Documentazione del prodotto
title: Configurare la profilatura progressiva del modulo
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 3%

---

# Configurare la profilatura progressiva del modulo {#configure-form-progressive-profiling}

Le forme corte sono buone! Quando qualcuno ritorna a un modulo, puoi presentare nuovi campi e compilare progressivamente il profilo del visitatore. Ecco come.

>[!NOTE]
>
>Affinché questa funzione funzioni correttamente, assicurati che la precompilazione del modulo sia abilitata per i campi visibili e [disabilitata](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) per i campi nascosti.

1. Vai a **[!UICONTROL Marketing Activities]**.

   ![](assets/ma-1.png)

1. Selezionare il modulo e fare clic su **[!UICONTROL Edit Form]**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. In **[!UICONTROL Form Settings]**, fare clic su **[!UICONTROL Settings]**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Imposta **[!UICONTROL Progressive Profiling]** su **[!UICONTROL Enabled]**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Ok, ora configuriamolo. Vai a **[!UICONTROL Field Details]**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Trascina e rilascia tutti i campi che fanno parte del set di profili progressivi.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Dopo aver spostato tutti i campi, dovrebbe essere simile al seguente:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >I campi al di fuori della casella **[!UICONTROL Progressive Profiling]** verranno sempre visualizzati nel modulo, anche se sono compilati.

1. Selezionare la casella **[!UICONTROL Progressive Profiling]**.

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Prestare attenzione quando si utilizzano i campi obbligatori in [!UICONTROL Progressive Profiling]. Questi campi potrebbero essere lasciati vuoti se il visitatore immette un nuovo indirizzo e-mail (che creerebbe una nuova persona) dopo aver precedentemente inviato i dati per gli altri campi, in quanto verrebbero soppressi nell’ultimo modulo.

1. Ora scegli quanti campi vuoti si desidera visualizzare dalla casella **Profilatura progressiva** in un dato momento.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Se scegli **[!UICONTROL Number of Blank Fields]** come 1, il visitatore vedrà quanto segue la prima volta che vede questo modulo:
   >
   >* Nome (vuoto)
   >* Cognome (vuoto)
   >* Indirizzo e-mail (vuoto)
   >* Numero di telefono (vuoto)
   >
   >Supponendo di compilare ogni campo, la seconda volta che visitano, vedranno:
   >
   >* Nome (precompilato)
   >* Cognome (precompilato)
   >* Indirizzo e-mail (precompilato)
   >* Numero di telefono cellulare (vuoto)
   >
   >Se compilano il numero di telefono cellulare, alla terza visita vedranno:
   >
   >* Nome (precompilato)
   >* Cognome (precompilato)
   >* Indirizzo e-mail (precompilato)
   >* Paese (vuoto)

1. Fai clic su **[!UICONTROL Finish]**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Fai clic su **[!UICONTROL Approve and Close]**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Bel lavoro! Il lavoro che hai appena fatto pagherà.

Sperimenta questa funzione e assicurati di testarla. È avanzato, ma in questo modo è possibile rendere i moduli molto dinamici.
