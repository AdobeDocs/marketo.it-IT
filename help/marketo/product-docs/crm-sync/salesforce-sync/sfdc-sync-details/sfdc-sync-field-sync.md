---
unique-page-id: 2953461
description: Sincr. SFDC - Sincronizzazione dei campi - Documenti Marketo - Documentazione del prodotto
title: Sincr. SFDC - Sincronizzazione campo
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# Sincr. SFDC: Sincronizzazione campo {#sfdc-sync-field-sync}

Marketo sincronizza le informazioni sui campi da Salesforce. Ecco i dettagli.

## Quali campi sono sincronizzati? {#which-fields-are-synced}

Sincronizziamo la maggior parte dei campi standard in SFDC e tutti i campi personalizzati che l&#39;utente della sincronizzazione ha l&#39;autorizzazione a visualizzare.

## Come determinare se un record di Marketo è un lead o un contatto in Salesforce? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Abbiamo un campo in Marketo chiamato Tipo SFDC. Ha tre possibili valori: piombo, contatto o è vuoto. Se è vuoto, significa che il lead Marketo non esiste nella DSC.

## Come determinare se un lead o un contatto viene eliminato dalla DSC? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Abbiamo un campo in Marketo chiamato SFDC isDeleted. Se il valore è true, il lead viene eliminato in SFDC.

## Come posso fare in modo che un nuovo campo aggiunto nella DSC venga aggiunto anche a Marketo? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Se si desidera un campo in entrambi i sistemi, crearlo prima in SFDC e si sincronizza automaticamente su Marketo.

Se si aggiunge un nuovo campo in SFDC e l&#39;utente di sincronizzazione ha l&#39;autorizzazione per visualizzarlo, verrà aggiunto automaticamente a Marketo.

## Cosa succede se si modifica un&#39;etichetta di campo in SFDC? {#what-if-i-change-a-field-label-in-sfdc}

La modifica dell&#39;etichetta del campo in SFDC non influisce sull&#39;etichetta del campo in Marketo.

## Cosa succede se si modifica un tipo di campo in SFDC? {#what-if-i-change-a-field-type-in-sfdc}

Quando si modifica un tipo di campo, Marketo elimina i dati presenti nei campi se non corrispondono (ma visualizza prima un avviso). Per conservare i dati, assicurarsi di esportarli e importarli nuovamente dopo aver modificato il tipo di campo.

## Cosa succede se cambio un nome di API in SFDC? {#what-if-i-change-an-api-name-in-sfdc}

Se si modifica il nome API di un campo in SFDC, in Marketo viene creato un nuovo campo.

## Cosa succede se si aggiunge un nuovo valore di elenco di selezione in SFDC? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Se a un campo viene aggiunto un nuovo valore di elenco di selezione, in SFDC Marketo invia una notifica.

## Che dire dei campi di ricerca SFDC personalizzati? {#what-about-custom-sfdc-lookup-fields}

I campi di ricerca in SFDC sincronizzano l’ID ma non il nome di riferimento.

## E i campi di Formula SFDC? {#what-about-sfdc-formula-fields}

I campi formula sono sincronizzati, tuttavia, gli aggiornamenti ai riferimenti nella formula non vengono sincronizzati finché non viene eseguito un aggiornamento a un [Timbro del sistema](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US).

## Cosa succede quando si elimina un campo da Salesforce precedentemente sincronizzato con Marketo? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Se si elimina un campo in SFDC, questo non viene eliminato automaticamente in Marketo, ma la sincronizzazione viene interrotta.
