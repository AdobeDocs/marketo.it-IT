---
title: using-a-program-in-an-Engagement-program-stream
description: Utilizzo di un programma in un flusso del programma di coinvolgimento
translation-type: tm+mt
source-git-commit: 73df78512226c6c57625a73f14ba8b00bea195bd
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---


# Utilizzo di un programma in un flusso del programma di coinvolgimento

## Perché utilizzare un programma nidificato in un flusso di programmi di coinvolgimento?

È facile aggiungere un&#39;e-mail a un flusso in un programma di coinvolgimento, e funziona bene. Tuttavia, se le esigenze aziendali sono più complesse, potrebbe essere utile inserire l&#39;e-mail all&#39;interno di un programma. Ad esempio, potrebbe essere utile:

* Inviare un&#39;e-mail a un sottogruppo di persone nello streaming
* Inviare e-mail _diverse_ ai sottogruppi all&#39;interno del flusso
* Includere pagine di destinazione, moduli o altre risorse nel programma di partecipazione
* Abilita attribuzione multi-touch
* Aggiunta di passaggi di flusso aggiuntivi, come e-mail di avviso

## Cosa succede quando si utilizza un programma in un flusso?

Quando si utilizza un programma nidificato, la decisione di inviare un&#39;e-mail a una persona è basata sull&#39;appartenenza al programma e sull&#39;ID del programma.

* Se non si è membri del programma, riceveranno una sola volta tutte le e-mail che fanno parte del programma
* Se siete membri del programma, non riceverete l&#39;e-mail
* Se non siete più membri ma avete già ricevuto l&#39;e-mail in precedenza tramite tale programma, non riceverete l&#39;e-mail

Quando utilizzi un programma in un flusso, non importa se hai già ricevuto quell&#39;e-mail specifica. Fintanto che l&#39;e-mail non è stata inviata prima _in quel programma_ specifico, potete riceverla nuovamente.

Può ottenere e-mail e programmi di mixaggio complicati in un programma di coinvolgimento. Potreste voler usare l&#39;uno o l&#39;altro.

>[!TIP]
>
>Accertatevi di utilizzare il filtro Partecipante al programma nell&#39;elenco smart.

## Cosa succede alle persone che non soddisfano i criteri della lista intelligente?

Nel caso in cui un utente venga escluso dall&#39;elenco smart della campagna smart di un programma nidificato, durante il cast corrente non passa al contenuto successivo. Passeranno alla parte successiva del contenuto nello streaming per il cast _seguente_ .

## Cosa contiene un programma nidificato?

Un programma nidificato ben progettato contiene e-mail, report e campagne intelligenti. Ha senso tenerli insieme.

L&#39;e-mail che utilizzate può essere pubblicata nel programma, in un altro programma o anche in Design Studio. Il luogo in cui vive dipende da come vuoi usarlo.

Generazione dei rapporti sulle modifiche con la posizione dell’e-mail. Quindi, ad esempio, se l&#39;e-mail si trova in Design Studio, nel report Email Performance (Prestazioni e-mail), tutte le metriche sono visualizzate in una riga - le diverse cast sono combinate. Tuttavia, nel rapporto sulle prestazioni del flusso di coinvolgimento, le diverse invii vengono visualizzate separatamente.

>[!CAUTION]
>
>Se si desidera inviare nuovamente qualcosa, è più sicuro creare un nuovo programma e una campagna intelligente.
