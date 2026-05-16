---
unique-page-id: 2953461
description: Scopri quali campi di Salesforce vengono sincronizzati con Marketo e come funzionano SFDC Type e isDeleted. Aggiungi prima nuovi campi in Salesforce in modo che vengano sincronizzati automaticamente con Marketo.
title: Sincronizzazione SFDC - Sincronizzazione campi
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/XUKJC6x2gIjkd3wkmeIMKISxR0jBaGu5vHg7ystMI6c
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 430
ht-degree: 0%

---

# Sincronizzazione SFDC: sincronizzazione campo {#sfdc-sync-field-sync}

Marketo sincronizza le informazioni sul campo da [!DNL Salesforce]. Ecco i dettagli.

## Quali campi sono sincronizzati? {#which-fields-are-synced}

Sincronizziamo la maggior parte dei campi standard in SFDC ed eventuali campi personalizzati per i quali l’utente può visualizzare l’autorizzazione di sincronizzazione.

## Come determinare se un record in Marketo è un lead o un contatto in [!DNL Salesforce]? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

In Marketo è presente un campo denominato Tipo SFDC. Possiede tre valori possibili: lead, contatto o vuoto. Se è vuoto, significa che questo lead Marketo non esiste in SFDC.

## Come determinare se un lead o un contatto viene eliminato in SFDC? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

In Marketo è presente un campo denominato SFDC isDeleted. Se il valore è true, il lead è stato eliminato in SFDC.

## Come posso essere sicuro che un nuovo campo che aggiungo in SFDC venga aggiunto anche a Marketo? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Se desideri un campo in entrambi i sistemi, crealo prima in SFDC e verrà automaticamente sincronizzato con Marketo.

Se aggiungi un nuovo campo in SFDC e l’utente di sincronizzazione dispone dell’autorizzazione per visualizzarlo, questo verrà aggiunto automaticamente a Marketo.

## Cosa succede se cambio l’etichetta di un campo in SFDC? {#what-if-i-change-a-field-label-in-sfdc}

La modifica dell’etichetta del campo in SFDC non influisce sull’etichetta del campo in Marketo.

## Cosa succede se si modifica un tipo di campo in SFDC? {#what-if-i-change-a-field-type-in-sfdc}

Quando si modifica un tipo di campo, Marketo elimina i dati nei campi se non corrispondono (ma prima visualizza un avviso). Per conservare i dati, esportarli e importarli nuovamente dopo aver modificato il tipo di campo.

## Cosa succede se cambio il nome di un’API in SFDC? {#what-if-i-change-an-api-name-in-sfdc}

Se modifichi il nome API di un campo in SFDC, viene creato un nuovo campo in Marketo.

## Cosa succede se aggiungo un nuovo valore di elenco a discesa in SFDC? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Se in SFDC a un campo viene aggiunto un nuovo valore per l’elenco a discesa, Marketo ti invierà una notifica.

## Informazioni sui campi di ricerca SFDC personalizzati {#what-about-custom-sfdc-lookup-fields}

I campi di ricerca in SFDC sincronizzano l’ID ma non il nome di riferimento.

## Informazioni sui campi formula di SFDC {#what-about-sfdc-formula-fields}

I campi formula sono sincronizzati, tuttavia, gli aggiornamenti ai riferimenti nella formula non vengono sincronizzati finché non viene eseguito un aggiornamento a [System Mod Stamp](https://help.salesforce.com/apex/HTViewSolution?id=000193203&language=en_US){target="_blank"}.

## Cosa succede quando si elimina un campo da [!DNL Salesforce] che in precedenza era sincronizzato con Marketo? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Se elimini un campo in SFDC, non lo elimina automaticamente in Marketo, ma interrompe la sincronizzazione.
