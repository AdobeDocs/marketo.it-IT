---
unique-page-id: 2950578
description: Gestisci dati profilo sociale - Documenti Marketo - Documentazione prodotto
title: Gestisci dati profilo social
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---


# Gestisci dati profilo sociale {#manage-social-profile-data}

Quando un utente interagisce con un&#39;app per social network Marketo [o autorizza il proprio social network a precompilare un modulo Marketo con [social form fill](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), Marketo acquisisce tutti i dati disponibili dal proprio profilo sociale. ](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md) È possibile visualizzare queste informazioni nella [pagina Dettagli persona](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page) oppure aggiungerle come colonna in una [visualizzazione personalizzata di un elenco smart](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List).

La compilazione del modulo social e le app per social network acquisiscono insiemi leggermente diversi di campi; vedete la sezione per ciascuno di questi elementi di seguito.

>[!NOTE]
>
>**Disponibilità**
>
>Non tutti i clienti hanno acquistato questa funzionalità. Per informazioni, contattate il rappresentante commerciale.

## Acquisita tramite Social App {#captured-via-social-app}

A seconda delle impostazioni di privacy della rete e dell&#39;utente, vengono recuperati uno o più di questi campi:

>[!NOTE]
>
>Le informazioni aggiuntive provenienti dai social network vengono visualizzate nella pagina Dettagli persona circa cinque minuti dopo che la persona ha concesso l&#39;autorizzazione.

## Da Twitter: {#from-twitter}

* Nome (analizzato dal nome visualizzato)
* Cognome (analizzato da Nome visualizzato)
* URL foto profilo
* URL pagina profilo
* Portata sociale (numero di follower)

>[!NOTE]
>
>Le app per social network non recuperano l&#39;indirizzo e-mail della persona.

## Da Facebook: {#from-facebook}

* Nome
* Cognome
* URL profilo
* URL foto profilo
* Genere
* Portata sociale (numero di amici)

### Acquisito tramite il modulo Social {#captured-via-social-form-fill}

A seconda delle impostazioni di privacy della rete e dell&#39;utente, vengono recuperati uno o più di questi campi:

>[!CAUTION]
>
>I dati acquisiti dal modulo per social network sovrascrivono i campi corrispondenti a meno che [blocchi gli aggiornamenti a tali campi a livello di modulo](../../../../product-docs/administration/field-management/block-updates-to-a-field.md).

## Da Twitter: {#from-twitter-1}

* Nome (analizzato dal nome visualizzato)
* Cognome (analizzato da Nome visualizzato)
* E-mail

## Da Facebook: {#from-facebook-1}

* Nome
* Cognome
* E-mail
* Data di nascita
* Titolo processo
* Azienda

>[!NOTE]
>
>Il modulo Social acquisisce l&#39;indirizzo *solo* se l&#39;utente lo inserisce nel modulo. Se è necessario l&#39;indirizzo e-mail, è necessario [renderlo un campo obbligatorio nel modulo](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Per acquisire queste informazioni dai moduli, abilitare la funzione di [compilazione del modulo social](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).

>[!NOTE]
>
>**Tubo profondo**
>
>Ulteriori informazioni sull&#39;utilizzo dei moduli nel modulo di approfondimento [Forms](http://docs.marketo.com/display/docs/forms).

