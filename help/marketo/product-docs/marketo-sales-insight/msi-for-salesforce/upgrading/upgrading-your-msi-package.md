---
unique-page-id: 37357050
description: Aggiornamento del pacchetto MSI - Documentazione Marketo - Documentazione del prodotto
title: Aggiornamento del pacchetto MSI
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Aggiornamento del pacchetto MSI {#upgrading-your-msi-package}

1. Passa a [questa pagina nell&#39;appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target=&quot;_blank&quot;}.

1. Accedi alla tua istanza Salesforce (quella connessa alla tua istanza Marketo, può essere sandbox o produzione) dall&#39;angolo in alto a destra nella pagina dal passaggio 1. Devi disporre dei privilegi di amministratore per installare/aggiornare un pacchetto gestito in Salesforce.

1. Fai clic sul pulsante **Scarica subito** pulsante . Ti verrà chiesto di scegliere il percorso di installazione. Potrai effettuare l’aggiornamento poiché disponi già di una versione precedente di MSI. Scegli un&#39;opzione in base all&#39;account a cui hai effettuato l&#39;accesso durante il primo passaggio.

   >[!TIP]
   >
   >È consigliabile testarlo sull’istanza sandbox prima di aggiornare l’istanza di produzione.

1. Puoi aggiornare il pacchetto scegliendo &quot;Installa solo per amministratori&quot; (e fornire l’accesso MSI a profili specifici in un secondo momento), &quot;Installa per tutti gli utenti&quot; o, &quot;Installa per profili specifici&quot;. In questo esempio scegliamo Solo amministratori. Dopo aver effettuato la selezione, fai clic su **Aggiornamento**.

   ![](assets/four.png)

>[!NOTE]
>
>Si consiglia di aggiornare il pacchetto solo per gli amministratori e quindi [fornire accesso a utenti specifici](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;} in base al numero di sedi MSI acquistate. In alternativa, puoi creare un profilo Salesforce specifico per gli utenti MSI e installare o aggiornare il pacchetto solo per tali utenti.
