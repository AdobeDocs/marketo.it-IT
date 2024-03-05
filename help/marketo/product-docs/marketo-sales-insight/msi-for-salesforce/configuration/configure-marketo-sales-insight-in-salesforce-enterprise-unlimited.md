---
unique-page-id: 2360368
description: Scopri come configurare Marketo Sales Insight nelle edizioni Salesforce Enterprise/Unlimited.
title: Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 3cbefabe80778b0502eaecd733b5732fd9003316
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Configurare Marketo Sales Insight nelle edizioni Salesforce Enterprise/Unlimited completando i passaggi seguenti.

>[!PREREQUISITES]
>
>[Installare il pacchetto Marketo Sales Insight nell’AppExchange di Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Sono necessarie le autorizzazioni di amministratore.**

## Configura approfondimenti vendite nel Marketo Engage {#configure-sales-insight-in-marketo}

1. Per ottenere le credenziali di Marketo Sales Insight nel Marketo Engage, vai al **[!UICONTROL Amministratore]** area e selezione **[!UICONTROL Insight sulle vendite]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Clic **[!UICONTROL Modifica configurazione API]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Inserisci una chiave segreta API a tua scelta e fai clic su **[!UICONTROL Salva]**. NON utilizzare una e commerciale (`&`) nella chiave segreta API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >La chiave segreta API è una password per la tua organizzazione e deve essere sicura.

1. Per compilare le credenziali, fai clic su **[!UICONTROL Visualizza]** nel _[!UICONTROL Configurazione API REST]_ pannello.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Quando viene visualizzata una finestra di dialogo di conferma, fai clic su **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Tieni aperta questa finestra. Queste informazioni sono necessarie successivamente per la configurazione di Salesforce.

## Configurare Sales Insight in Salesforce {#configure-sales-insight-in-salesforce}

1. In Salesforce, fai clic su **[!UICONTROL Configurazione]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Cercare &quot;sito remoto&quot; e selezionare **[!UICONTROL Impostazioni sito remoto]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Clic **[!UICONTROL Nuovo sito remoto]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Immetti il nome del sito remoto (può essere simile a `MarketoSoapAPI`). Immetti l&#39;URL del sito remoto, che è l&#39;URL dell&#39;host Marketo dalla _[!UICONTROL Configurazione API Soap]_ nel Marketo Engage. Clic **[!UICONTROL Salva]**. Sono state create le impostazioni del sito remoto per l’API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Clic **[!UICONTROL Nuovo sito remoto]** di nuovo.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Immetti il nome del sito remoto (può essere simile a `MarketoAPI`). Immetti l’URL del sito remoto, che è l’URL API da _[!UICONTROL Configurazione API REST]_ nel Marketo Engage. Clic **[!UICONTROL Salva]**. Sono state create le impostazioni del sito remoto per l’API REST.

   >[!NOTE]
   >
   >_Tu_ scegli il tuo **[!UICONTROL Nome sito remoto]** (`MarketoAPI` viene utilizzato qui). Il **[!UICONTROL URL sito remoto]** sono disponibili nel campo Host Marketo della finestra di dialogo Modifica configurazione API dal passaggio 3 nella sezione &quot;Configura approfondimenti vendite in Marketo&quot;.

## Concedi agli utenti di Sales Insight l’accesso al profilo per gli oggetti Salesforce standard {#grant-sales-insight-users-profile-access}

A causa dei miglioramenti apportati alla sicurezza di Salesforce, i pacchetti di AppExchange non possono più concedere l’autorizzazione agli oggetti standard e l’accesso deve essere concesso agli oggetti Salesforce pertinenti dal profilo dell’utente Salesforce. Per concedere le autorizzazioni necessarie, segui la procedura riportata di seguito.

1. Clic **[!UICONTROL Configurazione]**.

1. Cerca &quot;Profili&quot; nella Ricerca rapida.

1. Clic **[!UICONTROL Modifica]** accanto al profilo utilizzato dagli utenti Salesforce.

1. Sotto _[!UICONTROL Autorizzazione oggetto standard]_ sezione, abilita **[!UICONTROL Letto]** accesso per i seguenti oggetti: [!UICONTROL Lead], [!UICONTROL Contatto], [!UICONTROL Account], e [!UICONTROL opportunità].

1. Fai clic su **[!UICONTROL Salva]**.

## Personalizzare i layout di pagina {#customize-page-layouts}

1. Clic **[!UICONTROL Configurazione]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Cerca &quot;layout di pagina&quot; e seleziona la **[!UICONTROL Layout di pagina]** in **[!UICONTROL Lead]**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Clic **[!UICONTROL Visualforce Pages]** a sinistra. Trascina **[!UICONTROL Sezione]** al layout sotto il _[!UICONTROL Collegamenti personalizzati]_ sezione.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Immetti &quot;Marketo Sales Insight&quot; come **[!UICONTROL Nome sezione]**, seleziona **[!UICONTROL 1 colonna]** e fai clic su **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Trascina **[!UICONTROL Lead]** nella nuova sezione.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Il nome di questa casella cambia in base al tipo di oggetto. Se ad esempio si modifica il layout di pagina per i contatti, verrà visualizzato Contatto.

1. Fai doppio clic su **[!UICONTROL Lead]** blocco appena aggiunto.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Modifica altezza in **450** pixel e fai clic su **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Verifica **[!UICONTROL Mostra barre di scorrimento]** se hai bisogno di accedere alle attività di scorrimento.

   >[!TIP]
   >
   >L&#39;altezza consigliata per gli oggetti Account e Opportunità è di 410 pixel.

1. Clic **[!UICONTROL Campi]** a sinistra. Quindi cerca e trascina il **[!UICONTROL Urgenza]** etichetta in **[!UICONTROL Insight sulla vendita di Marketo]** layout.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. Ripeti il passaggio precedente anche per questi campi.

   * Ultimo momento di interesse
   * Data ultimo momento di interesse
   * Descrizione ultimo momento di interesse
   * Sorgente ultimo momento di interesse
   * Tipo ultimo momento di interesse
   * Ultima attività per vendite
   * Ultimo coinvolgimento per vendite
   * ID contatto MSI
   * Punteggio relativo
   * Valore punteggio relativo
   * Urgenza
   * Valore Urgenza
   * Visualizza in Marketo

1. Clic **[!UICONTROL Salva]** al termine.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Ripeti i passaggi 5-7 per aggiungere sezioni di pagina e campi approfondimento vendite di Visualforce per **[!UICONTROL Contatto]**, **[!UICONTROL Account]**, e **[!UICONTROL opportunità]**.

1. Ripeti i passaggi 8-10 per aggiungere questi campi di approfondimento sulle vendite per **[!UICONTROL Contatto]**. Assicurati di salvare tutte le modifiche.

   * Ultimo momento di interesse
   * Data ultimo momento di interesse
   * [!UICONTROL Descrizione ultimo momento di interesse]
   * [!UICONTROL Sorgente ultimo momento di interesse]
   * [!UICONTROL Tipo ultimo momento di interesse]
   * [!UICONTROL Ultima attività Marketo per vendite]
   * [!UICONTROL Ultimo coinvolgimento Marketo per vendite]
   * [!UICONTROL Punteggio lead MKTO]
   * [!UICONTROL Punteggio relativo]
   * [!UICONTROL Valore punteggio relativo]
   * [!UICONTROL Insight sulle vendite] - Apre la pagina dell&#39;elenco completo contatti
   * [!UICONTROL Urgenza]
   * [!UICONTROL Valore Urgenza]

## Mappa campi persona personalizzati {#map-custom-person-fields}

I campi della persona Marketo devono essere mappati sui campi del contatto Salesforce per garantire il corretto funzionamento della conversione. Segui questi passaggi per mapparli.

1. Clic **[!UICONTROL Configurazione]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Cerca i &quot;campi&quot; nella barra di ricerca e fai clic su **[!UICONTROL Campi]** in **[!UICONTROL Lead]**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Clic **[!UICONTROL Mappa campi lead]**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Fai clic sul menu a discesa a destra per **[!UICONTROL Coinvolgimento]**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Seleziona **[!UICONTROL Contact.Engagement]** nell&#39;elenco.

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

1. Clic **[!UICONTROL Salva]** quando hai finito.

## Scheda di configurazione di Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. In Salesforce, fai clic su **+** alla fine della barra delle schede e fare clic su **[!UICONTROL Configurazione approfondimento vendite Marketo]**.

1. Copiare le credenziali dal pannello API Soap in [Pagina di amministrazione di Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} e incollali nella sezione API Soap della pagina Configurazione di Salesforce Sales Insight.

1. Copiare le credenziali dal pannello API Rest in [Pagina di amministrazione di Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} e incollali nella sezione API Rest della pagina Configurazione di Salesforce Sales Insight.

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

Dovresti essere in grado di visualizzare i campi Insight vendite Marketo per lead, contatti, account e opportunità.

>[!NOTE]
>
>Se il test di diagnostica non è riuscito, [aggiunta di altri campi al layout della pagina](https://nation.marketo.com:443/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} potrebbe risolvere il problema.

>[!NOTE]
>
>Per gli account, Sales Insight include tutte le e-mail, ma solo i momenti di interesse più recenti, l’attività web e le modifiche dei punteggi.

>[!MORELIKETHIS]
>
>* [Priorità, urgenza, punteggio relativo e elementi di maggiore rilevanza](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Aggiungi scheda Marketo a Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Aggiungere l’accesso a Sales Insight ai profili](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
