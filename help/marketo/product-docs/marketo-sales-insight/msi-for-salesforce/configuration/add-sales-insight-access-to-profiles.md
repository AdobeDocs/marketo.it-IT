---
description: Aggiungere accesso a informazioni sulle vendite ai profili - Documenti Marketo - Documentazione del prodotto
title: Aggiungi accesso a informazioni sulle vendite nei profili
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Aggiungi accesso a informazioni sulle vendite nei profili {#add-sales-insight-access-to-profiles}

Ecco come creare un profilo con accesso a Sales Insight rimuovendo l’accesso per gli altri profili. Questo è per gli utenti che hanno già installato il [Pacchetto AppExchange Insight vendite](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target=&quot;_blank&quot;}.

>[!IMPORTANT]
>
>Se in precedenza hai concesso l’accesso a Sales Insight a tutti i profili, devi [rimuovi accesso a livello di profilo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target=&quot;_blank&quot;} per utilizzare questo set di autorizzazioni.

## Crea un nuovo profilo per Sales Insight {#create-a-new-profile-for-sales-insight}

Se disponi di un profilo dedicato per gli utenti di Sales Insight, puoi saltare questo passaggio.

1. In Salesforce, vai alla pagina Configurazione.

1. Cerca profili in Ricerca rapida e seleziona la **Profilo** opzione .

1. Fai clic sul pulsante **Nuovo profilo** nella parte superiore della pagina.

1. Scegli un profilo da clonare e assegnargli un nome (ad esempio: Sales Insight User).

1. Fai clic su **Salva** al termine.

## Aggiungere le autorizzazioni Approfondimenti vendite {#add-sales-insight-permissions}

1. Torna all’elenco Profili.

1. Fai clic sul pulsante **Modifica** collegamento per il nuovo profilo appena creato (o qualsiasi altro profilo esistente a cui desideri dare accesso a Sales Insight Access).

1. Nella pagina di modifica, dovrai modificare alcune impostazioni.

   **Per i profili a cui è consentito l’accesso a Sales Insight**:

   * In Impostazioni scheda, modificare le schede Marketo in Predefinito su
   * In Autorizzazioni oggetto personalizzate, selezionare Leggi, Crea, Modifica ed Elimina in Marketo Sales Insight Config (se l’utente deve avere accesso alle impostazioni di configurazione, in genere utilizzate per gli amministratori)

   **Per i profili ai quali non è consentito l’accesso a Sales Insight**:

   * In Impostazioni scheda, modificare le schede Marketo in Tabulazione nascosta
   * In Autorizzazioni oggetto personalizzate, deselezionare Leggi, Crea, Modifica ed Elimina in Marketo Sales Insight Config


1. Fai clic su **Salva** al termine.

## Crea layout per informazioni sulle vendite {#create-layout-for-sales-insight}

1. Vai alla pagina Configurazione, quindi fai clic su **Configurazione app** > **Personalizza** > **Lead** > **Layout di pagina**. Quindi fai clic sul pulsante **Nuovo** pulsante .

1. Clona il layout desiderato e assegna al layout un nome appropriato (ad esempio: Layout Approfondimenti vendite).

1. Fai clic su **Salva** al termine.

1. Ripetere questi passaggi per i layout di pagina Contatti, Opportunità e Account.

## Assegna profilo al layout {#assign-profile-to-layout}

1. Torna alla sezione Layout di pagina e fai clic sul pulsante **Assegnazione layout pagina** pulsante .

1. Seleziona **Modifica assegnazione**.

1. Seleziona il tuo profilo Approfondimenti vendite dall&#39;elenco, quindi seleziona il layout Approfondimenti vendite dal menu a discesa &quot;Seleziona layout pagina&quot;.

1. Fai clic su **Salva** al termine.

1. Ripetere questi passaggi per i layout di pagina Contatti, Opportunità e Account.

## Altre modifiche {#other-changes}

Qui ci sono altri posti in cui potrebbero apparire gli articoli di Insight vendite. Dovrai rimuoverli definitivamente poiché non puoi utilizzare Profili per limitarne l’accesso:

* Rimuovi i pulsanti Approfondimenti vendite da Cerca layout per contatti, lead e account
* Rimuovere le colonne Approfondimenti vendite dagli elenchi Contatti e Lead
