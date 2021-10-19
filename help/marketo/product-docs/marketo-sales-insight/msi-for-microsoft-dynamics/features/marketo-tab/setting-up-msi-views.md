---
description: Configurazione delle visualizzazioni MSI - Marketo Docs - Documentazione del prodotto
title: Impostazione delle visualizzazioni MSI
hide: true
hidefromtoc: true
source-git-commit: f4930d1747f1ca893d7494afc3dcbeb8c6398e93
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Impostazione delle visualizzazioni MSI {#setting-up-msi-views}

Quando si installa il plug-in Sales Insight in Dynamics, nella mappa del sito vengono aggiunti automaticamente i Best Bet e le relative dashboard. Se per qualche motivo le dashboard non vengono aggiunte, ecco come aggiungerle manualmente.

1. In Dynamics, fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni avanzate** dal menu a discesa.

1. In alto a sinistra dello schermo, fai clic su **Impostazioni**. In Personalizzazione scegliere Personalizzazioni.

1. Fai clic su **Personalizzare il sistema**.

1. Nell&#39;albero a sinistra, fai clic su **Estensioni client** e fai doppio clic **Mappa del sito**.

1. Fare clic sulla freccia destra per passare alla pagina successiva. In Vendite, dovresti vedere Marketo. In caso contrario, assicurati di aver importato correttamente il pacchetto.

   >[!NOTE]
   >
   >In Marketo dovresti avere: Best ets, My Email, Web Activity e Anonymous Web Activity. Se manca uno di questi dashboard, fai clic sul segno + sopra Vendite e aggiungili come sottoarea.

1. Fai clic su un dashboard per selezionarlo. Nella colonna a destra, inserisci le rispettive informazioni riportate di seguito. È possibile ignorare tutte le categorie non elencate.

   **Migliori offerte**</br>
URL: MainviewBestbets.html</br>
Icona: /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID: marketo_bestbets</br>
Titolo: Migliori offerte

   **E-mail personale**</br>
URL: mkt_/MainViewMyEmail.html</br>
Icona: /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID: marketo_myemail</br>
Titolo: E-mail personale

   **Attività web**</br>
URL: mkt_/MainViewWebActivity.html</br>
Icona: /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID: marketo_webactivity</br>
Titolo: Attività web

   **Attività Web anonime**</br>
URL: mkt_/MainViewWebActivity.html</br>
Icona: /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID: marketo_anonymous_webactivity</br>
Titolo: Attività Web anonime

1. Fai clic su **Salva** al termine.
