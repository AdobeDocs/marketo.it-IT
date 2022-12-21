---
unique-page-id: 10098134
description: Aggiunta di un programma a un flusso di programmi di coinvolgimento - Marketo Docs - Documentazione del prodotto
title: Aggiunta di un programma a un flusso del programma di coinvolgimento
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Aggiunta di un programma a un flusso del programma di coinvolgimento {#adding-a-program-to-an-engagement-program-stream}

## Perché utilizzare un programma nidificato in un flusso di programmi di coinvolgimento? {#why-use-a-nested-program-in-an-engagement-program-stream}

È facile aggiungere un&#39;e-mail a un flusso in un programma di coinvolgimento, e funziona bene. Tuttavia, se le tue esigenze aziendali sono più complesse, potrebbe essere utile inserire l&#39;e-mail all&#39;interno di un programma. Ad esempio:

* Invia un’e-mail a un sottogruppo di persone nel flusso
* Invia *diverso* e-mail a sottogruppi all’interno del flusso
* Includere pagine di destinazione, moduli o altre risorse nella pagina iniziale
* Abilitare l’attribuzione multi-touch
* Aggiungi passaggi di flusso aggiuntivi, ad esempio e-mail di avviso

## Cosa succede quando si utilizza un programma in un flusso? {#what-happens-when-you-use-a-program-in-a-stream}

Quando si utilizza un programma nidificato, la decisione di inviare un’e-mail a una persona si basa sull’appartenenza al programma e sull’ID del programma.

* Se non sei membro di un programma, riceverai tutte le e-mail che fanno parte del programma una volta
* Se sei membro del programma, non riceverai l’e-mail
* Se non sei più un membro ma hai ricevuto l&#39;e-mail in precedenza tramite quel programma, non riceverai l&#39;e-mail

Quando utilizzi un programma in un flusso, non importa se hai già ricevuto quell’e-mail specifica. Se l’e-mail non è stata inviata prima di *in detto programma specifico*, puoi riceverlo di nuovo.

Può ottenere e-mail e programmi complicati mescolando in un programma di coinvolgimento. Potrebbe essere utile utilizzare uno o l&#39;altro.

>[!TIP]
>
>Assicurati di utilizzare un **Membro del programma di coinvolgimento** nell’elenco smart.

## Cosa succede alle persone che non soddisfano i criteri dell’elenco avanzato? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

Nel caso in cui un utente venga escluso dall’elenco smart della campagna intelligente di un programma nidificato, non passa al contenuto successivo durante il cast corrente. Passeranno al successivo contenuto del flusso per *seguente* gettato.

## Cosa contiene un programma nidificato? {#what-does-a-nested-program-contain}

Un programma nidificato ben progettato contiene e-mail, report e campagne intelligenti. Ha senso tenerli insieme.

L&#39;e-mail che utilizzi può risiedere nel programma, in un programma diverso o anche in Design Studio. Il luogo in cui vive dipenderà da come vuoi usarlo.

Il reporting delle modifiche avviene con la posizione dell’e-mail. Quindi, ad esempio, se l’e-mail si trova in Design Studio, nel Rapporto sulle prestazioni dell’e-mail, tutte le metriche vengono visualizzate in una riga: i diversi cast vengono combinati. Tuttavia, nel rapporto sulle prestazioni del flusso di coinvolgimento, i diversi invii vengono visualizzati separatamente.

>[!CAUTION]
>
>Se desideri inviare nuovamente qualcosa, è più sicuro creare un nuovo programma e una campagna intelligente.

>[!MORELIKETHIS]
>
>* [Aggiungere contenuto a un flusso](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Informazioni sui programmi](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)

