---
description: Configurare l'integrazione ON24 con Marketo - Documentazione Marketo - Documentazione del prodotto
title: Configurare l'integrazione ON24 con Marketo
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Configurare l&#39;integrazione ON24 con Marketo{#set-up-the-on24-integration-with-marketo}

Ecco come configurare l’integrazione dell’evento ON24.

## Creare un ruolo solo API {#create-an-api-only-role}

1. Da Il mio Marketo, fai clic su **Amministratore**.

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. In Protezione fare clic su **Utenti e ruoli**.

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. Fare clic sulla scheda **Ruoli** e quindi su **Nuovo ruolo**.

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. Immettere un nome per il ruolo. Aprire il menu **Access API** e selezionare &quot;Read-Write Custom Object&quot; e &quot;Read-Write Person&quot;. Fai clic su **Crea**.

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## Crea un nuovo utente {#create-a-new-user}

1. Sempre in Utenti e ruoli, fai clic sulla scheda **Utenti** e poi su **Invita nuovo utente**.

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. Immettere le informazioni sul nuovo utente e fare clic su **Avanti**.

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. Seleziona solo il ruolo API ON24 appena creato. Selezionare la casella di controllo **Solo API**. Fai clic su **Avanti**.

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. Fai clic su **Invia**.

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>Non è necessario un invito per gli utenti solo API.

## Configura connessione ON24 {#set-up-on24-connection}

1. Sempre nella sezione Amministratore, fai clic su **LaunchPoint**.

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. Fai clic su **Nuovo** e quindi su **Nuovo servizio**.

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. Scegli un nome da visualizzare. Fai clic sul menu a discesa **Servizio** e seleziona **Personalizzato**. Immetti una descrizione. Fai clic sul menu a discesa Solo utente API e seleziona l&#39;utente che hai creato [ nei passaggi precedenti](#create-a-new-user). Fai clic su **Crea**.

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. Individuare il servizio LaunchPoint personalizzato appena creato e fare clic su Visualizza dettagli.

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. Evidenzia, fai clic con il pulsante destro del mouse, copia e salva l’ID client (sarà necessario in seguito). Ripeti per Segreto client.

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. Nell&#39;albero a sinistra fare clic su Servizi Web.

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. In &quot;REST API&quot;, evidenzia, fai clic con il pulsante destro del mouse, copia e salva la prima parte dell’identità (fino alla &quot;m&quot; in .com).

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. Con l&#39;ID client, il segreto client e l&#39;identità salvati, accedi all&#39;account ON24. I passaggi rimanenti vengono eseguiti qui e sono [descritti qui](https://on24support.force.com/Support/s/article/Connect-Marketo-ON24-Connect-Data-Integration#Step6){target="_blank"}.
