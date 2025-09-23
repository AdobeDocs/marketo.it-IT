---
description: Registrazione delle risposte - Documentazione di Marketo - Documentazione del prodotto
title: Registrazione delle risposte
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 2%

---

# Registrazione delle risposte {#reply-logging}

Sales Insight Actions consente di registrare automaticamente le risposte dei potenziali clienti in [!DNL Salesforce]. La struttura che ti consente di farlo si basa sul tracciamento delle risposte e-mail. Se possiamo tenere traccia della risposta di un potenziale cliente, possiamo registrare tale risposta in [!DNL Salesforce].

## Requisiti {#requirements}

* Deve registrare le e-mail tramite registrazione API
* Deve essere in grado di [tenere traccia di una risposta](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
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
1. In [!UICONTROL Task Type Picklist Values], fare clic su **[!UICONTROL New]**.
1. Digita &quot;Reply&quot; (&quot;Risposta&quot;) nella casella vuota. Assicurarsi di immettere la lettera &#39;R&#39; maiuscola e fare clic su **[!UICONTROL Save]**.

   >[!NOTE]
   >
   >Non è necessario selezionare un valore predefinito nell&#39;elenco a discesa Tipo. [!DNL Sales Insight Actions] vedrà che questo tipo di attività è disponibile nella tua istanza di [!DNL Salesforce] e compilerà di conseguenza il campo dell&#39;attività sulle attività in arrivo.
