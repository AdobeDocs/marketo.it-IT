---
unique-page-id: 37355569
description: Campi personalizzati dei membri del programma - Documentazione di Marketo - Documentazione del prodotto
title: Campi personalizzati del membro del programma
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
feature: Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 1%

---

# Campi personalizzati del membro del programma {#program-member-custom-fields}

I campi personalizzati dei membri del programma consentono di raccogliere dati specifici del programma per ciascun membro. Possono essere utilizzati in: Marketo forms, filtri e attivatori di elenchi avanzati e azioni di flusso di Smart Campaign. I dati sono visualizzabili nella scheda Membri del programma.

## Crea un campo personalizzato membro del programma {#create-a-program-member-custom-field}

1. In Marketo, fare clic su **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Fai clic su **[!UICONTROL Field Management]**.

   ![](assets/two.png)

1. Fai clic su **[!UICONTROL New Custom Field]**.

   ![](assets/three.png)

1. Fare clic sul menu a discesa **[!UICONTROL Object]** e selezionare l&#39;oggetto desiderato.

   ![](assets/four.png)

   >[!NOTE]
   >
   >I campi personalizzati [!UICONTROL Person] e [!UICONTROL Program Member] non possono condividere lo stesso nome.

1. Compila i campi rimanenti e fai clic su **[!UICONTROL Create]**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >I tipi supportati per i campi personalizzati [!UICONTROL Program Member] sono: booleano, data, datetime, float, integer, string, URL. [Ulteriori informazioni sui tipi di campo](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}.

## Descrizioni degli oggetti {#object-descriptions}

| Oggetto | Descrizione |
|---|---|
| Azienda | Il nome dell’azienda associata alla persona. |
| Opportunità | Un&#39;opportunità può essere associata a una persona o a un account come potenziale vendita futura. Di solito entrano in Marketo tramite un sistema CRM o tramite API. |
| Persona | Utente singolo nel database di Marketo con cui collabori tramite campagne di marketing. |
| Membro del programma | Persona che è anche membro di un programma |

## Trigger e filtri {#triggers-and-filters}

Puoi sfruttare questi dati specifici del programma negli elenchi avanzati tramite [trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"} e/o [filtri](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}.

![](assets/six.png)

## Aspetti da considerare {#things-to-know}

* I campi personalizzati dei membri del programma sono disponibili solo nelle risorse locali. Non sono supportati in Design Studio perché non è possibile collegarli a un programma specifico.
* Non è possibile clonare o spostare in Design Studio un modulo (o una pagina di destinazione con un modulo) contenente campi personalizzati per Membri del programma.
* [È possibile sincronizzare](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"} i campi personalizzati del membro del programma con i campi personalizzati del membro della campagna.
* L&#39;oggetto Membro del programma può contenere fino a 20 campi personalizzati. Questi campi sono disponibili per qualsiasi programma.
* Quando si rimuove un membro di un programma, se nel campo personalizzato Membro del programma sono presenti dati, questi verranno eliminati da tale campo.
* Per visualizzare i dati, fare clic sulla scheda Membri nel programma e creare una visualizzazione personalizzata che includa tali campi.
* Sono supportate l&#39;importazione e l&#39;esportazione tramite [list](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"} e [API](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/home){target="_blank"}. Le esportazioni funzionano solo sugli elenchi dei membri del programma, non sugli elenchi statici.
* Quando si uniscono due persone, verranno utilizzati i dati del campo personalizzato Membro del programma del vincitore. Ma se il vincitore non ha, verrà utilizzato il valore del perdente.
* Tipo di modifica non consentito nei campi Informazioni membro programma.
* Il vincolo &quot;contiene&quot; non è supportato per i campi personalizzati dei membri del programma.

>[!MORELIKETHIS]
>
>* [Crea un campo personalizzato in Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}
>
>* [Sincronizzazione campo personalizzato membro programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"}
