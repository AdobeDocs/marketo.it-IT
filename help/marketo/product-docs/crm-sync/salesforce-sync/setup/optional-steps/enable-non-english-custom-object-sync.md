---
unique-page-id: 4719302
description: Attiva sincronizzazione oggetti personalizzati non inglesi - Documenti Marketo - Documentazione prodotto
title: Attiva sincronizzazione oggetti personalizzata non in lingua inglese
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Abilita sincronizzazione oggetti personalizzata non inglese {#enable-non-english-custom-object-sync}

Se l&#39;utente di sincronizzazione Marketo è impostato su una lingua diversa dall&#39;inglese, è possibile che si verifichi un errore durante il tentativo di abilitare una sincronizzazione oggetto personalizzata.

## Errore {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Come aggirare {#getting-around-it}

1. Accedi a Salesforce utilizzando il markper sincronizzare l&#39;utente.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Sotto il nome utente, andate a **Setup**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. In **Informazioni personali**, fare clic su **Dati personali**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Fare clic su **Modifica**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Modificare la **lingua** in **inglese**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Fare clic su **Salva**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. Indietro in Marketo, in **Amministratore > Salesforce > Objects** fare clic su **Aggiorna schema**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Questo esegue il pull dell&#39;elenco degli oggetti in inglese. Selezionare l&#39;oggetto desiderato e fare clic su **Abilita sincronizzazione**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Notate che l&#39;oggetto personalizzato è ora abilitato e sincronizzato.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Ora torna a Salesforce e utilizza i passaggi precedenti per ripristinare l&#39;utente della sincronizzazione nella lingua desiderata.

>[!NOTE]
>
>**Promemoria**
>
>Non dimenticare di aggiornare lo schema un&#39;ultima volta per richiamare gli oggetti nella lingua.

