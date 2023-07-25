---
unique-page-id: 4719302
description: Abilita sincronizzazione oggetti personalizzati non in inglese - Documentazione di Marketo - Documentazione del prodotto
title: Abilita sincronizzazione oggetti personalizzati non inglese
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Abilita sincronizzazione oggetti personalizzati non inglese {#enable-non-english-custom-object-sync}

Se l&#39;utente di Marketo Sync è impostato su una lingua diversa dall&#39;inglese, è possibile che si verifichi un errore quando si tenta di abilitare una sincronizzazione oggetto personalizzata.

## L&#39;errore {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Come aggirare il problema {#getting-around-it}

1. Accedi a Salesforce utilizzando l’utente marketo sync.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Sotto il nome utente, vai a **Configurazione**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Sotto **Informazioni personali**, fai clic su **Informazioni personali**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Clic **Modifica**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Modificare il **Lingua** a **Inglese**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Clic **Salva**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. Torna a Marketo, sotto **Admin (Amministrazione) > Salesforce > Objects (Oggetti)** click **Aggiorna schema**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. L&#39;elenco degli oggetti verrà richiamato in inglese. Selezionare l&#39;oggetto desiderato e fare clic su **Abilita sincronizzazione**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Osserva che l’oggetto personalizzato è ora abilitato e sincronizzato.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Ora torna a Salesforce e utilizza i passaggi precedenti per ripristinare la lingua preferita dell’utente di sincronizzazione.

>[!NOTE]
>
>Non dimenticare di aggiornare lo schema un&#39;ultima volta per richiamare gli oggetti nella lingua.
