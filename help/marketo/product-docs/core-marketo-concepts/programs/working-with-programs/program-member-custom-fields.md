---
unique-page-id: 37355569
description: Campi personalizzati per i membri del programma - Documenti Marketo - Documentazione prodotto
title: Campi personalizzati membri del programma
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Campi personalizzati membri del programma {#program-member-custom-fields}

I campi personalizzati dei membri del programma consentono di raccogliere dati specifici per ciascun membro. Possono essere utilizzati in: Moduli marketing, filtri e attivatori per elenchi avanzati e azioni di flusso per Smart Campaign. I dati sono visualizzabili nella scheda Membri del programma.

## Creare un campo personalizzato membro del programma {#create-a-program-member-custom-field}

1. In Marketo, fare clic su **Admin**.

   ![](assets/one.png)

1. Fare clic su **Gestione dei campi**.

   ![](assets/two.png)

1. Fare clic su **Nuovo campo personalizzato**.

   ![](assets/three.png)

1. Fare clic sul menu a discesa Oggetto e selezionare l&#39;oggetto desiderato.

   ![](assets/four.png)

   >[!NOTE]
   >
   >I campi personalizzati della persona e del membro del programma non possono condividere lo stesso nome.

1. Compilare i campi rimanenti e fare clic su **Crea**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >I tipi supportati per i campi personalizzati dei membri del programma sono: booleano, data, datetime, float, integer, stringa, URL. [Ulteriori informazioni sui tipi](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md) di campo.

## Descrizioni oggetto {#object-descriptions}

| Oggetto | Descrizione |
|---|---|
| Azienda | Nome della società associata alla persona. |
| Opportunità | Un&#39;opportunità può essere associata a una persona o un conto come potenziale vendita futura. Di solito entrano in Marketo tramite un CRM, o tramite API. |
| Person | Un individuo nel database Marketo con cui ti occupi tramite campagne di marketing. |
| Membro del programma | Persona che è anche membro di un programma |

## Triggers e filtri {#triggers-and-filters}

È possibile utilizzare questi dati specifici del programma negli elenchi smart tramite [trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md) e/o [filtri](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md).

![](assets/six.png)

## Informazioni da conoscere {#things-to-know}

* I campi personalizzati per i membri del programma sono disponibili solo nelle risorse locali. Non sono supportati in Design Studio perché non è possibile collegarli a un programma specifico.
* Non è possibile duplicare/spostare in Design Studio un modulo (o una pagina di destinazione con un modulo) contenente campi personalizzati per i membri del programma.
* I campi personalizzati dei membri del programma non possono essere utilizzati come token.
* L&#39;oggetto Member del programma può avere fino a 20 campi personalizzati. Questi campi sono disponibili per qualsiasi programma.
* Quando si rimuove un membro di un programma, se nel campo personalizzato Membro programma sono presenti dati, i dati verranno eliminati da tale campo.
* Per visualizzare i dati, fare clic sulla scheda Membri del programma e creare una visualizzazione personalizzata che includa tali campi.
* Sono supportate l&#39;importazione e l&#39;esportazione tramite [list](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)e [API](https://developers.marketo.com/).
* Quando si uniscono due persone, verranno utilizzati i dati del campo personalizzato Membro programma del vincitore. Tuttavia, se il vincitore non ne ha, verrà utilizzato il valore del perdente.

>[!MORELIKETHIS]
>
>[Creare un campo personalizzato in Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
