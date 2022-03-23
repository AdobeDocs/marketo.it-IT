---
description: Criteri del pubblico - Documenti Marketo - Documentazione del prodotto
title: Criteri del pubblico
source-git-commit: 38e65efc50f7f5e7a2a3dbe91035327007475721
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Criteri del pubblico {#audience-criteria}

Analogamente agli elenchi avanzati di Marketo, gli attributi dei criteri per il pubblico consentono di definire il pubblico di destinazione. Puoi eseguire il targeting di persone conosciute o sconosciute utilizzando attributi dedotti, di persone o di società (o una combinazione di essi).

**Persone conosciute**

Ci sono _molti_ combinazioni di attributi tra cui scegliere. In questo esempio il targeting è tutto **persone conosciute** in California che lavorano in un&#39;azienda con più di 50 dipendenti.

1. Afferra la **Stato persona** e trascinalo a destra.

   ![](assets/audience-criteria-1.png)

1. _Is_ è impostato per impostazione predefinita. Nel campo Seleziona valori digitare CA (è inoltre possibile fare clic sul menu a discesa e selezionare dall’elenco).

   ![](assets/audience-criteria-2.png)

1. Afferra la **Dimensione dell&#39;azienda** attributo e trascinalo nel punto in cui dice _trascina un attributo qui_.

   ![](assets/audience-criteria-3.png)

   >[!NOTE]
   >
   >Puoi anche scegliere un attributo facendo clic sui relativi **+** icona.

1. Fai clic sull’elenco a discesa dell’operatore e seleziona **Maggiore di**.

   ![](assets/audience-criteria-4.png)

1. Digitare 50 e fare clic in un altro punto dello schermo per salvare.

   ![](assets/audience-criteria-5.png)

Ed è tutto!

**Persone anonime**

C&#39;è un modo semplice per indirizzare specificamente le persone che non sono ancora nel tuo database. In questo esempio, il targeting è tutto **persone anonime** situato nella zona di New York.

1. Afferra la **E-mail persona** e trascinalo a destra.

   ![](assets/audience-criteria-6.png)

1. Fai clic sull’elenco a discesa dell’operatore e seleziona **È vuoto**.

   ![](assets/audience-criteria-7.png)

1. Afferra la **Stato interessato** attributo e trascinalo nel punto in cui dice _trascina un attributo qui_.

   ![](assets/audience-criteria-8.png)

   >[!NOTE]
   >
   >Quando qualcuno visita il tuo sito web, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) li cookie e li inserisce nel sistema. Cerchiamo il loro IP in un database speciale e dedurre tutti i tipi di buone informazioni.

1. _Is_ è impostato per impostazione predefinita. Nel campo Seleziona valori digitare NY (è inoltre possibile fare clic sull’elenco a discesa e selezionarlo dall’elenco).

   ![](assets/audience-criteria-9.png)

## Aggiungi gruppi {#add-groups}

Hai anche la possibilità di raggruppare gli attributi, nel caso in cui desideri avere tutti gli attributi insieme a &quot;all o any&quot; di un altro. È possibile aggiungere più gruppi.

![](assets/audience-criteria-10.png)

![](assets/audience-criteria-11.png)

## Target {#target}

In questa finestra immetti gli URL su cui desideri visualizzare una finestra di dialogo specifica.

Formati accettabili:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>L&#39;utilizzo di un asterisco funge da jolly catch-all. Quindi `https://*.website.com` inserirebbe la finestra di dialogo in ogni pagina del sito, inclusi i sottodomini (ad esempio: `support.website.com`). E `https://website.com/folder/*` inserisce la finestra di dialogo in ogni pagina di HTML nella cartella successiva (ad esempio: in questo caso diciamo che la cartella è &quot;sport&quot;, quindi: website.com/sports/baseball.html, website.com/sports/football.html, ecc.).

>[!MORELIKETHIS]
>
>* [Creare una finestra di dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [Progettazione flussi](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md){target=&quot;_blank&quot;}
>* [Rapporti](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}

