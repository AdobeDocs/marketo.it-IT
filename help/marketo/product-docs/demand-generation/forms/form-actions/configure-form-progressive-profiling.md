---
unique-page-id: 2359646
description: Configurare la profilazione progressiva dei moduli - Documenti Marketo - Documentazione del prodotto
title: Configurare il profiling progressivo del modulo
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Configurare il profiling progressivo del modulo {#configure-form-progressive-profiling}

Le forme corte sono buone! Quando un utente torna a un modulo, puoi presentare nuovi campi e compilare progressivamente il profilo del visitatore. Ecco come.

>[!NOTE]
>
>Affinché questa funzione funzioni correttamente, assicurati che la funzione di precompilazione del modulo sia abilitata per i campi visibili e [disattivato](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) per i campi nascosti.

1. Vai a **Attività di marketing**.

   ![](assets/ma-1.png)

1. Seleziona il modulo e fai clic su **Modifica modulo**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. Sotto **Impostazioni modulo**, fai clic su **Impostazioni**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Imposta **Profilazione progressiva** a **Abilitato**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Ok, ora configuriamola. Vai a **Dettagli campo**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Trascina e rilascia tutti i campi che fanno parte del set di profili progressivi.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Dopo aver spostato tutti i campi, dovrebbe avere un aspetto simile al seguente:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >I campi al di fuori dei **Profilazione progressiva** viene sempre visualizzata nel modulo, anche se è compilato.

1. Seleziona la **Profilazione progressiva** scatola.

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Presta attenzione quando utilizzi i campi obbligatori in Profilazione progressiva. Questi campi potrebbero comunque restare vuoti se il visitatore immette un nuovo indirizzo e-mail (che creerebbe una nuova persona) dopo l’invio in precedenza dei dati per gli altri campi, in quanto verrebbero soppressi nel modulo più recente.

1. Ora scegli quanti campi vuoti desideri che le persone visualizzino dal **Profilazione progressiva** in qualsiasi momento.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Se scegli **Numero** **di** **Vuoto** **Campi** con 1, il visitatore visualizzerà per la prima volta questo modulo:
   >
   >* Nome (vuoto)
   >* Cognome (vuoto)
   >* Indirizzo e-mail (vuoto)
   >* Numero di telefono (vuoto)

   >
   >Presupponendo che compilino ogni campo, la seconda volta che visitano, vedranno:
   >
   >* Nome (precompilato)
   >* Cognome (precompilato)
   >* Indirizzo e-mail (precompilato)
   >* Numero di telefono cellulare (vuoto)

   >
   >Presupponendo che compilino il numero di telefono cellulare, la terza volta che visitano vedranno:
   >
   >* Nome (precompilato)
   >* Cognome (precompilato)
   >* Indirizzo e-mail (precompilato)
   >* Paese (vuoto)


1. Fai clic su **Fine**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Fai clic su **Approva e chiudi**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Bel lavoro! Il lavoro che hai appena fatto ripagherà.

Sperimenta questa funzione e assicurati di testarla. È avanzato, ma in questo modo è possibile rendere i moduli molto dinamici.
