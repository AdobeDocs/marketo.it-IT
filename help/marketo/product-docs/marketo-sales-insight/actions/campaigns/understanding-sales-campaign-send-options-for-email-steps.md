---
description: Informazioni sulle opzioni di invio della campagna di vendita per i passaggi dell’e-mail - Documenti Marketo - Documentazione del prodotto
title: Informazioni sulle opzioni di invio della campagna di vendita per i passaggi dell’e-mail
feature: Sales Insight Actions
exl-id: 775c6401-efb2-4940-a81c-be5d2759c7bd
source-git-commit: 3e1db4c113df7278eadcf1b61ee225989e70452b
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---

# Informazioni sulle opzioni di invio della campagna di vendita per i passaggi dell’e-mail {#understanding-sales-campaign-send-options-for-email-steps}

Durante la creazione di una campagna di vendita, puoi scegliere tra diverse opzioni per la creazione dei passaggi e-mail in Azioni approfondimento vendite. Inoltre, a seconda di dove si trova l’e-mail nella campagna di vendita, anche le opzioni sono diverse.

## Opzioni di invio primo passaggio {#first-step-send-options}

Se si tratta del primo passo e del primo giorno della campagna di vendita, avrai a disposizione le seguenti opzioni:

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

### Scegli quando inviare questa e-mail {#first-step-i-will-choose}

* Questa opzione consente di scegliere l’ora di invio per la prima e-mail della campagna di vendita quando si avvia la campagna aggiungendo persone.

### Invia questa e-mail al seguente orario {#first-step-following-time}

* Quando avvierai la tua campagna di vendita aggiungendo persone, pianificheremo l’e-mail per questo momento.
* È sempre possibile scegliere una nuova fase di invio quando si avvia la campagna di vendita.

### Crea un&#39;attività. Invierò io stesso questa e-mail {#first-step-create-a-task}

* Questa opzione consente di creare un’attività e-mail (e di sincronizzarla con Salesforce) che puoi inviare quando preferisci.
* Dopo aver effettuato questa selezione, quando avvierai la tua campagna di vendita, queste attività verranno messe in coda per te nel centro comandi e nel feed live. Puoi quindi personalizzare e inviare (o pianificare) ogni e-mail prima che esca.

   * Se apri questa attività nella nostra applicazione web, verrà aperta una finestra di composizione con l’indirizzo e-mail del tuo contatto, la riga dell’oggetto dell’e-mail e il modello scelto.
   * Se si apre l&#39;attività in Gmail o Outlook, verrà aperta una finestra di composizione nativa e l&#39;indirizzo di posta elettronica del contatto, l&#39;oggetto dell&#39;e-mail e il modello scelto verranno inseriti in modo dinamico.

## Opzioni di invio passaggio successivo {#subsequent-step-send-options}

Per i giorni/passaggi successivi della campagna di vendita, avrai a disposizione le seguenti opzioni:

### Invia questa e-mail contemporaneamente all&#39;e-mail precedente in questa campagna di vendita {#subsequent-send-at-same-time}

* Questa opzione invia l’e-mail contemporaneamente all’e-mail direttamente prima di essa.
* L’invio avverrà comunque nel giorno a cui è associato.

### Invia questa e-mail al seguente orario {#subsequent-send-at-following-time}

* Quando avvierai la tua campagna di vendita aggiungendo persone, pianificheremo l’e-mail per questo momento.
* È sempre possibile scegliere una nuova fase di invio quando si avvia la campagna di vendita.

### Crea un&#39;attività. Invierò io stesso questa e-mail {#subsequent-create-a-task}

* Questa opzione consente di creare un’attività e-mail (e di sincronizzarla con Salesforce) che puoi inviare quando preferisci.
* Dopo aver effettuato questa selezione, quando avvii la tua campagna di vendita, le azioni di approfondimento sulle vendite metteranno in coda queste attività nel centro comandi e nel feed live. Puoi quindi personalizzare e inviare (o pianificare) ogni e-mail prima che esca.

   * Se apri questa attività nella nostra applicazione web, verrà aperta una finestra di composizione con l’indirizzo e-mail del tuo contatto, la riga dell’oggetto dell’e-mail e il modello scelto.
   * Se si apre l&#39;attività in Gmail o Outlook, verrà aperta una finestra di composizione nativa e l&#39;indirizzo di posta elettronica del contatto, l&#39;oggetto dell&#39;e-mail e il modello scelto verranno inseriti in modo dinamico.

### Crea questa e-mail come follow-up dell’e-mail precedente in questa campagna {#subsequent-create-this-email}

* Abilita questa casella di controllo se desideri che l’e-mail precedente nella campagna di vendita venga aggiunta all’e-mail successiva inviata dalla campagna di vendita.
* Per la copia dell’e-mail aggiunta, il modello e-mail nella campagna di vendita verrà sempre inviato. Eventuali modifiche apportate dall’utente prima dell’invio non verranno incluse nell’invio.

>[!NOTE]
>
>Questa opzione per creare un’e-mail come follow-up sarà disponibile solo in un passaggio e-mail, quando anche il passaggio precedente è un’e-mail. Se il passaggio precedente è Chiama, InMail o Personalizzato, l’opzione per creare un follow-up non viene visualizzata.

>[!MORELIKETHIS]
>
>[Creare una campagna di vendita](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target="_blank"}
>[Tipi di fasi della campagna di vendita e task promemoria](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target="_blank"}
>[Impostazioni campagna di vendita](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target="_blank"}
