---
unique-page-id: 3571844
description: Sincronizzazione Microsoft Dynamics - Sincronizzazione opportunità - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione Microsoft Dynamics - Sincronizzazione opportunità
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 9a130e0b2ec84b638adf37188b65b565b090fe1b
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Sincronizzazione Microsoft Dynamics: Sincronizzazione opportunità {#microsoft-dynamics-sync-opportunity-sync}

La sincronizzazione da Marketo Engage a Dynamics è estremamente potente. Di seguito sono riportati tutti i dettagli relativi alla sincronizzazione delle opportunità.

## In che modo i dettagli delle opportunità vengono mantenuti sincronizzati tra i due sistemi? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La sincronizzazione delle opportunità è unidirezionale: da Dynamics a Marketo. Se apporti modifiche a un’opportunità in Dynamics, l’aggiornamento si rifletterà in Marketo.

## È possibile creare un’opportunità in Dynamics utilizzando Marketo? {#can-i-create-an-opportunity-in-dynamics-using-marketo}

No, devi creare l’opportunità in Dynamics che verrà sincronizzata automaticamente con Marketo.

## Quali campi verranno sincronizzati con Marketo? {#what-fields-will-sync-to-marketo}

È possibile [selezionare i campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante l&#39;installazione.

## In che modo un account/contatto è associato a un’opportunità? {#how-is-an-account-contact-associated-with-an-opportunity}

Il contatto/account può essere associato all’opportunità in due modi:

* Durante la creazione di un’opportunità, è possibile impostare Contatto (campo di ricerca nel modulo da contattare) e/o Account (campo di ricerca nel modulo da account). In entrambi i casi, questi valori vengono memorizzati nel campo Cliente potenziale (customerid) in Dynamics. Questo campo non viene visualizzato nel modulo dell’opportunità, ma può essere aggiunto dalle impostazioni. Questo campo può contenere solo 1 valore, contatto o account. Marketo esegue le operazioni seguenti:

   * Se il valore del contatto è impostato e l&#39;account viene lasciato vuoto, Marketo crea un account `opportunitycontactrole` e imposta l&#39;account dell&#39;opportunità sull&#39;account del contatto. Se il contatto non dispone di un account, questo campo viene lasciato vuoto.
   * Se il valore dell&#39;account è impostato e il contatto viene lasciato vuoto, Marketo imposterà l&#39;account solo sull&#39;opportunità.
   * Se sono impostati entrambi i valori, Dynamics sceglie account come valore per customerid, in modo che il comportamento sia lo stesso di cui sopra.


* Tramite parti interessate: Dynamics utilizza le connessioni per connettere l’opportunità di contattare le parti interessate dalla pagina di creazione dell’opportunità. Per questo, creeremo un record `opportunitycontactrole` per ogni nuovo stakeholder.
