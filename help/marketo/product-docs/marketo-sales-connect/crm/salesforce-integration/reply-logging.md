---
unique-page-id: 14352480
description: Registrazione delle risposte (SFDC) - Documentazione di Marketo - Documentazione del prodotto
title: Registrazione delle risposte (SFDC)
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Registrazione delle risposte (SFDC) {#reply-logging-sfdc}

Sales Connect offre la possibilità di registrare automaticamente le risposte dei potenziali clienti in Salesforce. La struttura che ti consente di farlo si basa sul tracciamento delle risposte e-mail. Se possiamo tenere traccia della risposta di un potenziale cliente, possiamo registrare tale risposta in Salesforce.

## Requisiti {#requirements}

* Deve registrare le e-mail tramite registrazione API
* Deve essere in grado di [tenere traccia di una risposta](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Deve essere connesso con [!DNL Salesforce]
* Deve avere [!DNL Salesforce] [chiamate API](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) disponibili

## Abilita registrazione risposte {#enable-reply-logging}

1. Per abilitare la registrazione delle risposte, passare alla pagina delle impostazioni di [!DNL Salesforce]. Una volta disattivata la registrazione API, verrà visualizzata l&#39;opzione per controllare _Registra risposte_.

   >[!NOTE]
   >
   >La registrazione delle risposte segue le stesse regole in vigore per le e-mail di registrazione inviate. Ciò include il modo in cui vengono registrate le e-mail; a lead e contatti; quando esiste un record duplicato; se non vengono trovati record corrispondenti.

## Impostazione del tipo di risposta in [!DNL Salesforce] {#setting-type-to-reply-in-salesforce}

Ottenere dati significativi dai report [!DNL Salesforce] è importante. La possibilità di compilare il campo Tipo come &quot;Risposta&quot; consente di ottenere tali dati tramite i rapporti. Collabora con `[!DNL Salesforce] admin` per completare la configurazione.

1. Vai a **[!UICONTROL Setup]** > **[!UICONTROL Customize]** > **[!UICONTROL Activities]** > **[!UICONTROL Task Fields]**.
1. Fai clic su **[!UICONTROL Type]**.
1. In Valori elenco a discesa Tipo di attività fare clic su **[!UICONTROL New]**.
1. Digita &quot;Reply&quot; (&quot;Risposta&quot;) nella casella vuota. Assicurarsi di immettere la lettera &#39;R&#39; maiuscola e fare clic su **[!UICONTROL Save]**.

   >[!NOTE]
   >
   >Non è necessario selezionare un valore predefinito nell&#39;elenco a discesa Tipo. [!DNL Sales Connect] vedrà che questo tipo di attività è disponibile nella tua istanza di [!DNL Salesforce] e compilerà di conseguenza il campo dell&#39;attività sulle attività in arrivo.
