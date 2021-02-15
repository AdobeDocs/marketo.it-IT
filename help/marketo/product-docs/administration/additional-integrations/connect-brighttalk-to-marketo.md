---
unique-page-id: 15695874
description: Connect BrightTALK to Marketo - Marketo Docs - Documentazione prodotto
title: Connect BrightTALK to Marketo
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# Connect BrightTALK to Marketo {#connect-brighttalk-to-marketo}

Scopri come collegare il canale BrightTALK all’istanza di Marketo. A tal fine, devi essere un amministratore per entrambi.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Passaggi in BrightTALK {#steps-in-brighttalk}

1. Accedete a [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login) e fate clic su **Connetti ora**.
1. In Connettore Marketo avanzato, fare clic su **Connetti**.
1. Viene visualizzata la schermata delle credenziali, in cui si chiede: ID client, Segreto cliente, URL servizio identità e URL servizio rimanente. Per ottenere queste informazioni, accedi a Marketo.

## Passaggi in Marketo {#steps-in-marketo}

>[!NOTE]
>
>A questo punto sarà necessario impostare un ruolo utente e un utente API solo API per limitare le autorizzazioni che BrightTALK avrà nell&#39;istanza di Marketo. Poiché abbiamo già articoli per questi passaggi, vi collegheremo a loro.

1. Create un [ruolo utente solo API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md).
1. [Create un utente](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) API utilizzando il ruolo API BrightTALK creato durante il Passaggio 4.
1. Torna all&#39;area Admin.

   ![](assets/one.png)

1. In Integrazione, fare clic su **LaunchPoint**.

   ![](assets/two.png)

1. Fare clic sul menu a discesa **Nuovo** e selezionare **Nuovo servizio**.

   ![](assets/three.png)

1. Immettete il nome visualizzato desiderato. Fare clic sul menu a discesa Servizio e selezionare **Personalizzato** (fare _not_ select BrightTALK).

   ![](assets/four.png)

   >[!CAUTION]
   >
   >Ricordare di non selezionare BrightTALK nel menu a discesa. Si tratta di un campo che stiamo cercando di rimuovere, e la sua selezione potrebbe creare problemi significativi con la vostra integrazione Marketo/BrightTALK.

1. Inserire una descrizione della scelta. Fate clic sul menu a discesa Solo utente API e selezionate l&#39;utente API BrightTALK creato durante il passaggio 5. Fare clic su **Crea**.

   ![](assets/five.png)

1. Fare clic su **Visualizza dettagli** per il servizio personalizzato appena creato.

   ![](assets/six.png)

1. Copiare (e salvare) l&#39; **ID client** e il **Segreto cliente**. Fare clic su **Chiudi**.

   ![](assets/eight-1.png)

1. In Integrazione, selezionare **Servizi Web**.

   ![](assets/nine-1.png)

1. In Rest API, copiare (e salvare) l&#39; **Endpoint** e **Identity**.

   ![](assets/ten.png)

## Passaggi aggiuntivi in BrightTALK {#additional-steps-in-brighttalk}

1. Tornare alla schermata di configurazione del connettore BrightTALK dal passaggio 3 e immettere le credenziali salvate dai passaggi 12 e 14.

   Dopo l&#39;autenticazione delle credenziali, hai collegato ufficialmente BrightTALK a Marketo. Il passaggio successivo consiste nel determinare [quali campi dati si desidera sincronizzare](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync).
