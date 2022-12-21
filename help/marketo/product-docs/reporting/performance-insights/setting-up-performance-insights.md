---
unique-page-id: 12981145
description: Configurazione di informazioni sulle prestazioni - Documentazione Marketo - Documentazione del prodotto
title: Impostazione di informazioni sulle prestazioni
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Impostazione di informazioni sulle prestazioni {#setting-up-performance-insights}

Per impostare MPI, effettua le seguenti operazioni.

## Impostazione opportunità {#opportunity-setup}

1. Fai clic su **Amministratore**.

   ![](assets/admin.png)

1. Fai clic su **Analisi del ciclo dei ricavi**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Se non hai RCA, dovrai selezionare **Analisi del programma** per il passaggio 2.

1. In Attribution, fai clic su **Modifica**.

   ![](assets/three-1.png)

1. Vengono visualizzate le impostazioni di attribuzione.

   ![](assets/four-2.png)

   Se Attribution è esplicito, assicurati che il ruolo Contatto opportunità sia stato popolato (tramite l’endpoint Ruolo opportunità o tramite l’integrazione con CRM).

   Se Attribution è implicito, assicurati che il campo società sul lead/contatto sia lo stesso del Nome account dell’opportunità.

   >[!NOTE]
   >
   >Assicurati che tutti i campi appropriati siano compilati:
   >
   >* Importo opportunità
   >* È chiuso
   >* Vinato
   >* Data creazione (potrebbe non essere impostata nel caso in cui lo si verifichi)
   >* Data di chiusura (potrebbe non essere impostata nel tuo caso)
   >* Tipo di opportunità


## Configurazione del programma {#program-setup}

Aggiornare i costi del programma per almeno 12 mesi. Puoi eseguire questa operazione manualmente o utilizzando l’API del programma. In questo esempio lo facciamo manualmente.

1. Fai clic su **Attività di marketing**.

   ![](assets/ma.png)

1. Trova e seleziona il programma.

   ![](assets/select-program.png)

1. Fai clic sul pulsante **Configurazione** scheda .

   ![](assets/setup-tab.png)

1. Trascina **Costo del periodo** sulla tela.

   ![](assets/period-cost.png)

1. Imposta il mese del programma almeno 12 mesi fa e fai clic su **Ok**.

   ![](assets/set-period.png)

1. Imposta il costo del periodo e fai clic su **Salva**.

   ![](assets/set-cost.png)

Quindi, controlla il comportamento di analisi per indicare se un particolare canale deve essere incluso in analytics. Imposta il comportamento di Analytics (Normale, Inclusivo, Operativo).

1. Fai clic su **Amministratore**.

   ![](assets/admin.png)

1. Fai clic su **Tag**.

   ![](assets/tags.png)

1. Fai clic sul pulsante **+** per espandere l’elenco Canale.

   ![](assets/channel.png)

1. Fai doppio clic sul canale desiderato.

   ![](assets/channel-click.png)

1. Fai clic sul pulsante **Comportamento di Analytics** e seleziona il comportamento desiderato.

   ![](assets/edit-channel.png)

1. Imposta i criteri di successo.

   ![](assets/success.png)

1. Fai clic su **Salva**.

   ![](assets/save.png)

## Legare il programma alla persona {#tie-the-program-to-the-person}

1. Assicurati che il programma di acquisizione e la data di acquisizione siano stati impostati per ciascuna persona nel database in modo che l&#39;attribuzione Primo contatto funzioni.
1. Assicurati che i tuoi programmi impostino gli stati di successo per il tuo personale.

>[!NOTE]
>
>Le modifiche apportate non sono istantanee. È necessario un periodo overnight prima che le modifiche entrino in vigore.
