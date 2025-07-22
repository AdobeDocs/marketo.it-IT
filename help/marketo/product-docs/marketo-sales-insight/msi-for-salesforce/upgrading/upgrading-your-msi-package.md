---
unique-page-id: 37357050
description: Aggiornamento del pacchetto MSI - Documentazione di Marketo - Documentazione del prodotto
title: Aggiornamento del pacchetto MSI
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Aggiornamento del pacchetto MSI {#upgrading-your-msi-package}

>[!IMPORTANT]
>
>A causa dei miglioramenti apportati alla sicurezza da Salesforce, il pacchetto Sales Insight non può più concedere l&#39;autorizzazione agli oggetti standard. In futuro, il profilo Salesforce degli utenti di Sales Insight dovrà avere accesso in lettura ai seguenti oggetti standard: lead, contatto, account e opportunità. [Scopri come configurarlo qui](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#grant-sales-insight-users-profile-access){target="_blank"}.

1. Passare a [questa pagina in appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target="_blank"}.

1. Accedi all&#39;istanza [!DNL Salesforce] (quella connessa alla tua istanza Marketo, che può essere sandbox o produzione) dall&#39;angolo in alto a destra della pagina dal passaggio 1. Per installare/aggiornare un pacchetto gestito in [!DNL Salesforce] è necessario disporre dei privilegi di amministratore.

1. Fare clic sul pulsante **Scarica ora**. Ti verrà chiesto di scegliere dove desideri installare. Potrai effettuare l&#39;aggiornamento poiché disponi già di una versione precedente di MSI. Scegli un’opzione in base all’account a cui hai effettuato l’accesso durante il passaggio 1.

   >[!TIP]
   >
   >È consigliabile eseguire un test nell’istanza sandbox prima di aggiornare l’istanza di produzione.

1. Per aggiornare il pacchetto, scegli &quot;Installa solo per amministratori&quot; (e fornisci l’accesso MSI a profili specifici in un secondo momento), &quot;Installa per tutti gli utenti&quot; o &quot;Installa per profili specifici&quot;. In questo esempio stiamo scegliendo Solo amministratori. Dopo aver effettuato la selezione, fai clic su **Aggiorna**.

   ![](assets/four.png)

>[!NOTE]
>
>È consigliabile aggiornare il pacchetto solo per gli amministratori e quindi [fornire l&#39;accesso a utenti specifici](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"} in base al numero di postazioni MSI acquistate. In alternativa, puoi creare un profilo Salesforce specifico per gli utenti MSI e installare o aggiornare il pacchetto solo per tali utenti.
