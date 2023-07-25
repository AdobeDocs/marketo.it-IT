---
unique-page-id: 2359646
description: Configurare la profilatura progressiva dei moduli - Documentazione di Marketo - Documentazione del prodotto
title: Configurare la profilatura progressiva dei moduli
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Configurare la profilatura progressiva dei moduli {#configure-form-progressive-profiling}

Le forme corte sono buone! Quando qualcuno ritorna a un modulo, puoi presentare nuovi campi e compilare progressivamente il profilo del visitatore. Ecco come.

>[!NOTE]
>
>Affinché questa funzione funzioni correttamente, assicurati che la precompilazione del modulo sia abilitata per i campi visibili e [disabilitato](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) per i campi nascosti.

1. Vai a **Attività di marketing**.

   ![](assets/ma-1.png)

1. Seleziona il modulo e fai clic su **Modifica modulo**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. Sotto **Impostazioni modulo**, fai clic su **Impostazioni**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Imposta **Profilatura progressiva** a **Abilitato**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Ok, ora configuriamolo. Vai a **Dettagli campo**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Trascina e rilascia tutti i campi che fanno parte del set di profili progressivi.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Dopo aver spostato tutti i campi, dovrebbe essere simile al seguente:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Campi al di fuori del **Profilatura progressiva** viene sempre visualizzata nel modulo, anche se è stata compilata.

1. Seleziona la **Profilatura progressiva** casella.

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Presta attenzione quando utilizzi i campi obbligatori nella profilatura progressiva. Questi campi potrebbero essere lasciati vuoti se il visitatore immette un nuovo indirizzo e-mail (che creerebbe una nuova persona) dopo aver precedentemente inviato i dati per gli altri campi, in quanto verrebbero soppressi nell’ultimo modulo.

1. Scegliere il numero di campi vuoti che si desidera visualizzare dall&#39; **Profilatura progressiva** in qualsiasi momento.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Se si sceglie **Numero** **di** **Vuoto** **Campi** come 1, la prima volta che vede questo modulo il visitatore vedrà quanto segue:
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

1. Clic **Fine**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Clic **Approva e chiudi**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Bel lavoro! Il lavoro che hai appena fatto pagherà.

Sperimenta questa funzione e assicurati di testarla. È avanzato, ma in questo modo è possibile rendere i moduli molto dinamici.
