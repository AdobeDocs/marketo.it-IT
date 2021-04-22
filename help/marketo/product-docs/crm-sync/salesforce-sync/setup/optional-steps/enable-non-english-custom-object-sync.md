---
unique-page-id: 4719302
description: Abilita sincronizzazione di oggetti personalizzati non inglesi - Documenti Marketo - Documentazione del prodotto
title: Abilita sincronizzazione oggetti personalizzata non inglese
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Abilita sincronizzazione oggetti personalizzata non inglese {#enable-non-english-custom-object-sync}

Se l&#39;utente di sincronizzazione Marketo è impostato su una lingua diversa dall&#39;inglese, si può verificare un errore durante il tentativo di abilitare una sincronizzazione oggetto personalizzata.

## Errore {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Come aggirare il problema {#getting-around-it}

1. Accedi a Salesforce utilizzando il markto per sincronizzare l’utente.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Sotto il nome utente, vai a **Configurazione**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. In **Informazioni personali**, fai clic su **Informazioni personali**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Fare clic su **Modifica**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Cambia la **Lingua** in **Inglese**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Fare clic su **Salva**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. In Marketo, in **Amministratore > Salesforce > Oggetti** fai clic su **Aggiorna schema**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Questo estrae l’elenco degli oggetti in inglese. Ora seleziona l&#39;oggetto desiderato e fai clic su **Abilita sincronizzazione**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Osserva che l’oggetto personalizzato è ora abilitato e sincronizzato.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Ora torna a Salesforce e utilizza i passaggi precedenti per ripristinare l’utente della sincronizzazione nella lingua preferita.

>[!NOTE]
>
>Non dimenticare di aggiornare lo schema un&#39;ultima volta per richiamare gli oggetti nella tua lingua.
