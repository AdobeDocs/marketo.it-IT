---
unique-page-id: 2950578
description: Gestisci dati profilo sociale - Documenti Marketo - Documentazione prodotto
title: Gestisci dati profilo social
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---


# Gestisci dati profilo social {#manage-social-profile-data}

Quando un utente interagisce con un&#39;app [](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)per social network Marketo o autorizza il proprio social network a precompilare un modulo Marketo con il modulo per [](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)social network, Marketo acquisisce tutti i dati disponibili dal proprio profilo sociale. Potete visualizzare queste informazioni nella pagina [Dettagli](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page)persona o aggiungerle come colonna in una visualizzazione [personalizzata di un elenco](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List)avanzato.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

La compilazione del modulo social e le app per social network acquisiscono insiemi leggermente diversi di campi; vedete la sezione per ciascuno di questi elementi di seguito.

>[!NOTE]
>
>**Disponibilità**
>
>Non tutti i clienti hanno acquistato questa funzionalità. Per informazioni, contattate il rappresentante commerciale.

## Acquisita tramite app social {#captured-via-social-app}

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

### Acquisita tramite compilazione modulo social {#captured-via-social-form-fill}

A seconda delle impostazioni di privacy della rete e dell&#39;utente, vengono recuperati uno o più di questi campi:

>[!CAUTION]
>
>I dati acquisiti dal modulo per social network sovrascrivono i campi corrispondenti a meno che non vengano [bloccati gli aggiornamenti a tali campi a livello](../../../../product-docs/administration/field-management/block-updates-to-a-field.md)di modulo.

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
>Il modulo Social acquisisce l&#39;indirizzo e-mail *solo* se l&#39;utente lo inserisce nel modulo. Se è necessario utilizzare l&#39;indirizzo e-mail, è necessario [renderlo un campo obbligatorio nel modulo](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!NOTE]
>
>**Articoli correlati**
>
>Per acquisire queste informazioni dai moduli, abilitare la compilazione [del modulo](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)social.

>[!NOTE]
>
>**Tubo profondo**
>
>Ulteriori informazioni sull&#39;uso dei moduli nel modulo [Forms](http://docs.marketo.com/display/docs/forms) deep approfondimenti.

