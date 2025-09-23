---
unique-page-id: 10098238
description: Domande frequenti sulla compilazione dei moduli social di LinkedIn - Documentazione di Marketo - Documentazione del prodotto
title: Domande frequenti sulla compilazione di un modulo di contatto LinkedIn
hide: true
hidefromtoc: true
exl-id: ce87b918-5b45-418f-9b42-8e8275f2e60a
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 1%

---

# [!DNL LinkedIn] domande frequenti sulla compilazione dei moduli social network {#linkedin-social-form-fill-faqs}

Il criterio API rivisto di [!DNL LinkedIn] ci ha richiesto di rimuovere [!DNL LinkedIn] Social Form Fill dal nostro prodotto.

## Aspetti importanti da considerare {#important-things-to-know}

* [!DNL LinkedIn] i pulsanti per la compilazione dei moduli social non erano più un&#39;opzione da aggiungere a Marketo il 28 aprile 2016

* È stato rimosso il pulsante [!DNL LinkedIn] riempimento modulo social da tutti i moduli in cui era abilitato

## Perché questa funzionalità è stata rimossa dal mio abbonamento a Marketo? {#why-was-this-functionality-removed-from-my-marketo-subscription}

LinkedIn ha apportato alcune modifiche significative al proprio programma per sviluppatori. Come parte di queste modifiche, Marketo non è più in grado di supportare questa funzionalità per i clienti.

## Cos&#39;è successo se non ho rimosso i pulsanti di riempimento del modulo social [!DNL LinkedIn] dai moduli in cui era abilitato il modulo social? {#what-happened-if-i-didnt-remove-the-linkedin-social-form-fill-buttons-from-my-forms-that-had-social-form-enabled}

Il 28 aprile 2016 è stato rimosso il pulsante [!DNL LinkedIn] per la compilazione dei moduli social dai moduli in cui era ancora abilitato il modulo social.

## Ho inserito questa funzionalità nei moduli da quando siamo diventati clienti di Marketo. Come posso sapere quali moduli utilizzano [!DNL LinkedIn] per la compilazione dei moduli social? {#i-have-been-inserting-this-functionality-on-forms-since-we-became-a-marketo-customer-how-do-i-know-which-forms-were-using-linkedin-social-form-fill}

Prima di apportare questa modifica, abbiamo inviato notifiche settimanali alla tua casella in entrata delle notifiche con un elenco di moduli che utilizzavano [!DNL LinkedIn] Riempimento modulo social. Questi avvisi hanno lo scopo di aiutarti a identificare dove stavi utilizzando questa funzionalità.

## [!DNL LinkedIn] pulsanti di condivisione social continuano a funzionare? {#do-linkedin-social-sharing-buttons-still-work}

Sì.  La modifica influisce solo sulla funzionalità di riempimento del modulo social network di [!DNL LinkedIn].

## [!DNL Facebook] e [!DNL Twitter] compilazioni modulo social continuano a funzionare? {#do-facebook-and-twitter-social-form-fill-still-work}

Sì.  [!DNL Facebook] e [!DNL Twitter] riempimento modulo social non sono stati modificati.

## È successo qualcosa ai dati che abbiamo già acquisito tramite [!DNL LinkedIn] compilazione modulo social? {#did-anything-happen-to-the-data-we-already-captured-via-linkedin-social-form-fill}

No, questi dati sono già stati memorizzati nel record persona in Marketo e non sono stati interessati da questa modifica.

## Dove posso trovare ulteriori informazioni sui criteri API di LinkedIn? {#where-can-i-find-more-information-about-linkedin-s-api-policy}

Segui questo collegamento per ulteriori informazioni sulle modifiche [!DNL LinkedIn] apportate ai criteri API: [https://developer.linkedin.com/blog/posts/2015/developer-program-changes](https://developer.linkedin.com/blog/posts/2015/developer-program-changes)

## Come posso contattare [!DNL LinkedIn] con domande? {#how-can-i-contact-linkedin-with-questions}

Segui questo collegamento per contattare [!DNL LinkedIn] in merito alle loro soluzioni di marketing: [https://business.linkedin.com/marketing-solutions/contact-us](https://business.linkedin.com/marketing-solutions/contact-us)

## Se Marketo ha rimosso questa funzionalità dai miei moduli il 28 aprile, i miei moduli e le pagine di destinazione interessate sono stati messi in modalità bozza? {#if-marketo-removed-this-functionality-from-my-forms-on-april-were-my-forms-and-the-affected-landing-pages-put-into-draft-mode}

No, i moduli in cui è stata rimossa questa funzionalità sono rimasti pubblicati.

## Se [!DNL LinkedIn] fosse la mia unica rete selezionata, cambierà l&#39;aspetto del mio modulo? {#if-linkedin-was-my-only-selected-network-will-this-change-the-appearance-of-my-form}

No, verrà rimosso solo il pulsante [!DNL LinkedIn] dal modulo. Ogni volta che a un modulo viene applicato il riempimento di un modulo social, viene creato un contenitore al di sopra del quale sono presenti i pulsanti Riempimento modulo social. Prima del 28 aprile 2016, se [!DNL LinkedIn] era l&#39;unica opzione, l&#39;aspetto del contenitore era simile a questa immagine:

![—](assets/one.png)

Dopo il 28 aprile 2016, è rimasto un contenitore vuoto nella parte superiore di qualsiasi modulo in cui [!DNL LinkedIn] Social Form Fill è stato rimosso:

![—](assets/two.png)

>[!NOTE]
>
>Le immagini di cui sopra sono solo per esempio. Potrebbe non essere esattamente così che viene visualizzato il contenitore del pulsante Riempimento modulo social network. Qualsiasi colore, stile, ecc. del font. hai scelto di influenzare l’aspetto del contenitore.

## Se [!DNL LinkedIn] era la mia unica rete selezionata, come posso rimuovere il contenitore vuoto sopra il mio modulo? {#if-linkedin-was-my-only-selected-network-how-can-i-remove-the-empty-container-above-my-form}

È possibile rimuovere il contenitore vuoto modificando il modulo, selezionando [!DNL Facebook] o [!DNL Twitter] come opzione per Riempimento modulo social, quindi deselezionando [!DNL Facebook] o [!DNL Twitter] come opzione per Riempimento modulo social. In questo modo verranno reimpostate le opzioni social all’interno del contenitore di riempimento del modulo e questo verrà rimosso dal modulo.
