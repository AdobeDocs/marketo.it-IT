---
unique-page-id: 15695874
description: Connect BrightTALK to Marketo - Marketo Docs - Documentazione prodotto
title: Connect BrightTALK to Marketo
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# Connect BrightTALK to Marketo {#connect-brighttalk-to-marketo}

Scopri come collegare il canale BrightTALK all’istanza di Marketo. A tal fine, devi essere un amministratore per entrambi.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Passaggi in BrightTALK {#steps-in-brighttalk}

1. Effettuate il login in [business.brighttalk.com/demandcentral](http://business.brighttalk.com/demandcentral/login) e fate clic su **Connect Now**.
1. In Connettore Marketo avanzato, fate clic su **Connect**.
1. Viene visualizzata la schermata delle credenziali, in cui si chiede: ID client, Segreto cliente, URL servizio identità e URL servizio rimanente. Per ottenere queste informazioni, accedi a Marketo.

## Passaggi in Marketo {#steps-in-marketo}

>[!NOTE]
>
>A questo punto sarà necessario impostare un ruolo utente e un utente API solo API per limitare le autorizzazioni che BrightTALK avrà nell&#39;istanza di Marketo. Poiché abbiamo già articoli per questi passaggi, vi collegheremo a loro.

1. Creare un ruolo [utente Solo](http://docs.marketo.com/x/iwMk)API.
1. [Create un utente](http://docs.marketo.com/x/jwMk)API utilizzando il ruolo API BrightTALK creato durante il Passaggio 4.
1. Torna all&#39;area Admin.

   ![](assets/one.png)

1. In Integrazione, fai clic su **LaunchPoint**.

   ![](assets/two.png)

1. Fate clic sul menu a **discesa Nuovo** e selezionate **Nuovo servizio**.

   ![](assets/three.png)

1. Immettete il nome visualizzato desiderato. Fare clic sul menu a discesa Servizio e selezionare **Personalizzato** ( **non** selezionare BrightTALK).

   ![](assets/four.png)

   >[!CAUTION]
   >
   >Ricordare di non selezionare BrightTALK nel menu a discesa. Si tratta di un campo che stiamo cercando di rimuovere, e la sua selezione potrebbe creare problemi significativi con la vostra integrazione Marketo/BrightTALK.

1. Inserire una descrizione della scelta. Fate clic sul menu a discesa Solo utente API e selezionate l&#39;utente API BrightTALK creato durante il passaggio 5. Fate clic su **Crea**.

   ![](assets/five.png)

1. Fate clic su **Visualizza dettagli** per il servizio personalizzato appena creato.

   ![](assets/six.png)

1. Copiate (e salvate) l&#39;ID **** client e il Segreto **** cliente. Fate clic su **Chiudi**.

   ![](assets/eight-1.png)

1. In Integrazione, selezionare Servizi **** Web.

   ![](assets/nine-1.png)

1. In Rest API, copia (e salva) l’ **endpoint** e l’ **identità**.

   ![](assets/ten.png)

## Passaggi in BrightTALK {#steps-in-brighttalk-1}

1. Tornare alla schermata di configurazione del connettore BrightTALK dal passaggio 3 e immettere le credenziali salvate dai passaggi 12 e 14.

   Dopo l&#39;autenticazione delle credenziali, hai collegato ufficialmente BrightTALK a Marketo. Il passaggio successivo consiste nel determinare [quali campi dati si desidera sincronizzare](http://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync).

