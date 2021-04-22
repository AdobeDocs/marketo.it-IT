---
unique-page-id: 2953461
description: Sincr. SFDC - Sincronizzazione dei campi - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione dei campi
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Sincr. SFDC: Sincronizzazione dei campi {#sfdc-sync-field-sync}

Marketo sincronizza le informazioni sui campi da Salesforce. Ecco i dettagli.

## Quali campi vengono sincronizzati? {#which-fields-are-synced}

Sincronizziamo la maggior parte dei campi standard in SFDC e tutti i campi personalizzati che l&#39;utente di sincronizzazione ha l&#39;autorizzazione per vedere.

## Come determinare se un record in Marketo è un lead o un contatto in Salesforce? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Abbiamo un campo in Marketo chiamato tipo SFDC. Ha tre possibili valori: piombo, contatto o vuoto. Se è vuoto, significa che questo lead Marketo non esiste in SFDC.

## Come determinare se un lead o un contatto viene eliminato in SFDC? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

In Marketo è presente un campo denominato SFDC isDeleted. Se il valore è true, il lead è stato eliminato in SFDC.

## Come posso essere sicuro che un nuovo campo che aggiungo in SFDC venga aggiunto anche a Marketo? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Se desideri un campo in entrambi i sistemi, crealo prima in SFDC e si sincronizza automaticamente con Marketo.

Se aggiungi un nuovo campo in SFDC e l’utente di sincronizzazione ha l’autorizzazione per visualizzarlo, verrà aggiunto automaticamente a Marketo.

## Cosa succede se cambio un’etichetta di campo in SFDC? {#what-if-i-change-a-field-label-in-sfdc}

La modifica dell’etichetta del campo in SFDC non influisce sull’etichetta del campo in Marketo.

## Cosa succede se cambio un tipo di campo in SFDC? {#what-if-i-change-a-field-type-in-sfdc}

Quando si modifica un tipo di campo, Marketo elimina i dati presenti nei campi se non corrispondono (ma visualizza prima un avviso). Per conservare i dati, è necessario esportarli e reimportarli dopo aver modificato il tipo di campo.

## Cosa succede se modifico un nome API in SFDC? {#what-if-i-change-an-api-name-in-sfdc}

Se modifichi il nome API di un campo in SFDC, in Marketo viene creato un nuovo campo.

## Cosa succede se aggiungo un nuovo valore di elenco a discesa in SFDC? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Se in SFDC viene aggiunto un nuovo valore di elenco a discesa a un campo, Marketo ti invierà una notifica.

## Cosa succede ai campi di ricerca SFDC personalizzati? {#what-about-custom-sfdc-lookup-fields}

I campi di ricerca in SFDC sincronizzano l’ID ma non il nome a cui si fa riferimento.

## E i campi di Formula SFDC? {#what-about-sfdc-formula-fields}

I campi Formula vengono sincronizzati, tuttavia, gli aggiornamenti ai riferimenti nella formula non vengono sincronizzati fino a quando non si verifica un aggiornamento a un [Timbro Mod sistema](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US).

## Cosa succede quando elimino un campo da Salesforce che in precedenza era sincronizzato con Marketo? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Se elimini un campo in SFDC, questo non elimina automaticamente il campo in Marketo, ma interrompe la sincronizzazione.
