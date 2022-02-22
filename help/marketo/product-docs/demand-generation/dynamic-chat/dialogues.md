---
description: Finestre di dialogo - Documenti Marketo - Documentazione del prodotto
title: Finestre di dialogo
exl-id: 5ec17ad0-6d56-4c06-a6ac-4c5771b2d91d
source-git-commit: 8aaa6f5225f7965228c3472c0cf6beb2259f3642
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---

# Finestre di dialogo {#dialogues}

Le finestre di dialogo sono conversazioni individuali via chat. Scopri come personalizzarle visivamente, determinare quali pagine visualizzano e decidere cosa dicono e chi le visualizza.

## Creare una nuova finestra di dialogo {#create-a-new-dialogue}

1. Fai clic su **Finestre di dialogo**.

   ![](assets/dialogues-1.png)

1. Fai clic sul pulsante **Crea nuovo** pulsante .

   ![](assets/dialogues-2.png)

1. Immettere un nome (la descrizione è facoltativa), impostare il livello di priorità e fare clic su **Salva**.

   ![](assets/dialogues-3.png)

>[!NOTE]
>
>La priorità determina quale finestra di dialogo verrà visualizzata a un visitatore quando si qualificano per più finestre di dialogo contemporaneamente.

## Criteri del pubblico {#audience-criteria}

Analogamente agli elenchi avanzati di Marketo, gli attributi dei criteri per il pubblico consentono di definire il pubblico di destinazione. Puoi eseguire il targeting di persone conosciute o sconosciute utilizzando attributi dedotti, di persone o di società (o una combinazione di essi).

**Persone conosciute**

Ci sono _molti_ combinazioni di attributi tra cui scegliere. In questo esempio il targeting è tutto **persone conosciute** in California che lavorano in un&#39;azienda con più di 50 dipendenti.

1. Afferra la **Stato persona** e trascinalo a destra.

   ![](assets/dialogues-4.png)

1. _Is_ è impostato per impostazione predefinita. Nel campo Seleziona valori digitare CA (è inoltre possibile fare clic sul menu a discesa e selezionare dall’elenco).

   ![](assets/dialogues-5.png)

1. Afferra la **Dimensione dell&#39;azienda** attributo e trascinalo nel punto in cui dice _trascina un attributo qui_.

   ![](assets/dialogues-6.png)

   >[!NOTE]
   >
   >Puoi anche scegliere un attributo facendo clic sui relativi **+** icona.

1. Fai clic sull’elenco a discesa dell’operatore e seleziona **Maggiore di**.

   ![](assets/dialogues-7.png)

1. Digitare 50 e fare clic in un altro punto dello schermo per salvare.

   ![](assets/dialogues-8.png)

Ed è tutto!

**Persone anonime**

C&#39;è un modo semplice per indirizzare specificamente le persone che non sono ancora nel tuo database. In questo esempio, il targeting è tutto **persone anonime** situato nella zona di New York.

1. Afferra la **E-mail persona** e trascinalo a destra.

   ![](assets/dialogues-9.png)

1. Fai clic sull’elenco a discesa dell’operatore e seleziona **È vuoto**.

   ![](assets/dialogues-10.png)

1. Afferra la **Stato interessato** attributo e trascinalo nel punto in cui dice _trascina un attributo qui_.

   ![](assets/dialogues-11.png)

   >[!NOTE]
   >
   >Quando qualcuno visita il tuo sito web, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) li cookie e li inserisce nel sistema. Cerchiamo il loro IP in un database speciale e dedurre tutti i tipi di buone informazioni.

1. _Is_ è impostato per impostazione predefinita. Nel campo Seleziona valori digitare NY (è inoltre possibile fare clic sull’elenco a discesa e selezionarlo dall’elenco).

   ![](assets/dialogues-12.png)

## Aggiungi gruppi {#add-groups}

Hai anche la possibilità di raggruppare gli attributi, nel caso in cui desideri avere tutti gli attributi insieme a &quot;all o any&quot; di un altro. È possibile aggiungere più gruppi.

![](assets/dialogues-13.png)

![](assets/dialogues-14.png)

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

## Progettazione flussi {#stream-designer}

Il designer del flusso contiene diverse schede che è possibile aggiungere per modellare la conversazione di chat.

<table>
 <tr>
  <td><strong>Messaggio</strong></td>
  <td>Utilizzare quando si desidera eseguire un'istruzione senza alcuna risposta necessaria (ad esempio: "Ciao! Tutti gli articoli sono 25% off oggi con codice SAVE25").
</td>
 </tr>
 <tr>
  <td><strong>Domanda</strong></td>
  <td>Utilizzare quando si desidera porre una domanda a scelta multipla, di cui fornire le risposte disponibili (ad esempio: A che tipo di veicolo ti interessa? Risposte = SUV, compatto, camion, ecc.).</td>
 </tr>
 <tr>
  <td><strong>Acquisizione delle informazioni</strong></td>
  <td>Utilizza quando desideri raccogliere informazioni. I tre campi tra cui scegliere sono Indirizzo e-mail, Numero di telefono e Testo (che consente al visitatore di scrivere il proprio messaggio).</td>
 </tr>
 <tr>
  <td><strong>Scheduler appuntamenti</strong></td>
  <td>Fornisce al visitatore un calendario delle date disponibili per pianificare un follow-up. La disponibilità del calendario riflette <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">l'agente successivo in linea</a>.</td>
 </tr>
 <tr>
  <td><strong>Obiettivo</strong></td>
  <td>Questa è l'unica carta che i visitatori non vedranno. Sta a te determinare a quale punto un obiettivo viene raggiunto all'interno della chat specifica (es: se la raccolta dell'e-mail del visitatore è l'obiettivo, posiziona la scheda Obiettivo subito dopo l'acquisizione delle informazioni nello streaming).</td>
 </tr>
</table>

**Creare un flusso**

Ci sono _molti_ possibili combinazioni di flussi. Vediamo un esempio [nel presente articolo](/help/marketo/product-docs/demand-generation/dynamic-chat/create-a-stream.md).

## Rapporti {#reports}

Nella scheda Rapporti , visualizza i dati degli ultimi 90 giorni. Ogni categoria è definita di seguito.

<table>
 <tr>
  <td><strong>Totale attivato</strong></td>
  <td>Viene incrementato ogni volta che un visitatore si qualifica o visualizza una finestra di dialogo.
</td>
 </tr>
 <tr>
  <td><strong>Coinvolto</strong></td>
  <td>Viene incrementato ogni volta che un visitatore fa clic sull’ancoraggio del chatbot per aprire la finestra di dialogo.</td>
 </tr>
 <tr>
  <td><strong>Completato</strong></td>
  <td>Viene incrementato ogni volta che un visitatore raggiunge la fine di un ramo in una finestra di dialogo.</td>
 </tr>
 <tr>
  <td><strong>Persone catturate</strong></td>
  <td>Viene incrementato ogni volta che un visitatore fornisce un indirizzo e-mail valido in un flusso di dialogo.</td>
 </tr>
 <tr>
  <td><strong>Riunioni prenotate</strong></td>
  <td>Incrementa ogni volta che un visitatore pianifica correttamente un appuntamento tramite il chatbot.</td>
 </tr>
 <tr>
  <td><strong>Obiettivi raggiunti</strong></td>
  <td>Incrementa ogni volta che un visitatore raggiunge un obiettivo in qualsiasi flusso di dialogo.</td>
 </tr>
</table>

>[!MORELIKETHIS]
>
>[Creare un flusso](/help/marketo/product-docs/demand-generation/dynamic-chat/create-a-stream.md)
