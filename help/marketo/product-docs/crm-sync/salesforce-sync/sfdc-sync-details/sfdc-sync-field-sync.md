---
unique-page-id: 2953461
description: Sincronizzazione SFDC - Sincronizzazione campi - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione campi
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Sincronizzazione SFDC: Sincronizzazione campi {#sfdc-sync-field-sync}

Marketo sincronizza le informazioni del campo da Salesforce. Ecco i dettagli.

## Quali campi sono sincronizzati? {#which-fields-are-synced}

Sincronizziamo la maggior parte dei campi standard in SFDC e tutti i campi personalizzati che l&#39;utente di sincronizzazione può visualizzare.

## Come puoi determinare se un record in Marketo è un lead o un contatto in Salesforce? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

In Marketo è presente un campo denominato Tipo SFDC. Possiede tre valori possibili: lead, contatto o è vuoto. Se è vuoto, significa che questo lead Marketo non esiste in SFDC.

## Come determinare se un lead o un contatto viene eliminato in SFDC? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

In Marketo è presente un campo denominato SFDC isDeleted. Se il valore è true, il lead è stato eliminato in SFDC.

## Come posso verificare che un nuovo campo che aggiungo in SFDC venga aggiunto anche a Marketo? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Se desideri un campo in entrambi i sistemi, crealo prima in SFDC e verrà automaticamente sincronizzato con Marketo.

Se aggiungi un nuovo campo in SFDC e l&#39;utente di sincronizzazione dispone dell&#39;autorizzazione per visualizzarlo, verrà aggiunto automaticamente a Marketo.

## Cosa succede se cambio l&#39;etichetta di un campo in SFDC? {#what-if-i-change-a-field-label-in-sfdc}

La modifica dell’etichetta del campo in SFDC non influisce sull’etichetta del campo in Marketo.

## Cosa succede se cambio un tipo di campo in SFDC? {#what-if-i-change-a-field-type-in-sfdc}

Quando si modifica un tipo di campo, Marketo elimina i dati nei campi se non corrispondono (ma visualizza prima un avviso). Per conservare i dati, esportarli e reimportarli dopo aver modificato il tipo di campo.

## Cosa succede se cambio il nome di un&#39;API in SFDC? {#what-if-i-change-an-api-name-in-sfdc}

Se modifichi il nome API di un campo in SFDC, viene creato un nuovo campo in Marketo.

## Cosa succede se aggiungo un nuovo valore di elenco a discesa in SFDC? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Se in SFDC viene aggiunto un nuovo valore dell’elenco a discesa a un campo, Marketo ti invierà una notifica.

## Informazioni sui campi di ricerca SFDC personalizzati {#what-about-custom-sfdc-lookup-fields}

I campi di ricerca in SFDC sincronizzano l&#39;ID ma non il nome di riferimento.

## Informazioni sui campi formula SFDC {#what-about-sfdc-formula-fields}

I campi della formula vengono sincronizzati, tuttavia, gli aggiornamenti ai riferimenti nella formula non vengono sincronizzati fino a quando non viene eseguito un aggiornamento a [Timbro mod di sistema](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US).

## Cosa succede quando elimino un campo da Salesforce che precedentemente era sincronizzato con Marketo? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Se elimini un campo in SFDC, non lo elimina automaticamente in Marketo, ma interrompe la sincronizzazione.
