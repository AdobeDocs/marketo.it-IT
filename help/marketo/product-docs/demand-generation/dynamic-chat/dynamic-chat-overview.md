---
description: Panoramica del Dynamic Chat - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica del Dynamic Chat
feature: Dynamic Chat
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: be1ca409642fd5d81d341fbadaff38c268fe198f
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 2%

---

# Panoramica del Dynamic Chat {#dynamic-chat-overview}

Il Dynamic Chat ti consente di sfruttare un’interfaccia di facile utilizzo per eseguire il targeting sia delle persone che degli account che visitano il tuo sito web. Raccogli contenuti rilevanti come nome, informazioni di contatto e testo libero. I visitatori del sito possono anche chattare con un agente live e persino prenotare riunioni con il team di vendita. I dati relativi all’attività e al coinvolgimento del Dynamic Chat possono essere utilizzati per aggiungere membri ai programmi Marketo e attivare attività cross-channel.

>[!TIP]
>
>Visita [questa pagina](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html){target="_blank"} per visualizzare i video tutorial sul Dynamic Chat.

## Integrazioni {#integrations}

Un componente chiave del Dynamic Chat è la sua capacità di interfacciarsi in modo nativo con il tuo abbonamento a Marketo. Per sfruttare appieno le funzionalità di questa integrazione, devi innanzitutto avviare la sincronizzazione dei dati. A seconda delle dimensioni del database Marketo, potrebbero essere necessarie fino a 24 ore per i dati iniziali, [sincronizzazione una tantum](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md){target="_blank"} per completare.

Viene sincronizzato quanto segue:

* Dati campo persona
* Dati campo società
* Dati attività

## Dialogo {#dialogues}

Le finestre di dialogo rappresentano un singolo coinvolgimento di chat. Consideralo come un contenitore con tutto il necessario per avere una coinvolgente chat di dialogo con i visitatori del tuo sito web. In ogni finestra di dialogo, puoi specificare su quali pagine visualizzare la finestra di dialogo, a chi desideri mostrarla e il contenuto e il flusso della finestra stessa. Inoltre, puoi trovare metriche per vedere le prestazioni della finestra di dialogo. [Ulteriori informazioni sulle finestre di dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/dialogue-overview.md){target="_blank"}.

## Configurazione {#configuration}

Nella scheda Configurazione, personalizza l’aspetto delle varie finestre di dialogo. Cambia il font, i colori, il tempo di risposta e altro ancora. [Ulteriori informazioni sulla configurazione](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/configuration.md){target="_blank"}.

## Calendario {#calendar}

Connetti il calendario di Outlook o Gmail per la pianificazione degli appuntamenti nel chatbot. [Ulteriori informazioni sul calendario](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md#connect-calendar){target="_blank"}

## Riunioni {#meetings}

Qui vengono visualizzati tutti gli appuntamenti pianificati dai visitatori del sito Web tramite le varie finestre di dialogo. [Ulteriori informazioni sulle riunioni](/help/marketo/product-docs/demand-generation/dynamic-chat/meeting-list.md){target="_blank"}

## Indirizzamento {#routing}

Qui puoi visualizzare un elenco di tutti gli agenti che hanno connesso i loro calendari, l’ordine in cui verranno presentati ai visitatori del sito web e creare regole di indirizzamento personalizzate. [Ulteriori informazioni sull&#39;indirizzamento](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/routing.md){target="_blank"}

## Chat live {#live-chat}

Offri ai visitatori web qualificati di entrare in contatto con i rappresentanti commerciali tramite [chat in diretta](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md){target="_blank"}.

## Flussi conversazionali {#conversational-flow}

[Progettare una conversazione](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-overview.md){target="_blank"} che può essere attivata da un visitatore in base a un’azione designata (ad esempio la compilazione di un modulo, il clic su un collegamento e così via).

## IA generativa {#generative-ai}

[IA generativa](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/overview.md){target="_blank"} in Adobi Dynamic Chat elabora in tempo reale segnali di intento, preferenze dell’utente e comportamenti passati per generare messaggi pertinenti e personalizzati per i visitatori della chat.

## Modifica della lingua {#changing-the-language}

Per cambiare la lingua del Dynamic Chat, attenersi alla procedura descritta di seguito.

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

## Limiti Dynamic Chat di conservazione dei dati {#dynamic-chat-data-retention-limits}

Di seguito sono riportati solo alcuni dei limiti/parametri all’interno di Dynamic Chat. Per un elenco completo, consultare il Marketo Engage [Pagina di descrizione prodotto](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}.

<table>
  <th>Tipo di dati</th>
  <th>Periodo di conservazione</th>
 <tr>
  <td>Lead anonimo senza alcun coinvolgimento</td>
  <td>90 giorni</td>
 </tr>
 <tr>
  <td>Attività obiettivo</td>
  <td>24 mesi</td>
 </tr>
 <tr>
  <td>Attività documento</td>
  <td>24 mesi</td>
 </tr>
 <tr>
  <td>Interazione con attività finestra di dialogo</td>
  <td>90 giorni</td>
 </tr>
 <tr>
  <td>Attività prenotazione riunioni</td>
  <td>24 mesi</td>
 </tr>
</table>

## Domande frequenti {#faq}

Consulta la sezione [Domande frequenti sul Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/faq.md){target="_blank"}.
