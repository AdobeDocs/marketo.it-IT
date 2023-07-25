---
unique-page-id: 2950799
description: Panoramica dei token - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica dei token
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Panoramica dei token {#tokens-overview}

Un token è una variabile che può essere utilizzata nei passaggi di flusso di campagne intelligenti Marketo, nelle e-mail, nelle pagine di destinazione, nei frammenti e nelle campagne web.

## Informazioni sui valori predefiniti {#understanding-default-values}

Quando utilizzi un token, desideri anche fornire un valore predefinito. Questo è il testo che mostra se una persona non ha un valore per il campo a cui stai facendo riferimento.

![](assets/image2014-12-2-13-3a16-3a48.png)

In questo esempio, l’e-mail indicherà &quot;Saluti, (nome)&quot; o &quot;Saluti, terra&quot; (valore predefinito).

![](assets/two.png)

>[!CAUTION]
>
>I token non funzionano nella preintestazione quando si utilizza l’editor e-mail di Marketo. Per utilizzare un token nella preintestazione, devi usare il tuo HTML in un modello e-mail.

>[!NOTE]
>
>Questo elenco non è esaustivo. Vengono creati anche token per ogni campo personalizzato disponibile in Marketo.

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
* I campi personalizzati della persona funzionano anche se utilizzi il loro nome visualizzato, ad esempio `{{lead.Custom Field Name}}`

## Token società {#company-tokens}

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
* I campi personalizzati dell’azienda funzionano anche se utilizzi il nome visualizzato, ad esempio. `{{Company.Custom Field Name}}`

## Token campagna {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## Token di sistema {#system-tokens}

>[!NOTE]
>
>Per ulteriori informazioni su questi token, consulta [Glossario dei token di sistema](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## Attiva token {#trigger-tokens}

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
>Ulteriori dettagli su [token per momenti interessanti](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) in base ai trigger utilizzati in una campagna intelligente.

## Token programma {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## I miei token {#my-tokens}

I miei token sono definiti all&#39;interno di un programma e iniziano con `{{my.` seguito dal nome creato per il token. Ulteriori informazioni su [I miei token in un programma](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## Token membro {#member-token}

I token dei membri vengono utilizzati per inserire valori univoci dai partner di servizi integrati. Un uso comune dei token di membro è quello di URL univoci per i partecipanti al webinar. Ogni persona ha un URL univoco per accedere al webinar, che può essere inserito utilizzando un `{{member.webinar url}}` token. Il `{{member.webinar url}}` Il token risolve automaticamente l’URL univoco di conferma della persona generato dal provider di servizi.

* `{{member.webinar url}}`

>[!CAUTION]
>
>Il `{{member.webinar url}}` il token viene popolato solo se la campagna avanzata che invia l’e-mail è una risorsa secondaria del programma dell’evento.
