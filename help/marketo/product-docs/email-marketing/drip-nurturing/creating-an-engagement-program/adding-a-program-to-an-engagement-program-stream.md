---
unique-page-id: 10098134
description: Aggiunta di un programma a un flusso di programma di coinvolgimento - Documentazione di Marketo - Documentazione del prodotto
title: Aggiunta di un programma a un flusso di programma di coinvolgimento
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
feature: Engagement Programs
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Aggiunta di un programma a un flusso di programma di coinvolgimento {#adding-a-program-to-an-engagement-program-stream}

## Perché utilizzare un programma nidificato in un flusso di programma di coinvolgimento? {#why-use-a-nested-program-in-an-engagement-program-stream}

È facile aggiungere un’e-mail a un flusso in un programma di coinvolgimento e funziona correttamente. Tuttavia, se le tue esigenze aziendali sono più complesse, potrebbe essere utile inserire l’e-mail all’interno di un programma. Ad esempio, potrebbe essere utile:

* Inviare un messaggio e-mail a un sottogruppo di persone nel flusso
* Invia *diverse* e-mail ai sottogruppi all’interno del flusso
* Includi pagine di destinazione, moduli o altre risorse nell’ambiente di sviluppo
* Abilita attribuzione multi-touch
* Aggiungi passaggi di flusso aggiuntivi, ad esempio e-mail di avviso

## Cosa succede quando si utilizza un programma in un flusso? {#what-happens-when-you-use-a-program-in-a-stream}

Quando si utilizza un programma nidificato, la decisione di inviare un messaggio e-mail a una persona si basa sull’iscrizione al programma e sull’ID del programma.

* Se non sei iscritto a un programma, riceverai tutte le e-mail che fanno parte del programma una volta
* Se sei iscritto al programma, non riceverai l’e-mail
* Se non sei più membro ma hai ricevuto l’e-mail in precedenza tramite quel programma, non riceverai l’e-mail

Quando utilizzi un programma in un flusso, non importa se hai già ricevuto quell’e-mail specifica. Se l&#39;e-mail non è stata inviata prima di *in tale programma specifico*, puoi riceverla nuovamente.

Può ottenere e-mail e programmi di mixaggio complicati in un programma di coinvolgimento. Potrebbe essere utile usare una delle due.

>[!TIP]
>
>Assicurarsi di utilizzare un filtro **[!UICONTROL Member of Engagement Program]** nell&#39;elenco avanzato.

## Cosa succede alle persone che non soddisfano i criteri della lista intelligente? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

Nel caso in cui qualcuno venga escluso dall’elenco avanzato della campagna intelligente di un programma nidificato, non passa alla parte successiva del contenuto durante il cast corrente. Passeranno al contenuto successivo nel flusso per il cast *seguente*.

## Cosa contiene un programma nidificato? {#what-does-a-nested-program-contain}

Un programma nidificato ben progettato contiene e-mail, rapporti e campagne intelligenti. Ha senso tenerle insieme.

L&#39;e-mail utilizzata può essere inserita nel programma, in un altro programma o persino in [!UICONTROL Design Studio]. Il luogo in cui vive dipenderà da come lo si desidera utilizzare.

La generazione di rapporti sulle modifiche con la posizione dell’e-mail. Quindi, ad esempio, se l&#39;e-mail si trova in [!UICONTROL Design Studio], nel Rapporto sulle prestazioni dell&#39;e-mail tutte le metriche sono visualizzate in una riga: i diversi cast vengono combinati. Tuttavia, nel Rapporto sulle prestazioni del flusso di coinvolgimento, i diversi invii vengono visualizzati separatamente.

>[!CAUTION]
>
>Se desideri inviare di nuovo qualcosa, è più sicuro creare un nuovo programma e una campagna intelligente.

>[!MORELIKETHIS]
>
>* [Aggiungi contenuto a un flusso](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Informazioni sui programmi](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
