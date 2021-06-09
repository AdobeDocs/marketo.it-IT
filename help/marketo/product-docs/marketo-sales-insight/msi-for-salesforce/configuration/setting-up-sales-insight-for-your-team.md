---
description: Impostazione di Sales Insight per il tuo team - Marketo Docs - Documentazione del prodotto
title: Impostazione di Sales Insight per il team
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
source-git-commit: ecceb1a3aff3a2088379f8f4f2ac33e566f90e21
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Impostazione di Sales Insight per il team {#setting-up-sales-insight-for-your-team}

Ecco come creare un profilo con accesso a Sales Insight rimuovendo l’accesso per gli altri profili. Questo è per gli utenti che hanno già installato il [pacchetto di AppExchange di Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md).

## Crea un nuovo profilo per informazioni sulle vendite {#create-a-new-profile-for-sales-insight}

Se disponi di un profilo dedicato per gli utenti di Sales Insight, puoi saltare questo passaggio.

1. In Salesforce, vai alla pagina Configurazione.

1. Cerca profili in Ricerca rapida e seleziona l’opzione **Profilo** .

1. Fai clic sul pulsante **Nuovo profilo** nella parte superiore della pagina.

1. Scegli un profilo da clonare e assegnargli un nome (ad esempio: Sales Insight User).

1. Al termine, fai clic su **Salva**.

## Aggiungere autorizzazioni Approfondimenti vendite {#add-sales-insight-permissions}

1. Torna all’elenco Profili.

1. Fai clic sul collegamento **Modifica** per il nuovo profilo appena creato (o qualsiasi altro profilo esistente a cui desideri dare accesso a Sales Insight Access).

1. Nella pagina di modifica, dovrai modificare alcune impostazioni.

   **Per i profili a cui è consentito l’accesso a Sales Insight**:

   * In Impostazioni scheda, modificare le schede Marketo in Predefinito su
   * In Autorizzazioni oggetto personalizzate, selezionare Leggi, Crea, Modifica ed Elimina in Marketo Sales Insight Config (se l’utente deve avere accesso alle impostazioni di configurazione, in genere utilizzate per gli amministratori)

   **Per i profili ai quali non è consentito l’accesso a Sales Insight**:

   * In Impostazioni scheda, modificare le schede Marketo in Tabulazione nascosta
   * In Autorizzazioni oggetto personalizzate, deselezionare Leggi, Crea, Modifica ed Elimina in Marketo Sales Insight Config


1. Al termine, fai clic su **Salva**.

## Crea layout per informazioni sulle vendite {#create-layout-for-sales-insight}

1. Vai alla pagina Configurazione, quindi fai clic su **Configurazione app** > **Personalizza** > **Lead** > **Layout di pagina**. Quindi fare clic sul pulsante **Nuovo**.

1. Clona il layout desiderato e assegna al layout un nome appropriato (ad esempio: Layout Approfondimenti vendite).

1. Al termine, fai clic su **Salva**.

1. Ripetere questi passaggi per i layout di pagina Contatti, Opportunità e Account.

## Assegna profilo al layout {#assign-profile-to-layout}

1. Torna alla sezione Layout di pagina e fai clic sul pulsante **Assegnazione layout di pagina** .

1. Selezionare **Modifica assegnazione**.

1. Seleziona il tuo profilo Approfondimenti vendite dall&#39;elenco, quindi seleziona il layout Approfondimenti vendite dal menu a discesa &quot;Seleziona layout pagina&quot;.

1. Al termine, fai clic su **Salva**.

1. Ripetere questi passaggi per i layout di pagina Contatti, Opportunità e Account.

## Altre modifiche {#other-changes}

Qui ci sono altri posti in cui potrebbero apparire gli articoli di Insight vendite. Dovrai rimuoverli definitivamente poiché non puoi utilizzare Profili per limitarne l’accesso:

* Rimuovi i pulsanti Approfondimenti vendite da Cerca layout per contatti, lead e account
* Rimuovere le colonne Approfondimenti vendite dagli elenchi Contatti e Lead
