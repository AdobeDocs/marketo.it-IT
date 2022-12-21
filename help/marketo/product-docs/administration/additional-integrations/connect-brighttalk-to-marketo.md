---
unique-page-id: 15695874
description: Collegare BrightTALK a Marketo - Documentazione Marketo - Documentazione del prodotto
title: Collegare BrightTALK a Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# Collegare BrightTALK a Marketo {#connect-brighttalk-to-marketo}

Scopri come collegare il tuo canale BrightTALK alla tua istanza Marketo. Per farlo, devi essere un amministratore per entrambi.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Passaggi in BrightTALK {#steps-in-brighttalk}

1. Accedi a [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target=&quot;_blank&quot;} e fai clic su **Connetti ora**.
1. In Connettore Marketo avanzato, fai clic su **Connetti**.
1. Verrà visualizzata la schermata delle credenziali, chiedendo: ID client, segreto client, URL del servizio Identity e URL del servizio di ripristino. Per ottenere queste informazioni, accedi a Marketo.

## Passaggi in Marketo {#steps-in-marketo}

>[!NOTE]
>
>A questo punto ti verrà richiesto di impostare un ruolo utente solo API e un utente API per limitare quali autorizzazioni avranno BrightTALK nella tua istanza Marketo. Poiché abbiamo già articoli per questi passaggi, vi collegheremo a loro.

1. Crea un [Ruolo utente solo API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target=&quot;_blank&quot;}.

1. [Creare un utente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target=&quot;_blank&quot;}, utilizzando il ruolo API BrightTALK creato durante il passaggio 4.

1. Torna all’area Amministratore.

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. In Integrazione, fai clic su **LaunchPoint**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Fai clic sul pulsante **Nuovo** a discesa e seleziona **Nuovo servizio**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Immetti un Nome visualizzato a tua scelta. Fai clic sull’elenco a discesa Servizio e seleziona **Personalizzato** (do _not_ selezionare BrightTALK).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >Ricordare di non selezionare BrightTALK nel menu a discesa. Si tratta di un campo che stiamo tentando di rimuovere e la sua selezione potrebbe creare problemi significativi con l’integrazione Marketo/BrightTALK.

1. Inserisci una descrizione a tua scelta. Fai clic sull’elenco a discesa Solo utente API e seleziona l’utente API BrightTALK creato durante il passaggio 5. Fai clic su **Crea**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Fai clic su **Visualizza dettagli** per il servizio personalizzato appena creato.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Copia (e salva) il **ID client** e **Segreto client**. Fai clic su **Chiudi**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. In Integrazione, seleziona **Servizi Web**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. In Rest API, copia (e salva) il **Endpoint** e **Identità**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Ulteriori passi in BrightTALK {#additional-steps-in-brighttalk}

1. Torna alla schermata di configurazione del connettore BrightTALK dal passaggio 3 e immetti le credenziali salvate dai passaggi 12 e 14.

   Dopo l&#39;autenticazione delle credenziali, hai collegato ufficialmente BrightTALK a Marketo. Il passaggio successivo consiste nel determinare [quali campi dati sincronizzare](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target=&quot;_blank&quot;}.
