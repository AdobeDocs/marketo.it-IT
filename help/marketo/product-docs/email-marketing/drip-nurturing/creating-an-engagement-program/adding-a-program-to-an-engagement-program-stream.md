---
unique-page-id: 10098134
description: Aggiunta di un programma a un flusso del programma di coinvolgimento - Documenti Marketo - Documentazione del prodotto
title: Aggiunta di un programma a un flusso del programma di coinvolgimento
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Aggiunta di un programma a un flusso del programma di coinvolgimento {#adding-a-program-to-an-engagement-program-stream}

## Perché utilizzare un programma nidificato in un flusso di programmi di coinvolgimento? {#why-use-a-nested-program-in-an-engagement-program-stream}

È facile aggiungere un&#39;e-mail a un flusso in un programma di coinvolgimento, e funziona bene. Tuttavia, se le esigenze aziendali sono più complesse, potrebbe essere utile inserire l&#39;e-mail all&#39;interno di un programma. Ad esempio, potrebbe essere utile:

* Inviare un&#39;e-mail a un sottogruppo di persone nello streaming
* Inviare *e-mail diverse* ai sottogruppi all&#39;interno del flusso
* Includi pagine di destinazione, moduli o altre risorse nella pagina
* Abilita attribuzione multi-touch
* Aggiunta di passaggi di flusso aggiuntivi, ad esempio e-mail di avviso

## Cosa succede quando si utilizza un programma in un flusso? {#what-happens-when-you-use-a-program-in-a-stream}

Quando si utilizza un programma nidificato, la decisione di inviare un&#39;e-mail a una persona è basata sull&#39;appartenenza al programma e sull&#39;ID del programma.

* Se non sei membro di un programma, riceverai tutte le e-mail che fanno parte del programma una volta
* Se siete membri del programma, non riceverete l&#39;e-mail
* Se non siete più membri ma avete ricevuto l&#39;e-mail in precedenza tramite tale programma, non riceverete l&#39;e-mail

Quando utilizzi un programma in un flusso, non importa se hai già ricevuto quell&#39;e-mail specifica. Fintanto che l&#39;e-mail non è stata inviata prima di *in quel programma specifico*, è possibile riceverla nuovamente.

Può ottenere e-mail e programmi di mixaggio complicati in un programma di coinvolgimento. Potreste voler usare l&#39;uno o l&#39;altro.

>[!TIP]
>
>Assicurarsi di utilizzare un filtro **Membro del programma di coinvolgimento** nell&#39;elenco smart.

## Cosa succede alle persone che non soddisfano i criteri della lista intelligente? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

Nel caso in cui un utente venga escluso dall&#39;elenco smart della campagna smart di un programma nidificato, durante il cast corrente non passa al contenuto successivo. Passeranno al contenuto successivo nello streaming per il cast *successivo*.

## Cosa contiene un programma nidificato? {#what-does-a-nested-program-contain}

Un programma nidificato ben progettato contiene e-mail, report e campagne intelligenti. Ha senso tenerli insieme.

L&#39;e-mail che utilizzate può essere pubblicata nel programma, in un altro programma o anche in Design Studio. Il luogo in cui vive dipenderà da come vuoi usarlo.

Generazione dei rapporti sulle modifiche con la posizione dell’e-mail. Quindi, ad esempio, se l&#39;e-mail si trova in Design Studio, nel report Email Performance (Prestazioni e-mail), tutte le metriche sono visualizzate in una riga - le diverse cast sono combinate. Tuttavia, nel rapporto sulle prestazioni del flusso di coinvolgimento, le diverse invii vengono visualizzate separatamente.

>[!CAUTION]
>
>Se si desidera inviare nuovamente qualcosa, è più sicuro creare un nuovo programma e una campagna intelligente.

>[!MORELIKETHIS]
>
>* [Aggiunta di contenuto a un flusso](add-content-to-a-stream.md)
>* [Informazioni sui programmi](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)

>



