---
description: Criteri del pubblico - Documenti Marketo - Documentazione del prodotto
title: Criteri di audience
exl-id: 9b70b03e-229e-469e-bd65-07aaf2dcbec6
source-git-commit: f71ac0398b3a93d2c46201a696dd41e6ccd89000
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 1%

---

# Criteri di audience {#audience-criteria}

Analogamente agli elenchi avanzati di Marketo, gli attributi dei criteri per il pubblico consentono di definire il pubblico di destinazione. Puoi eseguire il targeting di persone conosciute o sconosciute utilizzando attributi dedotti, di persone o di società (o una combinazione di essi).

## Priorità {#priority}

La priorità determina la finestra di dialogo che un lead riceve nel caso in cui si qualifichi per più di uno. È stabilito quando si inizia [crea la finestra di dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}. È possibile modificare la priorità di una finestra di dialogo esistente aprendola e andando a **Dettagli finestra di dialogo** nella scheda Criteri di pubblico .

![](assets/audience-criteria-1.png)

## Eventi {#events}

![](assets/audience-criteria-2.png)

Gli eventi ti consentono di eseguire il targeting dei visitatori in base al loro scorrimento o al loro tempo sulla pagina/sito. Nell’esempio seguente, il targeting è per i visitatori che si trovano su una pagina specifica da più di 20 secondi.

1. Afferra la **Tempo sulla pagina** e trascinarlo a destra.

   ![](assets/audience-criteria-3.png)

1. Impostare il tempo &quot;Maggiore di&quot; su 20 secondi.

   ![](assets/audience-criteria-4.png)

1. Aggiungi l’URL della pagina desiderata nel [Target](#target) sezione .

   ![](assets/audience-criteria-5.png)

## Attributi {#attributes}

![](assets/audience-criteria-6.png)

**Persone conosciute**

Ci sono _molti_ combinazioni di attributi tra cui scegliere. Nell’esempio seguente, eseguiamo il targeting di tutti **persone conosciute** in California che lavorano in un&#39;azienda con più di 50 dipendenti.

1. Afferra la **Stato persona** e trascinalo a destra.

   ![](assets/audience-criteria-7.png)

1. _Is_ è impostato per impostazione predefinita. Nel campo Seleziona valori digitare CA (è inoltre possibile fare clic sul menu a discesa e selezionare dall’elenco).

   ![](assets/audience-criteria-8.png)

1. Afferra la **Dimensione dell&#39;azienda** attributo e trascinalo nel punto in cui dice _trascina un attributo qui_.

   ![](assets/audience-criteria-9.png)

   >[!NOTE]
   >
   >Puoi anche scegliere un attributo facendo clic sui relativi **+** icona.

1. Fai clic sull’elenco a discesa dell’operatore e seleziona **Maggiore di**.

   ![](assets/audience-criteria-10.png)

1. Digitare 50 e fare clic in un altro punto dello schermo per salvare.

   ![](assets/audience-criteria-11.png)

Ed è tutto!

**Persone anonime**

C&#39;è un modo semplice per indirizzare specificamente le persone che non sono ancora nel tuo database. In questo esempio, il targeting è tutto **persone anonime** situato nella zona di New York.

1. Afferra la **E-mail persona** e trascinalo a destra.

   ![](assets/audience-criteria-12.png)

1. Fai clic sull’elenco a discesa dell’operatore e seleziona **È vuoto**.

   ![](assets/audience-criteria-13.png)

1. Afferra la **Stato interessato** attributo e trascinalo nel punto in cui dice _trascina un attributo qui_.

   ![](assets/audience-criteria-14.png)

   >[!NOTE]
   >
   >Quando qualcuno visita il tuo sito web, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) li cookie e li inserisce nel sistema. Cerchiamo il loro IP in un database speciale e dedurre tutti i tipi di buone informazioni.

1. _Is_ è impostato per impostazione predefinita. Nel campo Seleziona valori digitare NY (è inoltre possibile fare clic sull’elenco a discesa e selezionarlo dall’elenco).

   ![](assets/audience-criteria-15.png)

## Aggiungi gruppi {#add-groups}

Hai anche la possibilità di raggruppare gli attributi, nel caso in cui desideri avere tutti gli attributi insieme a &quot;all o any&quot; di un altro. È possibile aggiungere più gruppi.

![](assets/audience-criteria-16.png)

![](assets/audience-criteria-17.png)

## Target {#target}

In questa finestra immetti gli URL su cui desideri visualizzare una finestra di dialogo specifica. Puoi anche aggiungere esclusioni.

Formati accettabili:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>L&#39;utilizzo di un asterisco funge da jolly catch-all. Quindi `https://*.website.com` inserirebbe la finestra di dialogo in ogni pagina del sito, inclusi i sottodomini (ad esempio: `support.website.com`). E `https://website.com/folder/*` inserisce la finestra di dialogo in ogni pagina di HTML nella cartella successiva (ad esempio: in questo caso diciamo che la cartella è &quot;sport&quot;, quindi: website.com/sports/baseball.html, website.com/sports/football.html, ecc.).

**Esclusioni**

Utilizza le esclusioni per assicurarti che la finestra di dialogo funzioni **not** vengono visualizzate in una pagina/area specifica del sito. Le esclusioni seguono lo stesso formato delle inclusioni.

![](assets/audience-criteria-18.png)

>[!MORELIKETHIS]
>
>* [Creare una finestra di dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [Progettazione flussi](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md){target=&quot;_blank&quot;}
>* [Rapporti](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}

