---
unique-page-id: 14352621
description: Informazioni sulle opzioni di invio - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulle opzioni di invio
exl-id: acdee691-478e-4ffe-90e2-54cf559fa38d
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Informazioni sulle opzioni di invio {#understanding-send-options}

Durante la creazione di una campagna sono disponibili diverse opzioni per la creazione dei passaggi e-mail in [!DNL Sales Connect]. Inoltre, a seconda di dove si trova l’e-mail nella campagna, anche le opzioni sono diverse.

Se si tratta del primo passaggio e del primo giorno della campagna, avrai a disposizione le seguenti opzioni:

![](assets/image2019-10-25-10-43-19.png)

**Scegli quando inviare questa e-mail**

* Questa opzione consente di scegliere l’ora di invio per la prima e-mail della campagna quando la si avvia aggiungendo persone.

**Invia questa e-mail all&#39;ora seguente**

* Quando avvii la campagna aggiungendo persone, l’e-mail verrà pianificata per questo momento.
* Quando si avvia la campagna, è sempre possibile scegliere un nuovo orario di invio.

**Crea un&#39;attività. Invierò io stesso questa e-mail**

* Questa opzione creerà un [!UICONTROL Email Task] (e lo sincronizzerà con [!DNL Salesforce]) che potrai inviare secondo le tue esigenze.
* Dopo aver effettuato questa selezione, quando avvierai la campagna, queste attività verranno messe in coda per te nel centro comandi e nel feed live. Puoi quindi personalizzare e inviare (o pianificare) ogni e-mail prima che esca.

   * Se apri questa attività nella nostra applicazione web, verrà aperta una finestra di composizione con l’indirizzo e-mail del tuo contatto, la riga dell’oggetto dell’e-mail e il modello scelto.
   * Se apri questa attività in [!DNL Gmail] o [!DNL Outlook], verrà aperta una finestra di composizione nativa e verrà popolato in modo dinamico l&#39;indirizzo e-mail del contatto, la riga dell&#39;oggetto dell&#39;e-mail e il modello scelto.

Per qualsiasi giorno/passaggio successivo nella campagna, avrai a disposizione le seguenti opzioni:

**Invia questa e-mail contemporaneamente all&#39;e-mail precedente in questa campagna**

* Questa opzione invia l’e-mail contemporaneamente all’e-mail direttamente prima di essa.
* L’invio avverrà comunque nel giorno a cui è associato.

>[!IMPORTANT]
>
>L’invio di un’e-mail contemporaneamente all’e-mail precedente non è supportato per le e-mail inviate lo stesso giorno. Al contrario, l’e-mail verrà inviata al momento dell’e-mail inviata dal giorno precedente. Se questa opzione è selezionata per un’e-mail il primo giorno della campagna (scelta non consigliata), l’e-mail verrà inviata immediatamente all’inizio della campagna.

**Invia questa e-mail all&#39;ora seguente**

* Quando avvii la campagna aggiungendo persone, l’e-mail verrà pianificata per questo momento.
* Quando si avvia la campagna, è sempre possibile scegliere un nuovo orario di invio.

**Crea un&#39;attività. Invierò io stesso questa e-mail**

* Questa opzione creerà un [!UICONTROL Email Task] (e lo sincronizzerà con [!DNL Salesforce]) che potrai inviare secondo le tue esigenze.
* Dopo aver effettuato questa selezione, quando avvii la campagna, Tout metterà in coda queste attività al centro comandi e nel feed live. Puoi quindi personalizzare e inviare (o pianificare) ogni e-mail prima che esca.

   * Se apri questa attività nella nostra applicazione web, verrà aperta una finestra di composizione con l’indirizzo e-mail del tuo contatto, la riga dell’oggetto dell’e-mail e il modello scelto.
   * Se apri questa attività in [!DNL Gmail] o [!DNL Outlook], verrà aperta una finestra di composizione nativa e verrà popolato in modo dinamico l&#39;indirizzo e-mail del contatto, la riga dell&#39;oggetto dell&#39;e-mail e il modello scelto.

**Invia questa e-mail all&#39;e-mail precedente**

* Questa opzione di invio rappresenta un &quot;follow-up&quot; dell’e-mail precedente e aggiunge il corpo dell’e-mail precedente alla fine di questa e-mail.

