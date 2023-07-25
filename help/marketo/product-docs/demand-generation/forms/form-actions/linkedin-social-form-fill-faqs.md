---
unique-page-id: 10098238
description: Domande frequenti sulla compilazione dei moduli social network per linkedIn - Documentazione di Marketo - Documentazione del prodotto
title: Domande frequenti sulla compilazione dei moduli social network per linkedIn
exl-id: ce87b918-5b45-418f-9b42-8e8275f2e60a
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Domande frequenti sulla compilazione dei moduli social network per linkedIn {#linkedin-social-form-fill-faqs}

La politica API rivista di linkedIn ci ha richiesto di rimuovere LinkedIn Social Form Fill dal nostro prodotto.

## Aspetti importanti da considerare {#important-things-to-know}

* I pulsanti Riempimento modulo social network di linkedIn non erano più disponibili per l’aggiunta a Marketo del 28 aprile 2016

* È stato rimosso il pulsante LinkedIn Social Form Fill da tutti i moduli in cui era abilitato

## Perché questa funzionalità è stata rimossa dal mio abbonamento a Marketo? {#why-was-this-functionality-removed-from-my-marketo-subscription}

LinkedIn ha apportato alcune modifiche significative al suo programma per sviluppatori. Come parte di queste modifiche, Marketo non è più in grado di supportare questa funzionalità per i clienti.

## Cos’è successo se non ho rimosso i pulsanti Riempimento LinkedIn Social Form dai moduli in cui era abilitato Social Form? {#what-happened-if-i-didnt-remove-the-linkedin-social-form-fill-buttons-from-my-forms-that-had-social-form-enabled}

Il 28 aprile 2016 è stato rimosso il pulsante LinkedIn Social Form Fill dai moduli in cui era ancora abilitato Social Form.

## Ho inserito questa funzionalità nei moduli da quando siamo diventati clienti di Marketo. Come posso sapere quali moduli utilizzavano LinkedIn Social Form Fill? {#i-have-been-inserting-this-functionality-on-forms-since-we-became-a-marketo-customer-how-do-i-know-which-forms-were-using-linkedin-social-form-fill}

Prima di apportare questa modifica, abbiamo inviato notifiche settimanali alla casella in entrata delle notifiche con un elenco di moduli che utilizzavano LinkedIn Social Form Fill (Compilazione modulo social network). Questi avvisi hanno lo scopo di aiutarti a identificare dove stavi utilizzando questa funzionalità.

## I pulsanti di condivisione social di LinkedIn funzionano ancora? {#do-linkedin-social-sharing-buttons-still-work}

Sì. La modifica interessa solo la funzionalità di riempimento dei moduli social network di LinkedIn.

## Facebook e Twitter Social Form Fill funzionano ancora? {#do-facebook-and-twitter-social-form-fill-still-work}

Sì. La modalità di compilazione dei moduli social network per facebook e Twitter non è stata modificata.

## È successo qualcosa ai dati che abbiamo già acquisito tramite LinkedIn Social Form Fill? {#did-anything-happen-to-the-data-we-already-captured-via-linkedin-social-form-fill}

No, questi dati sono già stati memorizzati nel record persona in Marketo e non sono stati interessati da questa modifica.

## Dove posso trovare ulteriori informazioni sui criteri API di LinkedIn? {#where-can-i-find-more-information-about-linkedin-s-api-policy}

Segui questo collegamento per ulteriori informazioni sulle modifiche apportate da LinkedIn ai propri criteri API: [https://developer.linkedin.com/blog/posts/2015/developer-program-changes](https://developer.linkedin.com/blog/posts/2015/developer-program-changes)

## Come posso contattare LinkedIn per eventuali domande? {#how-can-i-contact-linkedin-with-questions}

Segui questo link per contattare LinkedIn in merito alle sue soluzioni di marketing: [https://business.linkedin.com/marketing-solutions/contact-us](https://business.linkedin.com/marketing-solutions/contact-us)

## Se Marketo ha rimosso questa funzionalità dai miei moduli il 28 aprile, i miei moduli e le pagine di destinazione interessate sono stati messi in modalità bozza? {#if-marketo-removed-this-functionality-from-my-forms-on-april-were-my-forms-and-the-affected-landing-pages-put-into-draft-mode}

No, i moduli in cui è stata rimossa questa funzionalità sono rimasti pubblicati.

## Se LinkedIn è l&#39;unica rete selezionata, l&#39;aspetto del modulo verrà modificato? {#if-linkedin-was-my-only-selected-network-will-this-change-the-appearance-of-my-form}

No, rimuoveremo solo il pulsante LinkedIn dal modulo. Ogni volta che a un modulo viene applicato il riempimento di un modulo social, viene creato un contenitore al di sopra del quale sono presenti i pulsanti Riempimento modulo social. Prima del 28 aprile 2016, se LinkedIn era l’unica opzione, l’aspetto del contenitore somigliava a questa immagine:

![--](assets/one.png)

Dopo il 28 aprile 2016, è rimasto un contenitore vuoto nella parte superiore di qualsiasi modulo da cui è stato rimosso il riempimento del modulo social di LinkedIn:

![--](assets/two.png)

>[!NOTE]
>
>Le immagini di cui sopra sono solo per esempio. Potrebbe non essere esattamente così che viene visualizzato il contenitore del pulsante Riempimento modulo social network. Qualsiasi colore, stile, ecc. del font. hai scelto di influenzare l’aspetto del contenitore.

## Se LinkedIn è stata la mia unica rete selezionata, come posso rimuovere il contenitore vuoto sopra il modulo? {#if-linkedin-was-my-only-selected-network-how-can-i-remove-the-empty-container-above-my-form}

Per rimuovere il contenitore vuoto, modifica il modulo, seleziona Facebook o Twitter come opzione per Riempimento modulo social, quindi deseleziona Facebook o Twitter come opzione per Riempimento modulo social. In questo modo verranno reimpostate le opzioni social all’interno del contenitore di riempimento del modulo e questo verrà rimosso dal modulo.
