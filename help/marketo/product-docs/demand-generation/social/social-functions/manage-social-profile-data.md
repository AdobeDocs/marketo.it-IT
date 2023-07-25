---
unique-page-id: 2950578
description: Gestire i dati del profilo social - Documentazione di Marketo - Documentazione del prodotto
title: Gestione dati profilo social network
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 5%

---

# Gestione dati profilo social network {#manage-social-profile-data}

Quando qualcuno interagisce con un Marketo [app social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md), o autorizza il proprio social network a precompilare un modulo Marketo con [compilazione modulo social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), Marketo acquisisce tutti i dati disponibili dal loro profilo social. È possibile visualizzare queste informazioni su [Pagina Dettagli persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)o aggiungerlo come colonna in una [visualizzazione personalizzata di un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

Il riempimento dei moduli social e le app social network acquisiscono set di campi leggermente diversi; vedi la sezione per ciascuno di essi.

>[!AVAILABILITY]
>
>Questa funzionalità non è stata acquistata da tutti i clienti. Per ulteriori informazioni, contatta il tuo rappresentante commerciale.

## Acquisito tramite app social {#captured-via-social-app}

A seconda delle impostazioni della rete e della privacy dell&#39;utente, vengono recuperati uno o più dei seguenti campi:

>[!NOTE]
>
>Le informazioni aggiuntive provenienti dai social network vengono visualizzate nella pagina Dettagli persona circa cinque minuti dopo l’autorizzazione della persona.

## Da Twitter: {#from-twitter}

* Nome (analizzato da Nome visualizzato)
* Cognome (analizzato da Nome visualizzato)
* URL foto profilo
* URL della pagina profilo
* Portata social (numero di follower)

>[!NOTE]
>
>Le app social non recuperano l’indirizzo e-mail della persona.

## Da Facebook: {#from-facebook}

* Nome
* Cognome
* URL profilo
* URL foto profilo
* Genere
* Portata social (numero di amici)

### Acquisito tramite riempimento modulo social network {#captured-via-social-form-fill}

A seconda delle impostazioni della rete e della privacy dell&#39;utente, vengono recuperati uno o più dei seguenti campi:

>[!CAUTION]
>
>I dati acquisiti dal riempimento del modulo social network sovrascrivono i campi corrispondenti a meno che tu non [blocca gli aggiornamenti a tali campi a livello di modulo](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## Da Twitter: {#from-twitter-1}

* Nome (analizzato da Nome visualizzato)
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
>Il riempimento di un modulo social acquisisce l’indirizzo e-mail _solo_ se la persona lo inserisce nel modulo. Se hai bisogno dell’indirizzo e-mail, devi [impostalo come campo obbligatorio nel modulo](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Per acquisire queste informazioni dai moduli, abilita [compilazione modulo social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
