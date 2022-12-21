---
unique-page-id: 2950578
description: Gestire i dati del profilo social - Documenti Marketo - Documentazione del prodotto
title: Gestisci dati profilo social
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 5%

---

# Gestisci dati profilo social {#manage-social-profile-data}

Quando qualcuno interagisce con un Marketo [app social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)o autorizza il loro social network a precompilare un modulo Marketo con [compilazione del modulo social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), Marketo acquisisce tutti i dati disponibili dal loro profilo social. Puoi visualizzare queste informazioni nella [Pagina Dettagli persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)oppure aggiungilo come colonna in una [visualizzazione personalizzata di un elenco smart](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

La compilazione del modulo social e le app social acquisiscono set di campi leggermente diversi; consulta la sezione per ciascuno di essi di seguito.

>[!AVAILABILITY]
>
>Non tutti i clienti hanno acquistato questa funzionalità. Contatta il tuo rappresentante commerciale per i dettagli.

## Acquisita tramite app social {#captured-via-social-app}

A seconda delle impostazioni di privacy della rete e dell’utente, viene recuperato uno o più di questi campi:

>[!NOTE]
>
>Le informazioni aggiuntive provenienti dai social network vengono visualizzate nella pagina Dettagli persona circa cinque minuti dopo l&#39;autorizzazione della persona.

## Da Twitter: {#from-twitter}

* Nome (analizzato dal nome visualizzato)
* Cognome (analizzato da Nome visualizzato)
* URL foto profilo
* URL della pagina del profilo
* Portata sociale (numero di follower)

>[!NOTE]
>
>Le app social non recuperano l&#39;indirizzo e-mail della persona.

## Da Facebook: {#from-facebook}

* Nome
* Cognome
* URL profilo
* URL foto profilo
* Genere
* Social reach (numero di amici)

### Acquisita tramite compilazione modulo social {#captured-via-social-form-fill}

A seconda delle impostazioni di privacy della rete e dell’utente, viene recuperato uno o più di questi campi:

>[!CAUTION]
>
>I dati acquisiti dal modulo social sovrascrivono i campi corrispondenti a meno che [bloccare gli aggiornamenti a tali campi a livello di modulo](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## Da Twitter: {#from-twitter-1}

* Nome (analizzato dal nome visualizzato)
* Cognome (analizzato da Nome visualizzato)
* E-mail

## Da Facebook: {#from-facebook-1}

* Nome
* Cognome
* E-mail
* Data di nascita
* Qualifica
* Azienda

>[!NOTE]
>
>La compilazione del modulo social acquisisce l&#39;indirizzo e-mail _only_ se l’utente lo inserisce nel modulo. Se hai bisogno dell’indirizzo e-mail, devi [renderlo un campo obbligatorio nel modulo](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Per acquisire queste informazioni dai moduli, abilita [compilazione del modulo social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
