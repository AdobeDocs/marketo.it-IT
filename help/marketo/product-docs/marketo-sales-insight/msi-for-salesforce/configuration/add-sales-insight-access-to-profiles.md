---
description: Aggiungere l’accesso a Sales Insight ai profili - Documenti Marketo - Documentazione del prodotto
title: Aggiungere l’accesso a Sales Insight ai profili
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Aggiungere l’accesso a Sales Insight ai profili {#add-sales-insight-access-to-profiles}

Ecco come creare un profilo con accesso a Sales Insight durante la rimozione dell’accesso per gli altri profili. Questo è per gli utenti che hanno già installato il [Pacchetto di AppExchange di Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>Se in precedenza hai concesso l’accesso a Sales Insight a tutti i profili, devi [rimuovi accesso a livello di profilo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} per utilizzare questo set di autorizzazioni.

## Crea un nuovo profilo per approfondimenti vendite {#create-a-new-profile-for-sales-insight}

Se disponi di un profilo dedicato per gli utenti di Sales Insight, puoi saltare questo passaggio.

1. In Salesforce, vai alla pagina Configurazione.

1. Cerca i profili in Ricerca rapida e seleziona la **Profilo** opzione.

1. Fai clic su **Nuovo profilo** nella parte superiore della pagina.

1. Selezionare un profilo da clonare e assegnargli un nome (ad esempio, Utente Sales Insight).

1. Clic **Salva** al termine.

## Aggiungi autorizzazioni approfondimento vendite {#add-sales-insight-permissions}

1. Torna all’elenco dei profili.

1. Fai clic su **Modifica** un collegamento per il nuovo profilo appena creato (o per qualsiasi altro profilo esistente a cui si desidera concedere l’accesso a Sales Insight).

1. Nella pagina di modifica, dovrai modificare alcune impostazioni.

   **Per i profili che sono autorizzati ad accedere a Sales Insight**:

   * In Impostazioni scheda, modifica le schede di Marketo in Attivato predefinito
   * In Autorizzazioni oggetto personalizzato, seleziona Leggi, Crea, Modifica ed Elimina in Configurazione di Marketo Sales Insight (se l’utente deve avere accesso alle impostazioni di configurazione, solitamente utilizzate per gli amministratori)

   **Per i profili a cui non è consentito l’accesso a Sales Insight**:

   * In Impostazioni scheda, modifica le schede di Marketo in Nascosto per scheda
   * In Autorizzazioni oggetto personalizzate, deseleziona Leggi, Crea, Modifica ed Elimina in Configurazione di Marketo Sales Insight

1. Clic **Salva** al termine.

## Crea layout per approfondimenti vendite {#create-layout-for-sales-insight}

1. Vai alla pagina Configurazione, quindi fai clic su **Configurazione app** > **Personalizza** > **Lead** > **Layout di pagina**. Quindi fai clic su **Nuovo** pulsante.

1. Clona il layout desiderato e assegna al layout un nome appropriato (ad esempio, Layout approfondimenti vendite).

1. Clic **Salva** al termine.

1. Ripetere questi passaggi per i layout di pagina Contatti, Opportunità e Account.

## Assegna profilo a layout {#assign-profile-to-layout}

1. Torna alla sezione Layout di pagina e fai clic su **Assegnazione layout di pagina** pulsante.

1. Seleziona **Modifica assegnazione**.

1. Seleziona il profilo Sales Insight dall’elenco, quindi seleziona il layout Sales Insight dal menu a discesa &quot;Seleziona layout di pagina&quot;.

1. Clic **Salva** al termine.

1. Ripetere questi passaggi per i layout di pagina Contatti, Opportunità e Account.

## Altre modifiche {#other-changes}

Di seguito sono riportati alcuni altri luoghi in cui potrebbero essere visualizzati articoli di approfondimento sulle vendite. Dovrai rimuoverli subito poiché non puoi utilizzare i Profili per limitarne l’accesso:

* Rimuovere i pulsanti Informazioni sulle vendite dai layout di ricerca per Contatti, Lead e Account
* Rimozione delle colonne Sales Insight dagli elenchi Contatti e Lead
