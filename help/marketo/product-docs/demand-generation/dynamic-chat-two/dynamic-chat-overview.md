---
description: Panoramica del Dynamic Chat - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica del Dynamic Chat
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: b4ba55769034e8fb8a7878f52e21bd08e073fa8c
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 2%

---

# Panoramica del Dynamic Chat {#dynamic-chat-overview}

Il Dynamic Chat ti consente di sfruttare un’interfaccia di facile utilizzo per eseguire il targeting sia delle persone che degli account che visitano il tuo sito web. Raccogli contenuti rilevanti come nome, informazioni di contatto e testo libero. I visitatori del sito possono inoltre prenotare riunioni con il team vendite. I dati relativi all’attività e al coinvolgimento del Dynamic Chat possono essere utilizzati per aggiungere membri ai programmi Marketo e attivare attività cross-channel.

>[!NOTE]
>
>Il Dynamic Chat è in fase di introduzione graduale ed è attualmente in disponibilità limitata. Questa pagina verrà aggiornata con i dettagli sulla disponibilità generale (GA) non appena saranno disponibili.

>[!TIP]
>
>Visita [questa pagina](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) per visualizzare i video tutorial sul Dynamic Chat.

## Integrazioni {#integrations}

Un componente chiave del Dynamic Chat è la sua capacità di interfacciarsi in modo nativo con il tuo abbonamento a Marketo. Per sfruttare appieno le funzionalità di questa integrazione, devi innanzitutto avviare la sincronizzazione dei dati. A seconda delle dimensioni del database Marketo, potrebbero essere necessarie fino a 24 ore per i dati iniziali, [sincronizzazione una tantum](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/connect-dynamic-chat-to-marketo.md) per completare.

Viene sincronizzato quanto segue:

* Dati campo persona
* Dati campo società
* Dati attività

## Dialogo {#dialogues}

Le finestre di dialogo rappresentano un singolo coinvolgimento di chat. Consideralo come un contenitore con tutto il necessario per avere una coinvolgente chat di dialogo con i visitatori del tuo sito web. In ogni finestra di dialogo, puoi specificare su quali pagine visualizzare la finestra di dialogo, a chi desideri mostrarla e il contenuto e il flusso della finestra stessa. Inoltre, puoi trovare metriche per vedere le prestazioni della finestra di dialogo. [Ulteriori informazioni sulle finestre di dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md){target="_blank"}.

## Configurazione {#configuration}

Nella scheda Configurazione, personalizza l’aspetto delle varie finestre di dialogo. Cambia il font, i colori, il tempo di risposta e altro ancora. [Ulteriori informazioni sulla configurazione](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md){target="_blank"}.

## Calendario {#calendar}

Connetti il calendario di Outlook o Gmail per la pianificazione degli appuntamenti nel chatbot. [Ulteriori informazioni sul calendario](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/calendar.md){target="_blank"}

## Riunioni {#meetings}

Qui vengono visualizzati tutti gli appuntamenti pianificati dai visitatori del sito Web tramite le varie finestre di dialogo. [Ulteriori informazioni sulle riunioni](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/meetings.md){target="_blank"}

## Indirizzamento {#routing}

Qui puoi visualizzare un elenco di tutti gli agenti che hanno connesso i loro calendari, l’ordine in cui verranno presentati ai visitatori del sito web e creare regole di indirizzamento personalizzate. [Ulteriori informazioni sull&#39;indirizzamento](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/routing.md){target="_blank"}

## Chat in tempo reale {#live-chat}

Offri ai tuoi visitatori web qualificati di entrare in contatto con i rappresentanti commerciali tramite chat live. COLLEGA A DOCUMENTO

## Domande frequenti {#faq}

**Posso installare il Dynamic Chat in un punto qualsiasi del sito Web della mia azienda o funziona solo sulle pagine di destinazione di Marketo?**

Lo snippet JavaScript di Dynamic Chat può essere installato su qualsiasi sito Web e sulle pagine di destinazione di Marketo.

**Per quanto tempo vengono memorizzati i dati per i rapporti?**

90 giorni (vedere l&#39;elenco completo dei limiti [sotto](#limits-in-dynamic-chat)).

**Il Dynamic Chat consente la chat in diretta?**

No, utilizza solo risposte predeterminate.

**Il Dynamic Chat supporta altre lingue oltre all&#39;inglese?**

Sì. Il Dynamic Chat supporta le seguenti lingue: francese, tedesco, giapponese, spagnolo, italiano, portoghese brasiliano, coreano, cinese semplificato e cinese tradizionale. Per ulteriori informazioni, consulta [sezione successiva](#changing-the-language).

**È supportata la funzionalità AI/NLP?**

La funzionalità AI/NLP non è supportata.

**Come posso eseguire il targeting di persone anonime?**

Nella finestra di dialogo, dovrai utilizzare _L’e-mail della persona è vuota_ attributo.

## Modifica della lingua {#changing-the-language}

Per cambiare la lingua del Dynamic Chat, eseguire la procedura seguente.

>[!IMPORTANT]
>
>La modifica della lingua a livello di profilo cambierà la lingua per _tutto_ Applicazioni Experienci Cloud, non solo Dynamic Chat.

1. Nell’account di Experience Cloud, fai clic sull’icona delle impostazioni e scegli **Preferenze**.

   ![](assets/dynamic-chat-overview-1.png)

1. Fai clic sulla lingua corrente sotto il tuo indirizzo e-mail.

   ![](assets/dynamic-chat-overview-2.png)

1. Scegliere la nuova lingua (la seconda lingua è facoltativa) e fare clic su **Salva**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >Tuttavia, il Dynamic Chat supporta solo le seguenti lingue: inglese, francese, tedesco, giapponese, spagnolo, italiano, portoghese brasiliano, coreano, cinese semplificato e cinese tradizionale.

Quando aggiorni la lingua, tutto ciò che si trova nell’app stessa cambia, tranne le parole che hai popolato personalmente (ad esempio, le risposte in streaming).

## Limiti nel Dynamic Chat {#limits-in-dynamic-chat}

<table>
  <th>Parametro</th>
  <th>Descrizione</th>
  <th>Limite</th>
 <tr>
  <td>Finestre di dialogo totali</td>
  <td>Numero di dialoghi (pubblicati e bozza)</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Calendari totali</td>
  <td>Numero di calendari connessi</td>
  <td>25</td>
 </tr>
 <tr>
  <td>Utenti totali (amministratori e utenti marketing)</td>
  <td>Numero di utenti combinati consentiti per istanza di Dynamic Chat</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Finestre di dialogo pubblicate</td>
  <td>Numero di finestre di dialogo pubblicate salvate</td>
  <td>100</td>
 </tr>
 <tr>
  <td>URL di destinazione per finestra di dialogo</td>
  <td>Numero di URL di destinazione che possono essere aggiunti a una singola finestra di dialogo</td>
  <td>20</td>
 </tr>
 <tr>
  <td>Attributi per finestra di dialogo</td>
  <td>Numero di attributi che possono essere aggiunti ai criteri di pubblico per una singola finestra di dialogo</td>
  <td>100</td>
 </tr>
 <tr>
  <td>Gruppi</td>
  <td>Numero di gruppi che è possibile aggiungere a una singola finestra di dialogo</td>
  <td>10</td>
 </tr>
 <tr>
  <td>Attributi per gruppo</td>
  <td>Numero di attributi che possono essere aggiunti a un gruppo</td>
  <td>10</td>
 </tr>
 <tr>
  <td>Schede</td>
  <td>Numero di schede che possono essere aggiunte all’area di lavoro per finestra di dialogo</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Periodo di conservazione dati lead anonimi</td>
  <td>Durata del periodo di conservazione delle informazioni di un lead anonimo senza alcun coinvolgimento</td>
  <td>90 giorni</td>
 </tr>
 <tr>
  <td>Periodo di conservazione attività obiettivo</td>
  <td>Quantità di tempo in cui i dati dell’attività obiettivo vengono conservati</td>
  <td>24 mesi</td>
 </tr>
 <tr>
  <td>Periodo di conservazione attività documenti</td>
  <td>Quantità di tempo in cui i dati dell'attività del documento vengono conservati</td>
  <td>24 mesi</td>
 </tr>
 <tr>
  <td>Interazione con periodo di conservazione attività finestra di dialogo</td>
  <td>Quantità di tempo di conservazione dei dati dell’attività interazione con il dialogo</td>
  <td>90 giorni</td>
 </tr>
 <tr>
  <td>Periodo di conservazione attività prenotazione riunione</td>
  <td>Quantità di tempo per la prenotazione della riunione memorizzata nel Dynamic Chat</td>
  <td>24 mesi</td>
 </tr>
 <tr>
  <td>Conversazioni coinvolte</td>
  <td>Numero di conversazioni chat che possono essere avviate con i visitatori Web al mese</td>
  <td>250</td>
 </tr>
 <tr>
  <td>Conversazioni attivate</td>
  <td>Numero di conversazioni chat che possono essere mostrate ai visitatori Web al mese</td>
  <td>25,000</td>
 </tr>
</table>
