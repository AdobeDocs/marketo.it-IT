---
unique-page-id: 2950578
description: Gestire i dati del profilo social - Documentazione di Marketo - Documentazione del prodotto
title: Gestione dati profilo social network
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 5%

---

# Gestione dati profilo social network {#manage-social-profile-data}

Quando qualcuno interagisce con una [app social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md) di Marketo o autorizza il proprio social network a precompilare un modulo di Marketo con [compilazione modulo social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), Marketo acquisisce tutti i dati disponibili dal proprio profilo social. Puoi visualizzare queste informazioni nella [pagina Dettagli persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) oppure aggiungerle come colonna in una [visualizzazione personalizzata di un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

>[!IMPORTANT]
>
>Il 31 luglio 2024 è iniziato il processo di rimozione di questa funzione. Non è più possibile creare nuove risorse. Le risorse esistenti continueranno a funzionare fino al 31 gennaio 2025. [Ulteriori informazioni](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

La compilazione dei moduli social e le app social network acquisiscono set di campi leggermente diversi; vedi la sezione per ciascuno di essi.

>[!AVAILABILITY]
>
>Non tutti gli utenti del Marketo Engage hanno acquistato questa funzionalità. Per ulteriori informazioni, contatta l’Adobe Account Team (il tuo Account Manager).

## Acquisito tramite app social {#captured-via-social-app}

A seconda delle impostazioni della rete e della privacy dell&#39;utente, vengono recuperati uno o più dei seguenti campi:

>[!NOTE]
>
>Le informazioni aggiuntive provenienti dai social network vengono visualizzate nella pagina Dettagli persona circa cinque minuti dopo l’autorizzazione della persona.

## Dal Twitter: {#from-twitter}

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
>I dati acquisiti dal riempimento del modulo social network sovrascrivono i campi corrispondenti a meno che non si [blocchi gli aggiornamenti a tali campi a livello di modulo](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## Dal Twitter: {#from-twitter-1}

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
>Il riempimento del modulo per social network acquisisce l&#39;indirizzo e-mail _solo_ se l&#39;utente lo inserisce nel modulo. Se hai bisogno dell&#39;indirizzo e-mail, dovresti [impostarlo come campo obbligatorio nel modulo](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Per acquisire queste informazioni dai moduli, abilita [compilazione modulo social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
