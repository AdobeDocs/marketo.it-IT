---
unique-page-id: 2359646
description: Configurare il profilo progressivo del modulo - Documenti Marketo - Documentazione del prodotto
title: Configura profilo progressivo modulo
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---


# Configura profilo progressivo modulo {#configure-form-progressive-profiling}

Le forme brevi sono buone! Quando un utente torna a un modulo, è possibile presentare nuovi campi e compilare progressivamente il profilo del visitatore. Ecco come.

>[!NOTE]
>
>Affinché questa funzione funzioni correttamente, accertatevi che la funzione di precompilazione del modulo sia abilitata per i campi visibili e [disattivata](http://docs.marketo.com/display/DOCS/Disable+Pre-fill+for+a+Form+Field) per i campi nascosti.

1. Vai a **Marketing** **Activities**.

   ![](assets/ma-1.png)

1. Selezionare il modulo e fare clic su **Modifica** **modulo**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. In **Impostazioni** **modulo** fare clic su **Impostazioni**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Imposta **Profiling progressivo** **su** Abilitato ****.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Ok, ora configuriamolo. Vai a **Dettagli** campo ****.

   ![](assets/image2014-9-15-12-3a31-3a55.png)
Trascinate tutti i campi che fanno parte del set di profili progressivo.
   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Dopo aver spostato tutti i campi, dovrebbe avere l&#39;aspetto seguente:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >I campi all’esterno della casella **Profilamento progressivo** **** vengono sempre visualizzati nel modulo, anche se sono compilati.

1. Selezionate la casella **Profilamento progressivo** **** .

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Prestate attenzione quando utilizzate i campi obbligatori in Profiling progressivo. Questi campi potrebbero comunque essere lasciati vuoti se il visitatore immette un nuovo indirizzo e-mail (che creerebbe una nuova persona) dopo l&#39;invio in precedenza dei dati per gli altri campi, in quanto sarebbero stati eliminati nel modulo più recente.

1. Ora scegliete quanti campi vuoti desiderate vengano visualizzati dalla casella **Progressi** **Profili** in qualsiasi momento.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >**Esempio**
   >
   >
   >Se scegliete **Numero** **di** **campi** vuoti **** come 1, il visitatore vedrà quanto segue al primo accesso al modulo:
   >
   >    
   >    
   >    * Nome (vuoto)
   >    * Cognome (vuoto)
   >    * Indirizzo e-mail (vuoto)
   >    * Numero di telefono (vuoto)

   >    
   >    
   >Presupponendo che compilino ogni campo, la seconda volta che visitano, vedranno:
   >
   >    
   >    
   >    * Nome (precompilato)
   >    * Cognome (precompilato)
   >    * Indirizzo e-mail (precompilato)
   >    * Numero di telefono cellulare (vuoto)

   >    
   >    
   >Presupponendo che compilino il numero di telefono cellulare, la terza volta che visita vedranno:
   >
   >    
   >    
   >    * Nome (precompilato)
   >    * Cognome (precompilato)
   >    * Indirizzo e-mail (precompilato)
   >    * Paese (vuoto)


1. Fare clic su **Fine**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Fate clic su **Approva e chiudi**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Bel lavoro! Il lavoro che hai appena fatto ripagherà.

Provate con questa funzione e accertatevi di eseguire il test. È avanzata, ma è possibile rendere i moduli molto dinamici in questo modo.
