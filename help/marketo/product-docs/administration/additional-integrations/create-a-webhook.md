---
unique-page-id: 2360360
description: Creare un Webhook - Documenti Marketo - Documentazione prodotto
title: Creare un Webhook
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---


# Creare un Webhook {#create-a-webhook}

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

Utilizza i webhooks per sfruttare i servizi Web di terze parti per inviare messaggi di testo, espandere i dati delle persone e altro ancora.

>[!NOTE]
>
>**Disponibilità**
>
>Non tutti i clienti hanno acquistato questa funzionalità. Per informazioni, contattate il rappresentante commerciale.

1. Vai a **Admin **e fai clic su **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Fate clic su **Nuovo Webhook**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Denominate e configurate il webhook.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Ciò spesso include l&#39;immissione delle credenziali del servizio di terze parti come parametro URL o nel modello POST.

   * **URL**: Inserite l’URL che utilizzate per POST della richiesta al servizio Web. Per inserire un token, ad esempio l&#39;indirizzo e-mail della persona (**`{{lead.Email Address}}`**), nella richiesta fate clic su **Inserisci token**.

   * **Modello**: Se desiderate trasmettere le informazioni nel corpo del POST, inserite il modello. Utilizzate qualsiasi formato di dati che supporti POST HTTP, inclusi XML, JSON o SOAP. Per inserire un token nel modello, fate clic su **Inserisci token**.

   * **Richiedi codifica** token: Se i valori del token includono caratteri speciali (ad esempio una e commerciale, &#39;&amp;&#39;), indicate il formato della richiesta (**JSON** o **Form/Url**).

   * **Tipo** di risposta: Selezionate il formato della risposta ricevuta dal servizio (**JSON** o **XML**).

   Fate clic su Crea.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>**Tubo profondo**
>
>Scopri di più nella [tuffi](http://developers.marketo.com/documentation/webhooks/) di webhooks.

