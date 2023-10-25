---
unique-page-id: 2952636
description: Trova persone duplicate con logica personalizzata - Documentazione Marketo - Documentazione del prodotto
title: Trova persone duplicate con logica personalizzata
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 6%

---

# Trova persone duplicate con logica personalizzata {#find-duplicate-people-with-custom-logic}

Il Marketo Engage dispone di un elenco avanzato di sistema che trova le persone duplicate in base ai loro indirizzi e-mail. Se desideri utilizzare un altro campo per trovare duplicati con, ecco come.

>[!PREREQUISITES]
>
>[Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Vai a **[!UICONTROL Attività di marketing]** area.

![](assets/ma-2.png)

1. Seleziona il tuo elenco avanzato, fai clic su **[!UICONTROL Elenco avanzato]** scheda.

   ![](assets/two-4.png)

1. Trova e trascina **[!UICONTROL Campi duplicati]** filtra nell’area di lavoro.

   ![](assets/three-4.png)

1. Scegli una delle quattro opzioni disponibili:

   * Indirizzo e-mail
   * Nome completo
   * Cognome
   * Data di aggiornamento

   >[!NOTE]
   >
   >Tutti i campi, ad eccezione di Indirizzo e-mail, fanno distinzione tra maiuscole e minuscole. Pertanto, l’utilizzo di &quot;john doe&quot; nel campo Nome completo _non_ risultati restituiti per John Doe.

   ![](assets/four-2.png)

   Completato! Esegui Smart List per trovare persone con lo stesso valore nel campo selezionato in precedenza.
