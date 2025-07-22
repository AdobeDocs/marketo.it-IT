---
unique-page-id: 4719314
description: Mappatura campo Salesforce predefinita - Documentazione Marketo - Documentazione del prodotto
title: Mappatura campo Salesforce predefinita
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 2%

---

# Mappatura campo [!DNL Salesforce] predefinita {#default-salesforce-field-mapping}

Quando sincronizzi inizialmente l’account Marketo Engage con Salesforce, Marketo crea automaticamente queste associazioni tra i campi Salesforce e Marketo incorporati. Marketo sincronizzerà inoltre i campi personalizzati sui lead, gli account, le opportunità e i contatti.

## Campi lead {#lead-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| [!UICONTROL Annual Revenue] | [!UICONTROL Annual Revenue] |
| [!UICONTROL City] | [!UICONTROL City] |
| [!UICONTROL Company] | [!UICONTROL Company Name] |
| [!UICONTROL Converted Date] | [!UICONTROL SFDC Converted Date] |
| [!UICONTROL Country] | [!UICONTROL Country] |
| [!UICONTROL Created Date] | [!UICONTROL SFDC Created Date] |
| [!UICONTROL Description] | [!UICONTROL Person Notes] |
| [!UICONTROL Email] | [!UICONTROL Email Address] |
| [!UICONTROL Fax] | [!UICONTROL Fax Number] |
| [!UICONTROL First Name] | [!UICONTROL First Name] |
| [!UICONTROL Email Opt Out] | [!UICONTROL Unsubscribed] |
| [!UICONTROL Industry] | [!UICONTROL Industry] |
| [!UICONTROL Converted] | [!UICONTROL SFDC Is Converted] |
| [!UICONTROL Deleted] | [!UICONTROL SFDC Is Deleted] |
| [!UICONTROL Last Name] | [!UICONTROL Last Name] |
| [!UICONTROL Lead Source] | [!UICONTROL Source] |
| [!UICONTROL Lead Score] | [!UICONTROL Score] |
| [!UICONTROL Mobile Phone] | [!UICONTROL Mobile Phone Number] |
| [!UICONTROL Employees] | [!UICONTROL Num Employees] |
| [!UICONTROL Phone] | [!UICONTROL Phone Number] |
| [!UICONTROL Zip/Postal Code] | [!UICONTROL Postal Code] |
| [!UICONTROL Rating] | [!UICONTROL Rating] |
| [!UICONTROL Salutation] | [!UICONTROL Salutation] |
| [!UICONTROL State/Province] | [!UICONTROL State] |
| [!UICONTROL Status] | [!UICONTROL Status] |
| [!UICONTROL Street] | [!UICONTROL Address] |
| [!UICONTROL Title] | [!UICONTROL Job Title] |
| [!UICONTROL Website] | [!UICONTROL Website] |

## Campi contatto {#contact-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| [!UICONTROL Birthdate] | [!UICONTROL Date of Birth] |
| [!UICONTROL Created Date] | [!UICONTROL SFDC Created Date] |
| [!UICONTROL Contact Description] | [!UICONTROL Person Notes] |
| [!UICONTROL Email] | [!UICONTROL Email Address] |
| [!UICONTROL Business Fax] | [!UICONTROL Fax Number] |
| [!UICONTROL First Name] | [!UICONTROL First Name] |
| [!UICONTROL Email Opt Out] | [!UICONTROL Unsubscribed] |
| [!UICONTROL Deleted] | [!UICONTROL SFDC Is Deleted] |
| [!UICONTROL Last Name] | [!UICONTROL Last Name] |
| [!UICONTROL Lead Source] | [!UICONTROL Source] |
| [!UICONTROL Lead Score] | [!UICONTROL Score] |
| [!UICONTROL MailingCity] | [!UICONTROL City] |
| [!UICONTROL MailingCountry] | [!UICONTROL Country] |
| [!UICONTROL MailingPostalCode] | [!UICONTROL Postal Code] |
| [!UICONTROL MailingState] | [!UICONTROL State] |
| [!UICONTROL MailingStreet] | [!UICONTROL Address] |
| [!UICONTROL Mobile Phone] | [!UICONTROL Mobile Phone Number] |
| [!UICONTROL Business Phone] | [!UICONTROL Phone Number] |
| [!UICONTROL Salutation] | [!UICONTROL Salutation] |
| [!UICONTROL Title] | [!UICONTROL Job Title] |

## Campi account {#account-fields}

| [!UICONTROL SFDC field] | [!UICONTROL Marketo field] |
|---|---|
| [!UICONTROL Annual Revenue] | [!UICONTROL Annual Revenue] |
| [!UICONTROL Billing City] | [!UICONTROL Billing City] |
| [!UICONTROL Billing Country] | [!UICONTROL Billing Country] |
| [!UICONTROL Billing Zip/Postal Code] | [!UICONTROL Billing Postal Code] |
| [!UICONTROL Billing State/Province] | [!UICONTROL Billing State] |
| [!UICONTROL Billing Street] | [!UICONTROL Billing Address] |
| [!UICONTROL Account Description] | [!UICONTROL Company Notes] |
| [!UICONTROL Industry] | [!UICONTROL Industry] |
| [!UICONTROL Deleted] | [!UICONTROL SFDC Is Deleted] |
| [!UICONTROL Account Name] | [!UICONTROL Company Name] |
| [!UICONTROL Employees] | [!UICONTROL Num Employees] |
| [!UICONTROL Account Phone] | [!UICONTROL Main Phone] |
| [!UICONTROL SIC Code] | [!UICONTROL SIC Code] |
| [!UICONTROL Account Site] | [!UICONTROL Site] |
| [!UICONTROL Account Type] | [!UICONTROL SFDC Type] |
| [!UICONTROL Website] | [!UICONTROL Website] |

## Campi di sistema correlati a [!DNL Salesforce] in Marketo (sola lettura) {#salesforce-related-system-fields-in-marketo-read-only}

Questi campi vengono creati in Marketo ma non possono essere regolati dai clienti.

| Campo | Descrizione |
|---|---|
| ID SFDC | ID [!DNL Salesforce] di 18 caratteri |
| Tipo SFDC | Lead o contatto. Se vuoto, il lead esiste solo come persona in Marketo |
| Data di creazione SFDC | Data di creazione in SFDC (può essere diversa da Creato in Marketo) |
| SFDC eliminato | La persona era in SFDC ma è stata eliminata e ora risiede solo in Marketo |
