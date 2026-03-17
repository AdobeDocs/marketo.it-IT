---
unique-page-id: 2950799
description: Scopri i token per personalizzare le pagine di destinazione di Marketo. Utilizza i token per inserire contenuto dinamico e personalizzare l’esperienza.
title: Panoramica dei token
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
feature: Landing Pages
source-git-commit: 031eb5f3ff8aac185ce496664f984a4c745c6e44
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 94%

---

# Panoramica dei token {#tokens-overview}

Un token è una variabile che può essere utilizzata nei passaggi del flusso di campagne avanzate Marketo, nelle e-mail, nelle pagine di destinazione, negli snippet e nelle campagne web.

## Informazioni sui valori predefiniti {#understanding-default-values}

Quando utilizzi un token, desideri anche fornire un valore predefinito. Questo è il testo che appare se una persona non ha un valore nel campo a cui fai riferimento.

![](assets/image2014-12-2-13-3a16-3a48.png)

In questo esempio, l’e-mail indicherà “Saluti, (nome)” o “Congratulazioni” (valore predefinito).

![](assets/two.png)

>[!CAUTION]
>
>Durante l’utilizzo dell’editor e-mail di Marketo, i token non funzionano nella preintestazione, Per utilizzare un token nella preintestazione, devi farlo tramite il tuo HTML in un modello e-mail.

>[!NOTE]
>
>Questo elenco non è esaustivo. I token vengono creati anche per ciascun campo personalizzato disponibile in Marketo.

## Token persona {#person-tokens}

* `{{lead.Acquisition Date}}`
* `{{lead.Acquisition Program Name}}`
* `{{lead.Acquisition Program}}`
* `{{lead.Address}}`
* `{{lead.Anonymous IP}}`
* `{{lead.Black Listed}}`
* `{{lead.City}}`
* `{{lead.Country}}`
* `{{lead.Created At}}`
* `{{lead.Date of Birth}}`
* `{{lead.Department}}`
* `{{lead.Do Not Call}}`
* `{{lead.Do Not Call Reason}}`
* `{{lead.Email Address}}`
* `{{lead.Email Invalid}}`
* `{{lead.Email Invalid Cause}}`
* `{{lead.Fax Number}}`
* `{{lead.First Name}}`
* `{{lead.Full Name}}`
* `{{lead.Id}}`
* `{{lead.Inferred City}}`
* `{{lead.Inferred Company}}`
* `{{lead.Inferred Country}}`
* `{{lead.Inferred Metropolitan Area}}`
* `{{lead.Inferred Phone Area Code}}`
* `{{lead.Inferred Postal Code}}`
* `{{lead.Inferred State Region}}`
* `{{lead.Is Customer}}`
* `{{lead.Is Employee}}`
* `{{lead.Is Partner}}`
* `{{lead.Job Title}}`
* `{{lead.Last Name}}`
* `{{lead.Lead Source}}`
* `{{lead.Marketing Suspended}}`
* `{{lead.Middle Name}}`
* `{{lead.Mobile Phone Number}}`
* `{{lead.Original Referrer}}`
* `{{lead.Original Search Engine}}`
* `{{lead.Original Search Phrase}}`
* `{{lead.Original Source Info}}`
* `{{lead.Original Source Type}}`
* `{{lead.Person Notes}}`
* `{{lead.Phone Number}}`
* `{{lead.Registration Source Info}}`
* `{{lead.Registration Source Type}}`
* `{{lead.Salutation}}`
* `{{lead.SFDC Created Date}}`
* `{{lead.SFDC Is Deleted}}`
* `{{lead.SFDC Type}}`
* `{{lead.Unsubscribed}}`
* `{{lead.Unsubscribed Reason}}`
* `{{lead.Updated At}}`
* I campi persona personalizzati funzionano anche se utilizzi il relativo nome visualizzato, ad esempio `{{lead.Custom Field Name}}`

## Token azienda {#company-tokens}

* `{{Company.Account Owner Email Address}}`
* `{{Company.Address}}`
* `{{Company.Annual Revenue}}`
* `{{Company.City}}`
* `{{Company.Company Name}}`
* `{{Company.Company Notes}}`
* `{{Company.Country}}`
* `{{Company.Industry}}`
* `{{Company.Main Phone}}`
* `{{Company.Num Employees}}`
* `{{Company.Parent Company Name}}`
* `{{Company.Postal Code}}`
* `{{Company.SFDC Account Num}}`
* `{{Company.SFDC Created Date}}`
* `{{Company.SFDC Type}}`
* `{{Company.SIC Code}}`
* `{{Company.Site}}`
* `{{Company.State}}`
* `{{Company.Website}}`
* I campi personalizzati dell’azienda funzionano anche se utilizzi il relativo nome visualizzato, ad esempio. `{{Company.Custom Field Name}}`

## Token campagna {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## Token di sistema {#system-tokens}

>[!NOTE]
>
>Ulteriori informazioni su questi token sono disponibili nel [Glossario dei token di sistema](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## Token di attivazione {#trigger-tokens}

* `{{trigger.Trigger Name}}`
* `{{trigger.Name}}`
* `{{trigger.Link}}`
* `{{trigger.Subject}}`
* `{{trigger.Category}}`
* `{{trigger.Details}}`
* `{{trigger.Web Page}}`
* `{{trigger.Client IP Address}}`
* `{{trigger.Sent By}}`
* `{{trigger.Received By}}`
* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!NOTE]
>
>Consulta ulteriori dettagli sui [token per momenti interessanti](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) in base ai trigger utilizzati in una campagna avanzata.

## Token programma {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## [!UICONTROL My Tokens] {#my-tokens}

[!UICONTROL My Tokens] sono definiti in un programma e iniziano con `{{my.` seguito dal nome creato per il token. Ulteriori informazioni su [I miei token in un programma](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## Token member {#member-token}

I token member vengono utilizzati per inserire valori univoci dai partner di servizi integrati. Un uso comune dei token member è la generazione di URL univoci per i partecipanti al webinar. Ogni persona dispone di un URL univoco per accedere al webinar che può essere inserito utilizzando un token `{{member.webinar url}}`. Il token `{{member.webinar url}}` risolve automaticamente l’URL di conferma univoco della persona generato dal fornitore di servizi.

* `{{member.webinar url}}`

>[!CAUTION]
>
>Il token `{{member.webinar url}}` verrà popolato solo se la campagna avanzata che invia l’e-mail è una risorsa secondaria del programma dell’evento.
