---
unique-page-id: 3571743
description: Scopri come configurare Marketo Sales Insight in Salesforce Professional Edition.
title: Configurare Marketo Sales Insight in Salesforce Professional Edition
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 1%

---

# Configura [!DNL Marketo Sales Insight] in [!DNL Salesforce] Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Configurare Marketo Sales Insight in Salesforce Professional Edition completando i passaggi seguenti.

>[!PREREQUISITES]
>
>* Installare Marketo nell&#39;edizione di [!DNL Salesforce] Professional.
>
>* [Installa [!DNL Marketo Sales Insight] Pacchetto in [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}

>[!NOTE]
>
>**Sono richieste le autorizzazioni di amministratore.**

## Configurare Sales Insight in Marketo Engage {#configure-sales-insight-in-marketo}

1. Per ottenere le credenziali Marketo Sales Insight dal tuo account Marketo, apri una nuova finestra del browser.

1. Passare all&#39;area **[!UICONTROL Admin]** e selezionare **[!UICONTROL Sales Insight]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Fai clic su **[!UICONTROL Edit API Configuration]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Immettere una chiave segreta API a scelta e fare clic su **[!UICONTROL Save]**. NON utilizzare una e commerciale (`&`) nella chiave segreta API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >La chiave segreta API è una password per la tua organizzazione e deve essere sicura.

1. Per compilare le credenziali, fare clic su **[!UICONTROL View]** nel pannello _[!UICONTROL Rest API Configuration]_.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Quando viene visualizzata una finestra di conferma, fare clic su **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Configura Sales Insight in [!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. Da Salesforce, fare clic su **[!UICONTROL Setup]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Cercare &quot;sito remoto&quot; e selezionare **[!UICONTROL Remote Site Settings]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Fai clic su **[!UICONTROL New Remote Site]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Immettere il nome del sito remoto (può essere simile a `MarketoSoapAPI`). Immetti l’URL del sito remoto, che è l’URL dell’host Marketo dal pannello Configurazione API Soap in Marketo Engage. Fare clic su **[!UICONTROL Save]**. Sono state create le impostazioni del sito remoto per l’API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Fare di nuovo clic su **[!UICONTROL New Remote Site]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Immetti il nome del sito remoto (può essere ad esempio &quot;MarketoRestAPI&quot;). Immetti l’URL del sito remoto, che è l’URL dell’API dal pannello Configurazione API REST in Marketo. Fare clic su **[!UICONTROL Save]**. Sono state create le impostazioni del sito remoto per l’API REST.

## Concedere agli utenti di Sales Insight l&#39;accesso al profilo per gli oggetti Salesforce standard {#grant-sales-insight-users-profile-access}

A causa dei miglioramenti apportati alla sicurezza di Salesforce, i pacchetti AppExchange non possono più concedere l’autorizzazione agli oggetti standard e l’accesso deve essere concesso agli oggetti Salesforce pertinenti dal profilo dell’utente Salesforce. Concedi le autorizzazioni necessarie seguendo questi passaggi.

1. Fai clic su **[!UICONTROL Setup]**.

1. Cerca &quot;Profili&quot; nella Ricerca rapida.

1. Fai clic su **[!UICONTROL Edit]** accanto al profilo utilizzato dagli utenti di Salesforce.

1. Nella sezione Autorizzazione oggetto standard, abilitare l&#39;accesso in lettura per i seguenti oggetti: lead, contatto, account e opportunità.

1. Fai clic su **[!UICONTROL Save]**.

## Personalizzare i layout di pagina {#customize-page-layouts}

1. Fai clic su **[!UICONTROL Setup]**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Cercare &quot;layout di pagina&quot; e selezionare **[!UICONTROL Page Layout]** in **[!UICONTROL Leads]**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. Fare clic su **[!UICONTROL Visualforce Pages]** a sinistra. Trascina **[!UICONTROL Section]** nel layout sotto la sezione Collegamenti personalizzati.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Immettere &quot;Marketo Sales Insight&quot; come **[!UICONTROL Section Name]**. Selezionare **[!UICONTROL 1-Column]** e fare clic su **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Trascina **[!UICONTROL Lead]** nella nuova sezione.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Il nome di questa casella cambia in base al tipo di oggetto. Se ad esempio si modifica il layout di pagina per i contatti, verrà visualizzato Contatto.

1. Fare doppio clic sul blocco **[!UICONTROL Lead]** appena aggiunto.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Modificare l&#39;altezza su 450 pixel e fare clic su **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Selezionare **[!UICONTROL Show scrollbars]** se è necessario accedere alle attività di scorrimento.

   >[!TIP]
   >
   >L&#39;altezza consigliata per gli oggetti Account e Opportunità è di 410 pixel.

1. Fare clic su **[!UICONTROL Fields]** a sinistra. Quindi cercare e trascinare l&#39;etichetta **[!UICONTROL Engagement]** nel layout **[!UICONTROL Marketo Sales Insight]**.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. Ripeti il passaggio precedente per i campi seguenti:

   * [!UICONTROL Engagement]
   * [!UICONTROL Relative Score Value]
   * [!UICONTROL Urgency Value]
   * [!UICONTROL Last Interesting Moment Date]
   * [!UICONTROL Last Interesting Moment Desc]
   * [!UICONTROL Last Interesting Moment Source]
   * [!UICONTROL Last Interesting Moment Type]

1. Al termine fai clic su **[!UICONTROL Save]** (Continua).

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Per aggiungere sezioni di pagina Visualforce per **[!UICONTROL Contact]**, **[!UICONTROL Account]** e **[!UICONTROL Opportunity]**, ripetere i passaggi 5-7.

1. Ripetere i passaggi da 8 a 10 per aggiungere campi Insight vendite per **[!UICONTROL Contact]**. Assicurati di salvare dopo eventuali modifiche.

## Mappa campi persona personalizzati {#map-custom-person-fields}

I campi persona di Marketo devono essere mappati sui campi contatto di Salesforce per garantire il corretto funzionamento della conversione. Segui questi passaggi per mapparli.

1. Fai clic su **[!UICONTROL Setup]**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Cercare &quot;fields&quot; nella barra di ricerca e fare clic su **[!UICONTROL Fields]** in **[!UICONTROL Leads]**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Fai clic su **[!UICONTROL Map Lead Fields]**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Fai clic sul menu a discesa a destra per **[!UICONTROL Engagement]**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Selezionare **[!UICONTROL Contact.Engagement]** nell&#39;elenco.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. Ripeti e mappa anche questi campi.

   | Campo personalizzato persona Marketo | Campo personalizzato contatto Salesforce |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

   {style="table-layout:auto"}

1. Al termine, fare clic su **[!UICONTROL Save]**.

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Scheda di configurazione di Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. Da Salesforce, fare clic su **+** alla fine della barra delle schede e fare clic su **[!UICONTROL Marketo Sales Insight Config]**.

1. Copiare le credenziali dal pannello API Soap nella [pagina di amministrazione di Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} e incollarle nella sezione API Soap della pagina Configurazione di Salesforce Sales Insight.

1. Copiare le credenziali dal pannello **[!UICONTROL Rest API]** nella [pagina di amministrazione di Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} e incollarle nella sezione Rest API della pagina di configurazione Salesforce Sales Insight.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

Dovresti essere in grado di visualizzare i campi Marketo Sales Insight per lead, contatti, account e opportunità.

>[!NOTE]
>
>Se il test di diagnostica non è riuscito, [aggiungere altri campi al layout di pagina](https://nation.marketo.com/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} potrebbe risolvere il problema.

>[!NOTE]
>
>Per gli account, Sales Insight include tutte le e-mail, ma solo i momenti di interesse più recenti, l’attività web e le modifiche dei punteggi.

>[!MORELIKETHIS]
>
>* [Priorità, Urgenza, Punteggio relativo e Elementi di maggiore rilevanza](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [Aggiungi scheda Marketo a [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [Aggiungere l&#39;accesso di Insight alle vendite ai profili](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
