---
unique-page-id: 2953415
description: Utilizzo della pagina dei dettagli della persona - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo della pagina Dettagli persona
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 22%

---

# Utilizzo della pagina Dettagli persona {#using-the-person-detail-page}

La pagina dei dettagli della persona contiene tutte le informazioni che Marketo conosce su una persona. Puoi modificare i dati direttamente da questa pagina.

## Vai alla pagina dei dettagli della persona {#getting-to-person-detail-page}

Ci sono molti modi per aprire persone specifiche. Alcuni esempi sono:

* Dalla sezione **Database**, è possibile eseguire una ricerca in Ricerca rapida
* Qualsiasi smart **list** o elenco
* **Membri** scheda di un programma
* **Visualizza membri della campagna** in una campagna avanzata
* Alcuni **rapporti**
  <br> 

1. Fai doppio clic su una persona o fai clic sull’ID a sinistra.

   ![](assets/one-1.png)

1. Verrà aperta la schermata dei dettagli della persona.

   ![](assets/two-5.png)

## Organizzazione pagina - Salesforce {#page-organization-salesforce}

Le informazioni sulla persona sono suddivise nelle seguenti schede:

| Linguetta | Descrizione |
|---|---|
| Informazioni | Informazioni di contatto e campi personalizzati su una persona. |
| Informazioni società | Informazioni e indirizzo dell’azienda della persona. |
| Informazioni sull’opportunità | Informazioni sull’opportunità sincronizzate da Salesforce. |
| Campo lead SFDC | Campi Salesforce incorporati. |
| Campo personalizzato SFDC | Campi Salesforce personalizzati. |
| Registro attività | Tutte le attività relative alla persona. |

## Organizzazione pagina - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Linguetta | Descrizione |
|---|---|
| Informazioni | Informazioni di contatto e campi personalizzati su una persona. |
| Informazioni società | Informazioni e indirizzo dell’azienda della persona. |
| Informazioni sull’opportunità | Informazioni sull’opportunità sincronizzate da Microsoft. |
| Campi personalizzati Microsoft | Campi Microsoft personalizzati. |
| Campo lead Microsoft | Campi Microsoft incorporati. |
| Registro attività | Tutte le attività relative alla persona. |

>[!NOTE]
>
>Puoi anche visualizzare le informazioni sull’opportunità [inserito tramite API](https://developers.marketo.com/rest-api/lead-database/opportunities/) per le istanze non sincronizzate con un CRM.

## Modifica di un campo {#editing-a-field}

Molti campi sono modificabili. Per aggiornare le informazioni di una persona, digita un nuovo valore e fai clic all’esterno del campo per salvare.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Campi predefiniti di Marketo prima della sincronizzazione CRM {#marketo-default-fields-prior-to-crm-sync}

|   |  |  |  |  |
|---|---|---|---|---|
| Indirizzo | Entrata annuale | IP anonimo | Indirizzo di fatturazione | Città di fatturazione |
| Paese di fatturazione | Codice postale di fatturazione | Stato di fatturazione | Città | Nome azienda |
| Paese | Data creazione | Data di nascita | Dipartimento | Non effettuare la chiamata |
| Non chiamare causa | Motivo per cui non effettuare la chiamata | Indirizzo e-mail | E-mail non valida | E-mail causa non valida |
| ID azienda esterna | ID dell&#39;addetto alle vendite esterno | Numero di fax | Nome | Nome completo |
| Settore | Città dedotta | Azienda in oggetto | Paese in oggetto | Area metropolitana dedotta |
| Prefisso telefonico dedotto | Codice postale dedotto | Area geografica dello stato dedotta | È anonimo | È cliente |
| È partner | Professione | Cognome | Valutazione | Punteggio |
| Origine persona | Stato | Numero di telefono | Nome visualizzato Marketo Social Facebook | ID Marketo Social Facebook |
| URL foto Marketo Social Facebook | URL profilo Marketo Social Facebook | Marketo Social Facebook Reach | Iscrizioni con riferimenti a Marketo Social Facebook | Visite di riferimento di Marketo Social Facebook |
| Genere social Marketo | Ultima iscrizione riferimento a Marketo Social | Ultima visita di riferimento di Marketo Social | Nome visualizzato Marketo Social LinkedIn | ID Marketo Social LinkedIn |
| URL foto Marketo Social LinkedIn | URL profilo Marketo Social LinkedIn | Marketo Social LinkedIn Reach | Iscrizioni con riferimenti a Marketo Social LinkedIn | Visite di riferimento di Marketo Social LinkedIn |
| ID Marketo Social Syndication | Totale iscrizioni inoltrate Social Marketo | Totale visite inoltrate Social Marketo | Nome visualizzato Marketo Social Twitter | ID Marketo Social Twitter |
| URL foto Marketo Social Twitter | URL profilo Marketo Social Twitter | Marketo Social Twitter Reach | Iscrizioni con riferimenti a Marketo Social Twitter | Visite di riferimento di Marketo Social Twitter |
| Secondo nome | Numero di cellulare | Numero dipendenti | Numero di telefono | Codice postale |
| Priorità | Punteggio relativo | Ruolo | Formula di saluto | Codice SIC (Standard Industrial Classification) |
| Sito | Stato | Annulla l&#39;iscrizione | Motivo di annullamento dell&#39;iscrizione | Data di aggiornamento |
| Urgenza | Sito web |  |  |  |

>[!NOTE]
>
>Alcuni campi sono _non_ modificabile:
>
>* Registro attività
>* Informazioni sull&#39;azienda
>* Opportunità per i contatti SFDC
>* Alcuni campi specifici di Marketo, come Data di creazione e Tipo di origine originale.
>
>Ulteriori informazioni su [Campi gestiti dal sistema](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md).

>[!MORELIKETHIS]
>
>[Creazione di una scheda personalizzata per la pagina Dettagli persona](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
