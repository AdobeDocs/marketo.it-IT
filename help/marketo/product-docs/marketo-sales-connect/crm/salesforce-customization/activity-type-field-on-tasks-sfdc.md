---
unique-page-id: 14352476
description: Campo Tipo di attività sulle attività (SFDC) - Documentazione di Marketo - Documentazione del prodotto
title: Campo Tipo di attività su Attività (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 7%

---

# Campo Tipo di attività su Attività (SFDC) {#activity-type-field-on-tasks-sfdc}

Con l&#39;aiuto di [!DNL Sales Connect] puoi registrare le tue e-mail e chiamate come attività in [!DNL Salesforce]. Una parte fondamentale per avere dati importanti in [!DNL Salesforce] è che il campo [!UICONTROL Type] popola il valore corretto.

>[!NOTE]
>
>La registrazione delle e-mail tramite Ccn non verrà visualizzata nell&#39;elenco a discesa Tipo di attività e al suo posto verrà automaticamente compilato il campo del tipo come &quot;e-mail&quot;, poiché vengono recapitate a [!DNL Salesforce] tramite il tuo indirizzo Ccn.

## Requisiti {#requirements}

* Connessione con [!DNL Salesforce]
* Nessun valore Tipo predefinito selezionato nell&#39;elenco a discesa Tipo di task
* Chiamata, Risposta ed E-mail devono essere presenti nell&#39;elenco a discesa Tipo di task (le maiuscole sono importanti)
* Nessun flusso di lavoro o trigger che interviene sul valore del campo Tipo

## Configurazione {#setup}

Verifica innanzitutto di disporre dei valori corretti per l’elenco a discesa. Per apportare modifiche all&#39;elenco di selezione, è necessario l&#39;aiuto dell&#39;amministratore [!DNL Salesforce].

1. Passa a [Salesforce.com](https://salesforce.com) e fai clic su Configurazione nell&#39;angolo in alto a destra.
1. Fai clic su **[!UICONTROL Customize]**.
1. Fai clic su **[!UICONTROL Activities]**.
1. Fai clic su **[!UICONTROL Task Fields]**.
1. Fai clic su **[!UICONTROL Type]**.
1. Ora ti trovi nell’elenco a discesa Tipo di attività. Assicurati che non sia selezionato &quot;Predefinito&quot;.
1. Verificare che sia presente un valore [!UICONTROL Type] elencato per [!UICONTROL Email], [!UICONTROL Call] e [!UICONTROL Reply].

Ora che questa è attiva, inizierai a vedere che il campo Tipo popola il valore corrispondente per e-mail, chiamate e risposte registrate. Questi valori _non_ verranno inseriti nelle attività promemoria di Sales Connect.

>[!NOTE]
>
>Se il valore &quot;Reply&quot; non è visualizzato, aggiungerlo facendo clic su **[!UICONTROL New]**. &#39;Reply&#39; non è un valore standard in [!DNL Salesforce].
