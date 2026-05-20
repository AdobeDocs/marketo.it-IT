---
unique-page-id: 10098134
description: Scopri i programmi nidificati nei flussi di coinvolgimento e quando utilizzarli. Aggiungi programmi per sottogruppi, passaggi multi-touch e di flusso aggiuntivo.
title: Aggiunta di un programma a un flusso di programma di coinvolgimento
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
feature: Engagement Programs
TQID: https://experienceleague.adobe.com/kI2v6drF78DnJhhEbgeVSi4TYbF5rExY2wgR0aAK-bI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 471
ht-degree: 4%

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
>Utilizza un filtro **[!UICONTROL Member of Engagement Program]** nell&#39;elenco avanzato.

## Cosa succederà alle persone che non soddisfano i criteri dell’elenco avanzato? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

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
>* [Aggiungere contenuti a un flusso](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Informazioni sui programmi](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
