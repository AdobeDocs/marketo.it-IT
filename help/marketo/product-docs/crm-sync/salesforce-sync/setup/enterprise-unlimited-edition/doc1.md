---
description: Passaggio 1 di 3 - Aggiungere campi Marketo a Salesforce (Enterprise/Unlimited) - Documenti Marketo - Documentazione del prodotto
title: Passaggio 1 di 3 - Aggiungere campi Marketo a Salesforce (Enterprise/Unlimited)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 1%

---

# Passaggio 1 di 3: aggiungere campi Marketo a Salesforce (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>Per eseguire la sincronizzazione tra Marketo Engage e Salesforce, è necessario avere accesso alle API di Salesforce.

Marketo utilizza un set di campi per acquisire determinati tipi di informazioni di marketing. Se desideri questi dati in Salesforce, segui le istruzioni riportate di seguito.

1. Crea tre campi personalizzati in Salesforce sugli oggetti lead e contatto: Punteggio, Programma di acquisizione e Data di acquisizione.
1. Mappa questi campi personalizzati tra lead e contatti in modo che, al momento della conversione in Salesforce, i valori vengano riportati.
1. Se necessario, puoi creare altri campi aggiuntivi (vedi la tabella seguente).

Tutti questi campi personalizzati sono facoltativi e non sono necessari per sincronizzare Marketo e Salesforce. Come best practice, consigliamo di creare campi per Punteggio, Programma di acquisizione e Data di acquisizione.

## Aggiungere campi Marketo a Salesforce {#add-marketo-fields-to-salesforce}

Aggiungi tre campi personalizzati agli oggetti lead e contatto in Salesforce elencati sopra. Per aggiungerne altri, vedere la tabella dei campi disponibili alla fine di questa sezione.

Per aggiungerli, effettua le seguenti operazioni per ciascuno dei tre campi personalizzati. Inizia con Punteggio.

1. Accedi a Salesforce e fai clic su Configurazione.

   SCHERMATA

1. Nella Ricerca rapida cercare la parola &quot;Object&quot;

   SCHERMATA

1. Fare clic su Object Manager e cercare &quot;Lead&quot;

   SCHERMATA

1. Fare clic su Lead in ETICHETTA e quindi su Campi e relazioni a sinistra.

   SCHERMATA

1. Fai clic sul pulsante Nuovo nella pagina &quot;Campi e relazioni&quot;.

   SCHERMATA

1. Scegli il tipo di campo appropriato (per Punteggio - Numero; Programma di acquisizione - Testo; Data di acquisizione - Data/ora).

   SCHERMATA

1. Fai clic su Avanti.

   SCHERMATA

1. Immettere l&#39;Etichetta campo, la Lunghezza e il Nome campo per il campo, come illustrato nella tabella seguente.

   TABELLA

   >[!NOTE]
   >
   >Salesforce aggiunge __c ai nomi dei campi quando li utilizza per creare i nomi API.

   SCHERMATA

   >[!NOTE]
   >
   >I campi di testo e numerici richiedono una lunghezza, ma i campi di data e ora non la richiedono. Una descrizione è facoltativa.

1. Fai clic su Avanti.

   SCHERMATA

1. Specificare le impostazioni di accesso e fare clic su Avanti:

   Imposta tutti i ruoli su Visibile e Sola lettura

   Deselezionare la casella di controllo Sola lettura per il profilo dell&#39;utente di sincronizzazione:

   Se come utente di sincronizzazione è presente un utente con il profilo Amministratore di sistema, deselezionare la casella di controllo Sola lettura per il profilo Amministratore di sistema (come illustrato di seguito)
Se è stato creato un profilo personalizzato per l&#39;utente di sincronizzazione, deselezionare la casella di controllo Sola lettura per il profilo personalizzato

   SCHERMATA

1. Scegliere i layout di pagina da visualizzare nel campo.

   SCHERMATA

1. Fai clic su Salva e nuovo per tornare indietro e creare ciascuno degli altri due campi personalizzati. Fai clic su Salva. Hai terminato tutte e tre le operazioni.

   SCHERMATA

* In Object Manager, cercare &quot;Contatti&quot;. Fare clic su Campi e relazioni.
* Eseguire i passaggi da 5 a 12 per i campi Punteggio, Data acquisizione e Programma di acquisizione sull&#39;oggetto contatto, come è stato fatto per l&#39;oggetto lead.
* Facoltativamente, utilizza la procedura precedente per tutti i campi personalizzati aggiuntivi di questa tabella.

  TABELLA

  >[!NOTE]
  >
  >I valori nei campi assegnati automaticamente da Marketo non saranno immediatamente disponibili in Salesforce al momento della creazione del nuovo campo. Marketo sincronizzerà i dati con Salesforce al prossimo aggiornamento del record di uno dei due sistemi (ovvero, un aggiornamento di uno qualsiasi dei campi sincronizzati tra Marketo e Salesforce).

## Mappa campi personalizzati per conversioni {#map-custom-fields-for-conversions}

Un campo personalizzato sull’oggetto lead in Salesforce deve essere mappato su un campo contatto nell’oggetto contatto in modo che i dati vengano trasferiti quando si verifica una conversione.

1. Nell’angolo in alto a destra, fai clic su Configurazione.

   SCHERMATA

1. Nella Ricerca rapida cercare la parola &quot;Object&quot;

   SCHERMATA

1. Vai alla sezione Campi personalizzati lead e relazioni e fai clic su Mappa campi lead

   SCHERMATA

1. Fai clic sul menu a discesa accanto al campo che desideri mappare, nella scheda corrispondente- account, contatto o opportunità.

   SCHERMATA

1. Selezionare il campo personalizzato del contatto corrispondente.

   SCHERMATA

1. Ripeti i passaggi precedenti per tutti gli altri campi creati.

1. Al termine, fai clic su Salva.
