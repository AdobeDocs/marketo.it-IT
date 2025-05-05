---
unique-page-id: 37355534
description: Note sulla versione - Gennaio 2020 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Gennaio 2020
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
feature: Release Information
source-git-commit: 89995b2cd6fdc2f2e4ea43906304bdf16d367de1
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 0%

---

# Note sulla versione: gennaio 2020 {#release-notes-jan}

Le seguenti funzioni sono incluse nella versione del 20 gennaio. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella ( ![(stella)](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzionalità verranno rilasciate il **17 gennaio 2020**.

## Applicazione Adobe Marketo Engage core {#core-marketo-engage-adobe-application}

* [Selettore risorse Adobe Experience Manager](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md): accedi rapidamente alle risorse allineate al tuo marchio con le risorse AEM disponibili direttamente nel Marketo Engage. Nota: anche se questa funzione è disponibile sia nelle nostre esperienze Marketo Sky che in quelle classiche, le funzionalità amministrative sono disponibili anche nella nostra esperienza classica. Devi essere un cliente di AEM Assets e disporre della versione 6.5 o successiva.

>[!NOTE]
>
>Attualmente, il selettore di risorse AEM è completamente supportato solo in Firefox. Non è supportato in Safari e potrebbe non funzionare nella versione più recente di Chrome (v. 80), a seconda delle impostazioni dei cookie SameSite.

* **Microsoft Dynamics - Sincronizza lead con CRM in tempo reale**: sincronizzazione in tempo reale di lead e contatti tra il Marketo Engage e Microsoft Dynamics. Crea lead o contatti e visualizzali immediatamente in Microsoft Dynamics con l’azione di flusso &quot;Sincronizza persona con Microsoft&quot;.
* **Mappatura campi aggiuntivi Forms lead di LinkedIn**: acquisisci i dati dei lead da LinkedIn Lead Gen Forms per creare esperienze più rilevanti sia per i punti di contatto di vendita che per quelli di marketing. Estrai i campi nascosti, i campi di consenso e il campo dei lead di test in Marketo Engage.
* **API delle dipendenze dei modelli e-mail**: ottieni un elenco di risorse che dipendono da un modello e-mail per comprendere l&#39;ambito delle potenziali modifiche e indirizzare le dipendenze ai modelli in modo che possano essere modificate ed eliminate più rapidamente.
* **Miglioramenti alla gestione di più istanze**: accedi rapidamente all&#39;istanza desiderata con un menu a discesa scorrevole e alfabetico delle sottoscrizioni.

## Account-Based Marketing {#account-based-marketing}

![(stella)](assets/yellow-star.png)

* [Nuova individuazione account (BETA)](https://docs.marketo.com/x/WQA6Ag) ![(star)](assets/yellow-star.png): utilizza la profilatura account per individuare nuovi account di destinazione per la strategia ABM basata sul modello di profilo cliente ideale basato sull&#39;intelligenza artificiale. Visualizza, seleziona e importa nuovi account consigliati, insieme ai relativi indicatori di dati di idoneità e intento basati su IA, che non esistono già nel database dei lead di Marketo Engage e degli account per il targeting ABM. Disponibile immediatamente per i clienti idonei per la profilazione degli account.

<br> 

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## Bizible {#bizible}

![(stella)](assets/yellow-star.png)

* **Integrazione lead di Marketo Engage**: unisci vendite e marketing con una visualizzazione unificata dei lead tra Bizible e Marketo Engage. Con questo aggiornamento, il Marketo Engage ora può essere utilizzato come origine dati del lead aggiuntiva, quindi non è più necessario attendere che i lead vengano sincronizzati con il sistema di gestione delle relazioni con i clienti per generare rapporti sulla generazione di lead.
* **Scopri i miglioramenti**: scopri di più dalle nostre Discover Boards in Bizible con miglioramenti sviluppati dal feedback dei clienti, come la possibilità di espandere i record transazionali da sezioni e attributi, aggiungere conteggi di record essenziali e metriche corrispondenti del costo per e aggiungere/rimuovere filtri dashboard per più dashboard. Al momento dell’accesso, verrai indirizzato direttamente al dashboard predefinito.

## Marketo Sky {#marketo-sky}

* [Modifica immagini](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=it#design-studio): accedi alle funzionalità di modifica di Adobe senza uscire dal Marketo Engage. Questa nuova funzionalità consente di eseguire facilmente operazioni quali migliorare, ritagliare e aggiungere testo alle immagini direttamente in Design Studio.

## Insight sulle vendite {#sales-insight}

* **Salesforce Lightning Bulk Actions**: migliora l&#39;efficienza delle vendite e mantiene gli acquirenti coinvolti con la possibilità di aggiungere fino a 200 contatti/lead alle campagne e inviare loro e-mail di Marketo Engage in blocco con Salesforce Lightning.
* **Supporto mobile per Salesforce1**: ora puoi accedere da dispositivi mobili a tutte le funzioni di Sales Insight, come Momenti di interesse e Attività Web e e-mail, direttamente nell&#39;app Salesforce1.
* **Miglioramenti all&#39;interfaccia utente**: interfaccia aggiornata con miglioramenti alla leggibilità e una progettazione coerente con la nostra esperienza Marketo Sky.

## Sales Connect {#sales-connect}

* **Componenti Grid**: ottimizza l&#39;istanza Sales Connect con nuove funzionalità di personalizzazione della griglia. Scegliere le colonne da visualizzare, cercare le colonne, selezionare o deselezionare tutte le colonne e determinare il numero di righe di dati da visualizzare in ogni pagina.
* **[Blocco dei contenuti](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**: massimizza l&#39;allineamento del brand con un&#39;impostazione a livello di abbonamento che controlla se i non amministratori possono creare e modificare modelli e campagne.

>[!NOTE]
>
>* **Deprecazione di TLS 1.0 e 1.1**: in un continuo sforzo di integrazione con la struttura delle versioni di Adobe, la rimozione di TLS 1.0 e TLS 1.1 verrà spostata al 13 gennaio 2020. Ulteriori informazioni sono disponibili [qui](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
>
>* **Aggiornamento Munchkin ITP 2.1+**: a causa delle modifiche ai criteri dei cookie per Safari, la capacità di Munchkin di tenere traccia degli utenti tra sessioni sullo stesso dominio sarà limitata da ITP a 1 o 7 giorni in base alla versione del browser e del browser utilizzati dal visitatore. Per questo, stiamo implementando un nuovo servizio web per consentire l’impostazione dei cookie di Munchkin con un’intestazione Set-Cookie tramite risposta HTTP. Ulteriori informazioni sull&#39;implementazione di questo nuovo servizio sono disponibili [qui](https://nation.marketo.com/docs/DOC-7351).

**_Webinar sulla versione del prodotto_** [Unisciti a noi](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) il 3 marzo alle 11:00AM PT / 2:00PM ET per un webinar live ospitato dal nostro team di prodotto e ulteriori informazioni sulle funzioni incluse in questa versione.
