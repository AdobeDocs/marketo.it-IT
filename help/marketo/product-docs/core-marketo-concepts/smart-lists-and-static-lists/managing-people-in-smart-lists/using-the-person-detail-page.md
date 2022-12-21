---
unique-page-id: 2953415
description: Utilizzo della pagina dei dettagli della persona - Documenti Marketo - Documentazione del prodotto
title: Utilizzo della pagina Dettagli persona
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 19%

---

# Utilizzo della pagina Dettagli persona {#using-the-person-detail-page}

La pagina dei dettagli relativi alla persona contiene tutte le informazioni che Marketo conosce su una persona. Puoi modificare i dati direttamente da questa pagina.

## Passaggio alla pagina dei dettagli della persona {#getting-to-person-detail-page}

Ci sono molti modi per aprire persone specifiche. Alcuni esempi sono:

* Da **Database**, è possibile cercare nella Ricerca rapida
* Qualsiasi intelligente **elenco** o elenco
* **Membri** scheda di un programma
* **Visualizza membri della campagna** in una campagna avanzata
* Alcuni **rapporti**

   <br> 

1. Fai doppio clic su una persona o fai clic sull’ID a sinistra.

   ![](assets/one-1.png)

1. Verrà visualizzata la schermata di dettaglio della persona.

   ![](assets/two-5.png)

## Organizzazione pagina - Salesforce {#page-organization-salesforce}

Le informazioni sulla persona sono suddivise in categorie nelle seguenti schede:

| Scheda | Descrizione |
|---|---|
| Informazioni | Contatta informazioni e campi personalizzati su una persona. |
| Informazioni aziendali | Informazioni e indirizzo aziendali della persona. |
| Informazioni opportunità | Informazioni sulle opportunità sincronizzate da Salesforce. |
| Campo lead SFDC | Campi Salesforce incorporati. |
| Campo personalizzato SFDC | Campi Salesforce personalizzati. |
| Registro attività | Tutte le attività relative alla persona. |

## Organizzazione delle pagine - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Scheda | Descrizione |
|---|---|
| Informazioni | Contatta informazioni e campi personalizzati su una persona. |
| Informazioni aziendali | Informazioni e indirizzo aziendali della persona. |
| Informazioni opportunità | Informazioni sulle opportunità sincronizzate da Microsoft. |
| Campi personalizzati Microsoft | Campi Microsoft personalizzati. |
| Campo lead Microsoft | Campi Microsoft incorporati. |
| Registro attività | Tutte le attività relative alla persona. |

>[!NOTE]
>
>Puoi anche vedere le informazioni sulle opportunità [inserito tramite API](https://developers.marketo.com/rest-api/lead-database/opportunities/) per le istanze che non sono sincronizzate con un CRM.

## Modifica di un campo {#editing-a-field}

Molti campi sono modificabili. Per aggiornare le informazioni di una persona, digitare un nuovo valore e fare clic all&#39;esterno del campo per salvare.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Campi predefiniti di Marketo prima della sincronizzazione CRM {#marketo-default-fields-prior-to-crm-sync}

|  |  |  |  |  |
|---|---|---|---|---|
| Indirizzo | Entrata annuale | IP anonimo | Indirizzo di fatturazione | Città di fatturazione |
| Paese di fatturazione | Codice postale di fatturazione | Stato di fatturazione | Città | Nome azienda |
| Paese | Creato | Data di nascita | Dipartimento | Non effettuare la chiamata |
| Non chiamare causa | Motivo per cui non effettuare la chiamata | Indirizzo e-mail | E-mail non valida | E-mail causa non valida |
| ID società esterna | ID dell&#39;addetto alle vendite esterno | Numero di fax | Nome | Nome completo |
| Settore | Città in oggetto | Azienda in oggetto | Paese in oggetto | oArea metropolitana in oggetto |
| Prefisso telefonico in oggetto | Codice postale in oggetto | Stato in oggetto | È Anonimo | È cliente |
| È partner | Professione | Cognome | Valutazione | Punteggio |
| Origine persona | Stato | Numero di telefono | Nome visualizzato di Marketo Social Facebook | ID Facebook di Marketo Social |
| URL foto di Marketo Social Facebook | URL profilo Facebook di Marketo Social | Raggiungimento di Marketo Social Facebook | Iscrizioni di riferimento Marketo Social Facebook | Visite con riferimento a Marketo Social Facebook |
| Genere sociale Marketo | Ultima registrazione di riferimento di Marketo Social | Ultima visita di riferimento di Marketo Social | Nome visualizzato di Marketo Social LinkedIn | ID LinkedIn di Marketo Social |
| URL foto di Marketo Social LinkedIn | URL profilo LinkedIn di Marketo Social | Raggiungimento di Marketo Social LinkedIn | Iscrizioni di riferimento Marketo Social LinkedIn | Visite con riferimento a Marketo Social LinkedIn |
| ID sindacazione Marketo Social | Iscrizioni totali di riferimento di Marketo Social | Totale visite di riferimento di Marketo Social | Nome visualizzato di Marketo Social Twitter | ID Twitter di Marketo Social |
| URL foto di Marketo Social Twitter | URL profilo Twitter di Marketo Social | Raggiungimento di Marketo Social Twitter | Iscrizioni di riferimento Marketo Social Twitter | Visite con riferimento a Marketo Social Twitter |
| Secondo nome | Numero di cellulare | Numero dipendenti | Numero di telefono | Codice postale |
| Priorità | Punteggio relativo | Ruolo | Formula di saluto | Codice SIC (Standard Industrial Classification) |
| Sito | Stato | Annulla l&#39;iscrizione | Motivo di annullamento dell&#39;iscrizione | Aggiornato a |
| Urgenza | Sito web |  |  |  |

>[!NOTE]
>
>Alcuni campi sono _not_ modificabile:
>
>* Registro attività
>* Informazioni aziendali
>* Opportunità per i contatti della DSC
>* Alcuni campi specifici di Marketo, ad esempio Data creazione e Tipo origine originale.
>
>Ulteriori informazioni [Campi gestiti di sistema](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md).

>[!MORELIKETHIS]
>
>[Creazione di una scheda personalizzata per la pagina Dettagli persona](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
