---
description: Configurare l’integrazione ON24 con Marketo - Marketo Docs - Documentazione del prodotto
title: Configurare l'integrazione ON24 con Marketo
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
source-git-commit: 3e0823976e8b837fcb2fdbbf03f26da48cbd74b7
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 1%

---

# Configurare l&#39;integrazione ON24 con Marketo{#set-up-the-on24-integration-with-marketo}

Ecco come impostare l’integrazione degli eventi ON24.

## Creare un ruolo solo API {#create-an-api-only-role}

1. Dal mio Marketo, fai clic su **Amministratore**.

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. In Sicurezza, fai clic su **Utenti e ruoli**.

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. Fai clic sul pulsante **Ruoli** e quindi **Nuovo ruolo**.

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. Immetti un Nome ruolo. Apri **API di accesso** e selezionare &quot;Read-Write Custom Object&quot; e &quot;Read-Write Person&quot;. Fai clic su **Crea**.

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## Creare un nuovo utente {#create-a-new-user}

1. Sempre in Utenti e ruoli, fai clic sul pulsante **Utenti** e fai clic su **Invita nuovo utente**.

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. Immetti le informazioni del nuovo utente e fai clic su **Successivo**.

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. Seleziona il ruolo Solo API ON24 appena creato. Seleziona la **Solo API** casella di controllo. Fai clic su **Successivo**.

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. Fai clic su **Invia**.

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>Un invito non è richiesto per gli utenti solo API.

## Configurazione connessione ON24 {#set-up-on24-connection}

1. Sempre nella sezione Amministratore, fai clic su **LaunchPoint**.

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. Fai clic su **Nuovo** then **Nuovo servizio**.

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. Scegli un nome visualizzato. Fai clic sul pulsante **Servizio** a discesa e seleziona **Personalizzato**. Immetti una descrizione. Fai clic sull’elenco a discesa Solo utente API e seleziona l’utente creato [nei passaggi precedenti](#create-a-new-user). Fai clic su **Crea**.

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. Individua il servizio LaunchPoint personalizzato appena creato e fai clic su Visualizza dettagli.

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. Evidenzia, fai clic con il pulsante destro del mouse, copia e salva l’ID client (ne avrai bisogno in un secondo momento). Ripeti per segreto client.

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. Nella struttura a sinistra fare clic su Servizi Web.

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. In &quot;REST API&quot;, evidenzia, fai clic con il pulsante destro del mouse, copia e salva la prima parte dell’identità (fino a &quot;m&quot; in .com).

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. Con l’ID client, il segreto client e l’identità salvati, accedi al tuo account ON24. Gli altri passaggi vengono eseguiti e [delineato qui](https://on24support.force.com/Support/s/article/Connect-Marketo-ON24-Connect-Data-Integration#Step6){target=&quot;_blank&quot;}.
