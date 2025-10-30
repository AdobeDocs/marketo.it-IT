---
solution: Marketo Engage
product: marketo
title: Importazione modello
description: Scopri come importare i modelli e-mail esistenti dall’editor classico nel nuovo E-mail Designer.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: f5f5e256631b09937d97d7b70f9475f2c286676d
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Importazione modello {#template-import}

Importa facilmente i modelli e-mail esistenti dall’editor classico al nuovo Designer e-mail, mantenendo le progettazioni e accelerando la creazione dei modelli con strutture familiari e riutilizzabili.

1. Passare a **Design Studio**.

   SCHERMATA

1. Fai clic su **Modelli e-mail** e seleziona **Modelli e-mail (nuovi)**.

   SCHERMATA

1. Fare clic su **Crea modello**.

   SCHERMATA

1. Immettere un _Nome_ e (facoltativo) _Descrizione_.

   SCHERMATA

1. Fai clic su **Modelli Marketo** e scegli i modelli esistenti creati nell&#39;editor e-mail classico.

   SCHERMATA

   >[!NOTE]
   >
   >È possibile importare solo i modelli approvati e i modelli condivisi con l&#39;area di lavoro corrente.

1. Seleziona il modello desiderato.

   SCHERMATA

1. Fare clic su Usa questo modello.

   SCHERMATA

1. Il modello importato viene aperto in E-mail Designer.

1. Rivedi i componenti per una conversione corretta e apporta le eventuali modifiche desiderate utilizzando il Designer. Quando sei soddisfatto del modello, approvalo per l’utilizzo nelle e-mail.

## Creare i frammenti {#create-fragments}

È consigliabile creare frammenti di sezioni ripetibili da utilizzare in un secondo momento.

1. Fai clic sul pulsante **...More** in alto e seleziona **Salva come frammento**.

   SCHERMATA

1. Selezionare un componente o una struttura e fare clic su **Crea**.

   SCHERMATA

1. Immettere un nome (con descrizione facoltativa) e fare clic su **Salva**.

   SCHERMATA

## Best practice {#best-practices}

* Poiché il HTML freestyle può variare in modo significativo, l&#39;importatore potrebbe non sempre interpretare perfettamente ogni componente. Esamina i modelli importati per assicurarti che tutte le sezioni siano modificabili e mappate correttamente. Se una parte non è selezionabile, è sufficiente ricrearla per ottenere risultati ottimali.

* Dopo l’importazione, puoi salvare le sezioni riutilizzabili come frammenti e approvarle per l’utilizzo da parte degli autori di e-mail. Applica i temi del brand per mantenere coerenza e conformità.

* Puoi continuare a utilizzare gli script Velocity e considerare la possibilità di reimplementare snippet meno recenti utilizzando una combinazione di frammenti e contenuto condizionale per migliorare la flessibilità e il controllo.

<table><thead>
  <tr>
    <th>Limitazione</th>
    <th>Motivo</th>
    <th>Rimedio</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Le variabili definite nell’editor e-mail classico non sono disponibili a livello di e-mail.</td>
    <td>Le variabili sono state originariamente progettate per semplificare la modifica delle e-mail quando l’editor non offriva ancora le funzionalità di WYSIWYG. In E-mail Designer, gli utenti possono ottenere una flessibilità simile tramite i controlli disponibili. L’importazione mantiene la struttura e i componenti del modello esistente, consentendoti di ricrearlo in modo efficiente nel Designer e-mail.</td>
    <td>Gli utenti dovrebbero essere in grado di ottenere questo risultato in Designer. <p>
    Per i moduli, puoi salvare diversi segmenti come frammenti. I frammenti approvati saranno disponibili per l’utilizzo a livello di e-mail.</td>
  </tr>
  <tr>
    <td>Se il HTML di origine contiene blocchi nidificati, i livelli più profondi non sono indirizzabili in Designer.</td>
    <td>E-mail Designer non supporta i commenti nidificati.</td>
    <td>Anche se Designer non consente la modifica delle strutture nidificate, dovrebbe eseguire il rendering con precisione. Verifica prima il modello.<p>
    Ricrea la struttura utilizzando Griglia.</td>
  </tr>
  <tr>
    <td>A volte i pulsanti vengono importati come contenitori semplici con testo all’interno.</td>
    <td>Alcuni degli stili di implementazione che utilizzano HTML possono essere fraintesi durante l’importazione.</td>
    <td>Ricrea il pulsante in Designer.</td>
  </tr>
  <tr>
    <td>A volte i pulsanti possono essere di dimensioni eccessive.</td>
    <td>Conflitto tra il file CSS del messaggio di posta elettronica di Marketo e altri elementi di livello inferiore (<code>&lt;span&gt;</code>)</td>
    <td>Provare a regolare i margini e le impronte del pulsante in Designer.</td>
  </tr>
  <tr>
    <td>I punti elenco non sono supportati in modalità nativa.</td>
    <td>Al momento, E-mail Designer non offre punti elenco.</td>
    <td>Prendere in considerazione la reimplementazione dei punti elenco utilizzando tecniche alternative.</td>
  </tr>
  <tr>
    <td>L’allineamento verticale viene distorto se il contenuto del contenitore non rispetta il valore dell’attributo valign.</td>
    <td><code>valign</code> non funziona all’interno dei contenitori definiti nel modello.</td>
    <td>Prova a regolare i margini e le spaziature del pulsante in E-mail Designer.</td>
  </tr>
  <tr>
    <td>I token Personalization (I miei token) a livello di programma a livello di modello possono causare errori di convalida.</td>
    <td>I modelli e-mail non supportano i token a livello di programma.</td>
    <td>Sostituiscili con altri tipi di token all’interno dei modelli e sostituiscili con I miei token all’interno delle singole e-mail.</td>
  </tr>
  <tr>
    <td>I componenti divisore potrebbero non essere selezionabili.</td>
    <td>I componenti divisore non sono inclusi nella release.</td>
    <td>n/d</td>
  </tr>
  <tr>
    <td>Se la HTML originale ha strutture mal formate, è probabile che vengano riportate.</td>
    <td>Problemi con il HTML originale.</td>
    <td>I problemi devono essere risolti prima dell’importazione.</td>
  </tr>
  <tr>
    <td>Per il contenuto importato, l’utilizzo dell’anteprima del contenuto non è un indicatore affidabile.</td>
    <td>La funzione di anteprima di Designer non supporta HTML personalizzati.</td>
    <td>È consigliabile verificare l'indirizzo e-mail utilizzando l'opzione <b>Invia bozza</b> nella schermata <i>Simula contenuto</i>.</td>
  </tr>
  <tr>
    <td>I frammenti nel vecchio modello non funzioneranno in E-mail Designer.</td>
    <td>E-mail Designer non supporta snippet.</td>
    <td>Implementa nuovamente i frammenti come frammenti associati a contenuto condizionale.</td>
  </tr>
</tbody></table>
