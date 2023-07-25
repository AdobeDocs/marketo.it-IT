---
unique-page-id: 37355534
description: Note sulla versione - Gennaio 2020 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Gennaio 2020
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Note sulla versione: gennaio 2020 {#release-notes-jan}

Le seguenti funzioni sono incluse nella versione del 20 gennaio. Verifica la disponibilità delle funzioni nella tua edizione di Marketo.

>[!AVAILABILITY]
>
>Caratteristiche contrassegnate da una stella ( ![(stella)](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

**_Versioni trimestrali_**

Le seguenti funzioni verranno rilasciate il **17 gennaio 2020**.

## Applicazione Adobe Marketo Engage core {#core-marketo-engage-adobe-application}

* [Selettore risorse Adobe Experience Manager](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md): accedi rapidamente alle risorse in linea con il tuo marchio con le risorse AEM disponibili direttamente nel Marketo Engage. Nota: anche se questa funzione è disponibile sia nelle nostre esperienze Marketo Sky che in quelle classiche, le funzionalità amministrative sono disponibili anche nella nostra esperienza classica. Devi essere un cliente di AEM Assets e disporre della versione 6.5 o successiva.

>[!NOTE]
>
>Attualmente, il selettore di risorse AEM è completamente supportato solo in Firefox. Non è supportato in Safari e potrebbe non funzionare nella versione più recente di Chrome (v. 80), a seconda delle impostazioni del cookie SameSite.

* **Microsoft Dynamics - Sincronizza lead con CRM in tempo reale**: sincronizzazione in tempo reale di lead e contatti tra Marketi Engage e Microsoft Dynamics. Crea lead o contatti e visualizzali immediatamente in Microsoft Dynamics con l’azione di flusso &quot;Sincronizza persona con Microsoft&quot;.
* **Mappatura campi aggiuntivi Forms linkedIn Lead Gen**: acquisisci i dati dei lead da LinkedIn Lead Gen Forms per creare esperienze più rilevanti sia per i punti di contatto di vendita che per quelli di marketing. Estrai i campi nascosti, i campi di consenso e il campo dei lead di test in Marketo Engage.
* **API dipendenze modello e-mail**: ottieni un elenco di risorse che dipendono da un modello e-mail per comprendere l’ambito delle potenziali modifiche e le dipendenze degli indirizzi dai modelli possono essere modificate ed eliminate più rapidamente.
* **Miglioramenti alla gestione di più istanze**: passa rapidamente all’istanza necessaria con un menu a discesa scorrevole e alfabetico delle sottoscrizioni.

## Account-Based Marketing {#account-based-marketing}

![(stella)](assets/yellow-star.png)

* **[Individuazione nuovo account (BETA)](https://docs.marketo.com/x/WQA6Ag) ![(stella)](assets/yellow-star.png)**: utilizza la funzione di profilazione dell’account per individuare nuovi account di destinazione per la strategia ABM in base al modello di profilo cliente ideale basato sull’intelligenza artificiale. Visualizza, seleziona e importa nuovi account consigliati, insieme ai relativi indicatori di dati di idoneità e intento basati su IA, che non esistono già nel database dei lead di Marketo Engage e degli account per il targeting ABM. Disponibile immediatamente per i clienti idonei per la profilazione degli account.

<br> 

**_Rilascio nel corso del trimestre_**

Le seguenti funzioni sono in un ciclo non trimestrale e verranno rilasciate nei prossimi mesi.

## Bizible {#bizible}

![(stella)](assets/yellow-star.png)

* **Integrazione dei lead di Marketo Engage**: unisci vendite e marketing con una visione unificata dei lead tra Bizible e Marketi Engage. Con questo aggiornamento, il Marketo Engage ora può essere utilizzato come origine dati del lead aggiuntiva, quindi non è più necessario attendere che i lead vengano sincronizzati con il sistema di gestione delle relazioni con i clienti per generare rapporti sulla generazione di lead.
* **Scopri i miglioramenti**: per saperne di più, scopri le bacheche in Bizible con miglioramenti sviluppati dal feedback dei clienti, come la possibilità di espandere i record transazionali da riquadri e attributi, aggiungere conteggi di record essenziali e le metriche costo per corrispondenti e aggiungere/rimuovere filtri dashboard per più dashboard. Al momento dell’accesso, verrai indirizzato direttamente al dashboard predefinito.

## Marketo Sky {#marketo-sky}

* [Editing immagini](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=en#design-studio): consente di accedere alle funzionalità di modifica di Adobe senza uscire dal Marketo Engage. Questa nuova funzionalità consente di eseguire facilmente operazioni quali migliorare, ritagliare e aggiungere testo alle immagini direttamente in Design Studio.

## Insight sulle vendite {#sales-insight}

* **Azioni collettive Salesforce Lightning**: aumenta l’efficienza delle vendite e mantiene gli acquirenti coinvolti con la possibilità di aggiungere fino a 200 contatti/lead per campagne e inviare loro e-mail di Marketo Engage in blocco con Salesforce Lightning.
* **Supporto mobile per Salesforce1**: ora puoi accedere da dispositivi mobili a tutte le funzioni di Sales Insight, come Momenti di interesse e Attività web ed e-mail, direttamente nell’app Salesforce1.
* **Miglioramenti dell’interfaccia utente**: interfaccia aggiornata con miglioramenti a livello di leggibilità e un design coerente con la nostra esperienza Marketo Sky.

## Sales Connect {#sales-connect}

* **Componenti griglia**: ottimizza l’istanza Sales Connect con nuove funzionalità di personalizzazione della griglia. Scegliere le colonne da visualizzare, cercare le colonne, selezionare o deselezionare tutte le colonne e determinare il numero di righe di dati da visualizzare in ogni pagina.
* **[Blocco dei contenuti](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**: massimizza l’allineamento del brand con un’impostazione a livello di abbonamento che controlla se gli utenti non amministratori possono creare e modificare modelli e campagne.

>[!NOTE]
>
>* **Obsolescenza di TLS 1.0 e 1.1**: con il continuo sforzo di integrazione con la struttura di rilascio di Adobe, abbiamo spostato la rimozione di TLS 1.0 e TLS 1.1 al 13 gennaio 2020. Ulteriori informazioni sono disponibili [qui](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
>
>* **Aggiornamento ITP 2.1+ Munchkin**: a causa delle modifiche alla policy sui cookie per Safari, la capacità di Munchkin di monitorare gli utenti tra sessioni sullo stesso dominio sarà limitata da ITP a 1 o 7 giorni in base al browser e alla versione del browser utilizzati dal visitatore. Per questo, stiamo implementando un nuovo servizio web per consentire l’impostazione dei cookie Munchkin con un’intestazione Set-Cookie tramite risposta HTTP. Ulteriori informazioni su come implementare questo nuovo servizio sono disponibili [qui](https://nation.marketo.com/docs/DOC-7351).

**_Webinar sulla versione del prodotto_** [Partecipa](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) il 3 marzo alle 11:00 PT / 2:00 ET per un webinar live ospitato dal nostro team di prodotto e ulteriori informazioni sulle funzioni incluse in questa versione.
