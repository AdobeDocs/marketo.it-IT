---
unique-page-id: 2950799
description: Panoramica dei token - Documenti Marketo - Documentazione del prodotto
title: Panoramica sui token
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# Panoramica sui token {#tokens-overview}

Un token è una variabile che può essere utilizzata nei passaggi di flusso delle campagne smart Marketo, nelle e-mail, nelle pagine di destinazione, negli snippet e nelle campagne Web.

## Informazioni sui valori predefiniti {#understanding-default-values}

Quando utilizzate un token, desiderate anche fornire un valore predefinito. Testo che mostra se una persona non ha un valore per il campo a cui si fa riferimento.

![](assets/image2014-12-2-13-3a16-3a48.png)

In questo esempio, il messaggio e-mail contiene &quot;Saluti, (nome)&quot; o &quot;Saluti, messa in movimento&quot; (valore predefinito).

![](assets/two.png)

>[!CAUTION]
>
>I token non funzionano nella preintestazione quando si utilizza l&#39;editor e-mail di Marketo. Per utilizzare un token nel preheader, deve essere tramite il codice HTML personalizzato in un modello e-mail.

>[!NOTE]
>
>Questo elenco non è esaustivo. I token vengono creati anche per ogni campo personalizzato disponibile in Marketo.

## Token di persona {#person-tokens}

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
* I campi per le persone personalizzate funzionano anche se utilizzate il nome visualizzato, ad esempio `{{lead.Custom Field Name}}`

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
* I campi personalizzati della società funzionano anche se utilizzate il nome visualizzato ad esempio. `{{Company.Custom Field Name}}`

## Token campagna {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## Token di sistema {#system-tokens}

>[!NOTE]
>
>Per ulteriori informazioni su questi token, vedere [Glossario dei token di sistema](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## Token trigger {#trigger-tokens}

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
>Maggiori informazioni sui [token per momenti interessanti](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/tokens-for-interesting-moments.md) in base ai trigger utilizzati in una campagna intelligente.

## Token programma {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## Token personali {#my-tokens}

I miei token sono definiti all&#39;interno di un programma e iniziano con `{{my.` seguito dal nome creato per il token. Ulteriori informazioni su [My Tokens in a program](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## Token membro {#member-token}

I token membri vengono utilizzati per inserire valori univoci dai partner di servizi integrati. Un uso comune dei token membri è quello degli URL univoci per i partecipanti al seminario. Ogni persona dispone di un URL univoco per accedere al webinar che può essere inserito utilizzando un token `{{member.webinar url}}`. Il token `{{member.webinar url}}` risolve automaticamente l&#39;URL di conferma univoco della persona generato dal provider di servizi.

* `{{member.webinar url}}`

>[!CAUTION]
>
>Il token `{{member.webinar url}}` verrà popolato solo se la campagna smart che invia l&#39;e-mail è una risorsa figlia del programma dell&#39;evento.
