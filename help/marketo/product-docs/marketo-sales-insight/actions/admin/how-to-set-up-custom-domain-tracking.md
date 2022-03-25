---
description: Come impostare il tracciamento del dominio personalizzato - Documenti Marketo - Documentazione del prodotto
title: Come impostare il tracciamento del dominio personalizzato
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Come impostare il tracciamento del dominio personalizzato {#how-to-set-up-custom-domain-tracking}

Il tracciamento del dominio personalizzato consente al tuo team di utilizzare il nome della tua azienda in tutti i collegamenti tracciabili aggiunti alle e-mail di vendita. Una volta configurato questo, inserire nell&#39;elenco Consentiti tutti i collegamenti presenti nell&#39;e-mail che compariranno come go.yourcompany.com, in modo che quando qualcuno passa il mouse su un collegamento, legga go.yourcompany.com invece di go.toutapp.com.

Per impostare un record CNAME per il dominio che punta a go.toutapp.com, ti servirà l&#39;assistenza del team IT. Questo CNAME sarà ciò che verrà visualizzato su tutti i tuoi collegamenti di tracciamento (ad esempio, go.yourcompany.com).

Dopo aver confermato con il team IT che il CNAME è configurato correttamente, puoi aggiungerlo alla pagina Monitoraggio dominio personalizzato in Azioni.

>[!NOTE]
>
>Se il CNAME non è configurato correttamente e lo attivi come dominio personalizzato in Azioni, può interrompere i collegamenti di tracciamento e i pixel.

## Abilita tracciamento dominio personalizzato {#enable-custom-domain-tracking}

>[!NOTE]
>
>**Sono richiesti i privilegi di amministratore.**

1. Fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. In Impostazioni amministratore, seleziona **Tracking**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. Nella scheda Custom Domain Tracking , immetti il tuo CNAME e fai clic su **Connetti**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
