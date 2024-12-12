---
description: Promozione di un webinar interattivo - Documentazione di Marketo - Documentazione del prodotto
title: Promozione di un webinar interattivo
feature: Interactive Webinars
exl-id: d26f91ce-3a95-4247-9a52-085260bb15e8
source-git-commit: 6747a7b85047024d295ecc2c061bb6370ccfe0b9
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Promozione di un webinar interattivo {#promoting-an-interactive-webinar}

La promozione di un webinar interattivo è simile alla promozione di un webinar per partner tramite Launchpoint. Durante la creazione di un programma di eventi di webinar interattivo, è possibile aggiungere membri eseguendo una campagna o importando membri nel programma. Per verificare i membri aggiunti al programma eventi webinar interattivi, fare clic sulla scheda **Membri**.

![](assets/promoting-an-interactive-webinar-1.png)

Dopo l’aggiunta o l’importazione dei membri, puoi creare una campagna e-mail all’interno del programma di eventi del webinar interattivo per inviare un invito a tutti i membri del programma e cambiarne lo stato in &quot;invitato&quot; una volta che l’e-mail è stata consegnata.

>[!NOTE]
>
>Se desideri aggiungere un co-host o un presentatore come membro del pubblico al programma di eventi del webinar interattivo, devi utilizzare un ID e-mail diverso per loro, altrimenti riceveranno un errore &quot;Questa e-mail è già registrata&quot;.

L’e-mail può contenere dettagli specifici del programma e includere un URL della pagina di destinazione che reindirizzerebbe il destinatario a una pagina specifica in cui è possibile aggiungere ulteriori informazioni relative al webinar (ad esempio, contenuto, informazioni sul presentatore, ecc.). Questa pagina di destinazione può essere creata come risorsa locale nel programma di eventi dei webinar interattivi.

Per richiedere la registrazione a questo webinar, abilita un modulo nella pagina di destinazione e collega i clic del modulo alla registrazione abilitata nel programma di eventi del webinar interattivo. È quindi possibile creare una campagna che utilizza l’invio dei moduli come attivatore e cambia lo stato del programma da &quot;invitato&quot; a &quot;registrato&quot;.

>[!NOTE]
>
>La transizione da &quot;invitato&quot; a &quot;registrato&quot; non è automatica nei webinar interattivi, in quanto possono esserci più attivatori che creano la transizione.

Quando un membro si trova nello stato di programma &quot;registrato&quot; in un programma di eventi di webinar interattivi, viene automaticamente effettuata una registrazione al webinar creato in Adobe Connect. I dati di registrazione come Nome, Cognome e ID e-mail vengono quindi trasferiti ad Adobe Connect. Ciò significa che una volta che l’utente si unisce al webinar come partecipante, le informazioni saranno disponibili al presentatore o all’host durante il webinar.

Entro pochi minuti dalla registrazione, l’URL del webinar per il membro viene popolato nella scheda Membri. Se non riesci a individuare la colonna per l’URL del webinar, accertati che la colonna sia stata aggiunta alla vista. Questo è un URL personalizzato per ogni membro registrato per poter accedere al webinar all’ora pianificata senza richiedere alcuna autenticazione. I token scambiati internamente si occupano dell&#39;autenticazione per i membri.

È possibile utilizzare il `{{member.webinar url}}` [token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} per includere l&#39;URL del webinar ai singoli membri in una campagna e-mail per comunicare che sono stati registrati nell&#39;evento e per utilizzare l&#39;URL di partecipazione per accedere al webinar all&#39;ora pianificata. I token del calendario possono essere utilizzati nella stessa campagna e-mail per garantire che la pianificazione del webinar possa essere aggiunta ai calendari dei membri.

Sul lato destro della scheda Panoramica nel programma dell’evento sono disponibili collegamenti per creare una pagina di destinazione e una campagna e-mail. Le altre promozioni relative a un evento rimangono invariate rispetto ai webinar dei partner che utilizzano l’integrazione Launchpoint.

![](assets/promoting-an-interactive-webinar-2.png)

I webinar interattivi consentono di richiedere la registrazione prima, durante o dopo un webinar. In tutti i casi, dovrai semplicemente condividere l’URL del webinar con il lead. Facendo clic sul collegamento prima dell’inizio del webinar, vengono inviate a una pagina di destinazione precedente al webinar. Facendo clic su di esso durante il webinar, vengono indirizzati al webinar in corso. Facendo clic su di esso dopo il webinar, viene visualizzata una registrazione del webinar.

## Token webinar interattivi {#interactive-webinars-tokens}

Utilizza i token per promuovere i webinar interattivi nelle e-mail e nelle pagine di destinazione senza dover aggiungere manualmente i dettagli del webinar. Questo migliora l’efficienza complessiva, poiché qualsiasi modifica apportata ai metadati del webinar (come titolo del webinar, data di inizio e così via) si rifletterà automaticamente nelle risorse.

![](assets/promoting-an-interactive-webinar-3.png)

**Elenco dei token**

* program.webinarCapacity
* program.webinarDuration
* program.webinarEndDate
* program.webinarEndTime
* program.webinarGenericURL
* program.webinarLanguage
* program.webinarStartDate
* program.webinarStartTime
* program.webinarTimezone
* program.webinarTitle
