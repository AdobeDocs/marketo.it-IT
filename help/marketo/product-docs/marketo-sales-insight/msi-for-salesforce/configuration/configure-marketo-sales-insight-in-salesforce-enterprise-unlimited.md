---
unique-page-id: 2360368
description: Scopri come configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited Edition.
title: Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 1%

---

# Configura [!DNL Marketo Sales Insight] in [!DNL Salesforce] Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Configurare Marketo Sales Insight nelle edizioni Enterprise/Unlimited di Salesforce completando i passaggi seguenti.

>[!PREREQUISITES]
>
>[Installa [!DNL Marketo Sales Insight] Pacchetto in [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Sono richieste le autorizzazioni di amministratore.**

## Configurare Sales Insight in Marketo Engage {#configure-sales-insight-in-marketo}

1. Per ottenere le credenziali Marketo Sales Insight in Marketo Engage, vai all&#39;area **[!UICONTROL Admin]** e seleziona **[!UICONTROL Sales Insight]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Fai clic su **[!UICONTROL Edit API Configuration]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Immettere una chiave segreta API a scelta e fare clic su **[!UICONTROL Save]**. NON utilizzare una e commerciale (`&`) nella chiave segreta API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >La chiave segreta API è una password per la tua organizzazione e deve essere sicura.

1. Per compilare le credenziali, fare clic su **[!UICONTROL View]** nel pannello _[!UICONTROL Rest API Configuration]_.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Quando viene visualizzata una finestra di conferma, fare clic su **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Tieni aperta questa finestra. Queste informazioni sono necessarie in seguito per la configurazione di Salesforce.

## Configura [!DNL Sales Insight] in [!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. In Salesforce, fare clic su **[!UICONTROL Setup]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Cercare &quot;sito remoto&quot; e selezionare **[!UICONTROL Remote Site Settings]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Fai clic su **[!UICONTROL New Remote Site]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Immettere il nome del sito remoto (può essere simile a `MarketoSoapAPI`). Immettere l&#39;URL del sito remoto, ovvero l&#39;URL dell&#39;host Marketo dal pannello _[!UICONTROL Soap API Configuration]_in Marketo Engage. Fare clic su **[!UICONTROL Save]**. Sono state create le impostazioni del sito remoto per l’API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Fare di nuovo clic su **[!UICONTROL New Remote Site]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Immettere il nome del sito remoto (può essere simile a `MarketoAPI`). Immettere l&#39;URL del sito remoto, che corrisponde all&#39;URL API del pannello _[!UICONTROL Rest API Configuration]_in Marketo Engage. Fare clic su **[!UICONTROL Save]**. Sono state create le impostazioni del sito remoto per l’API REST.

   >[!NOTE]
   >
   >_Scegli_ (**[!UICONTROL Remote Site Name]** è utilizzato qui)`MarketoAPI`. **[!UICONTROL Remote Site URL]** si trova nel campo Host Marketo della finestra di dialogo Modifica configurazione API dal passaggio 3 nella sezione &quot;Configura Insight vendite in Marketo&quot;.

## Concedere agli utenti di Sales Insight l&#39;accesso al profilo per gli oggetti Salesforce standard {#grant-sales-insight-users-profile-access}

A causa dei miglioramenti apportati alla sicurezza di Salesforce, i pacchetti AppExchange non possono più concedere l’autorizzazione agli oggetti standard e l’accesso deve essere concesso agli oggetti Salesforce pertinenti dal profilo dell’utente Salesforce. Per concedere le autorizzazioni necessarie, segui la procedura riportata di seguito.

1. Fai clic su **[!UICONTROL Setup]**.

1. Cerca &quot;Profili&quot; nella Ricerca rapida.

1. Fai clic su **[!UICONTROL Edit]** accanto al profilo utilizzato dagli utenti di Salesforce.

1. Nella sezione _[!UICONTROL Standard Object Permission]_, abilitare l&#39;accesso **[!UICONTROL Read]**per i seguenti oggetti: [!UICONTROL Lead], [!UICONTROL Contact], [!UICONTROL Account] e [!UICONTROL Opportunity].

1. Fai clic su **[!UICONTROL Save]**.

## Personalizzare i layout di pagina {#customize-page-layouts}

1. Fai clic su **[!UICONTROL Setup]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Cercare &quot;layout di pagina&quot; e selezionare **[!UICONTROL Page Layout]** in **[!UICONTROL Leads]**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Fare clic su **[!UICONTROL Visualforce Pages]** a sinistra. Trascina **[!UICONTROL Section]** nel layout sotto la sezione _[!UICONTROL Custom Links]_.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Immettere &quot;Marketo Sales Insight&quot; come **[!UICONTROL Section Name]**, selezionare **[!UICONTROL 1-Column]** e fare clic su **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Trascina **[!UICONTROL Lead]** nella nuova sezione.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Il nome di questa casella cambia in base al tipo di oggetto. Se ad esempio si modifica il layout di pagina per i contatti, verrà visualizzato Contatto.

1. Fare doppio clic sul blocco **[!UICONTROL Lead]** appena aggiunto.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Modifica l&#39;altezza in **450** pixel e fai clic su **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Selezionare **[!UICONTROL Show scrollbars]** se è necessario accedere alle attività di scorrimento.

   >[!TIP]
   >
   >L&#39;altezza consigliata per gli oggetti Account e Opportunità è di 410 pixel.

1. Fare clic su **[!UICONTROL Fields]** a sinistra. Quindi cercare e trascinare l&#39;etichetta **[!UICONTROL Urgency]** nel layout **[!UICONTROL Marketo Sales Insight]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. Ripeti il passaggio precedente anche per questi campi.

   * Ultimo momento di interesse
   * Data ultimo momento di interesse
   * Descrizione ultimo momento di interesse
   * Ultimo momento di interesse Source
   * Tipo ultimo momento di interesse
   * Ultima attività per vendite
   * Ultimo coinvolgimento per vendite
   * ID contatto MSI
   * Punteggio relativo
   * Valore punteggio relativo
   * Urgenza
   * Valore Urgenza
   * Visualizza in Marketo

1. Al termine fai clic su **[!UICONTROL Save]** (Continua).

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Ripetere i passaggi 5-7 per aggiungere sezioni di pagina e campi Sales Insight di Visualforce per **[!UICONTROL Contact]**, **[!UICONTROL Account]** e **[!UICONTROL Opportunity]**.

1. Ripetere i passaggi 8-10 per aggiungere questi campi Sales Insight per **[!UICONTROL Contact]**. Assicurati di salvare tutte le modifiche.

   * Ultimo momento di interesse
   * Data ultimo momento di interesse
   * [!UICONTROL Last Interesting Moment Desc]
   * [!UICONTROL Last Interesting Moment Source]
   * [!UICONTROL Last Interesting Moment Type]
   * [!UICONTROL Last Marketo Activity by Sales]
   * [!UICONTROL Last Marketo Engagement by Sales]
   * [!UICONTROL MKTO Lead Score]
   * [!UICONTROL Relative Score]
   * [!UICONTROL Relative Score Value]
   * [!UICONTROL Sales Insight] - Apre la pagina dell&#39;elenco completo contatti
   * [!UICONTROL Urgency]
   * [!UICONTROL Urgency Value]

## Mappa campi persona personalizzati {#map-custom-person-fields}

I campi persona di Marketo devono essere mappati sui campi contatto di Salesforce per garantire il corretto funzionamento della conversione. Segui questi passaggi per mapparli.

1. Fai clic su **[!UICONTROL Setup]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Cercare &quot;fields&quot; nella barra di ricerca e fare clic su **[!UICONTROL Fields]** in **[!UICONTROL Leads]**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Fai clic su **[!UICONTROL Map Lead Fields]**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Fai clic sul menu a discesa a destra per **[!UICONTROL Engagement]**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Selezionare **[!UICONTROL Contact.Engagement]** nell&#39;elenco.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

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

1. Al termine, fai clic su **[!UICONTROL Save]**.

## Scheda di configurazione di Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. In Salesforce, fare clic su **+** alla fine della barra delle schede e fare clic su **[!UICONTROL Marketo Sales Insight Config]**.

1. Copiare le credenziali dal pannello API Soap nella [pagina di amministrazione di Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} e incollarle nella sezione API Soap della pagina di configurazione [!DNL Salesforce] [!DNL Sales Insight].

1. Copiare le credenziali dal pannello API REST nella [pagina di amministrazione di Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} e incollarle nella sezione API REST della pagina di configurazione [!DNL Salesforce] [!DNL Sales Insight].

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

Dovresti essere in grado di visualizzare i campi Marketo Sales Insight per lead, contatti, account e opportunità.

>[!NOTE]
>
>Se il test di diagnostica non è riuscito, [aggiungere altri campi al layout di pagina](https://nation.marketo.com:443/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} potrebbe risolvere il problema.

>[!NOTE]
>
>Per gli account, Sales Insight include tutte le e-mail, ma solo i momenti di interesse più recenti, l’attività web e le modifiche dei punteggi.

>[!MORELIKETHIS]
>
>* [Priorità, Urgenza, Punteggio relativo e Elementi di maggiore rilevanza](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Aggiungi scheda Marketo a [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Aggiungere l&#39;accesso di Insight alle vendite ai profili](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
