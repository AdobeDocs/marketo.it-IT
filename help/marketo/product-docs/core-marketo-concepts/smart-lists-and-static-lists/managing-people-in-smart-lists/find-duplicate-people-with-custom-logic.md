---
unique-page-id: 2952636
description: Trova persone duplicate con logica personalizzata - Documentazione Marketo - Documentazione del prodotto
title: Trova persone duplicate con logica personalizzata
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 5%

---

# Trova persone duplicate con logica personalizzata {#find-duplicate-people-with-custom-logic}

Il Marketo Engage dispone di un elenco avanzato di sistema che trova le persone duplicate in base ai loro indirizzi e-mail. Se desideri utilizzare un altro campo per trovare duplicati con, ecco come.

>[!PREREQUISITES]
>
>[Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Vai all&#39;area **[!UICONTROL Attività di marketing]**.

![](assets/ma-2.png)

1. Seleziona il tuo elenco avanzato e fai clic sulla scheda **[!UICONTROL Elenco avanzato]**.

   ![](assets/two-4.png)

1. Trova e trascina il filtro **[!UICONTROL Campi duplicati]** nell&#39;area di lavoro.

   ![](assets/three-4.png)

1. Scegli una delle quattro opzioni disponibili:

   * Indirizzo e-mail
   * Nome completo
   * Cognome
   * Data di aggiornamento

   >[!NOTE]
   >
   >Tutti i campi, ad eccezione di Indirizzo e-mail, fanno distinzione tra maiuscole e minuscole. Pertanto, se si utilizza &quot;john doe&quot; nel campo Nome completo, _not_ restituirà risultati per John Doe.

   ![](assets/four-2.png)

   Fine. Esegui Smart List per trovare persone con lo stesso valore nel campo selezionato in precedenza.
