---
unique-page-id: 10099077
description: Power Pack di recapito messaggi e-mail - Come importare una lista di distribuzione - Marketo Docs - Documentazione del prodotto
title: Power Pack di recapito messaggi e-mail - Come importare un elenco di messaggi
exl-id: a4782611-2556-43bf-802b-afeb332eafcd
source-git-commit: 4448d6e082c0c4fad35fc2980446175bffe47e4b
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Power Pack di recapito messaggi e-mail: Come importare un elenco di sementi {#email-deliverability-power-pack-how-to-import-a-seedlist}

Un elenco di seed è un elenco di account e-mail in più provider di cassette postali, tra cui Google Apps, Hotmail, Yahoo!, ecc, che vengono utilizzati per approssimare il tasso di consegna della cartella Posta in arrivo rispetto a quella della cartella spam. Ecco come ottenere quell’elenco nella tua istanza di Marketo.

>[!AVAILABILITY]
>
>Non tutti i clienti hanno acquistato questa funzionalità. Per ulteriori informazioni, contattare il rappresentante commerciale.

## Importare un elenco di sementi {#import-a-seedlist}

1. In My Marketo, seleziona **Strumenti di consegna**.

   ![](assets/email-deliverability-power-pack-1.png)

1. Fai clic su **Inviatore casella in entrata**.

   ![](assets/two-1.png)

1. Fai clic su **Get Seedlist**.

   ![](assets/three-1.png)

1. Fai clic su **Esporta elenco**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Scegli **Elenco di ottimizzazione** se si desidera 250ok [ottimizzare l&#39;elenco](https://help.returnpath.com/hc/en-us/articles/360046746451-What-is-250ok-s-seedlist-optimizer-and-why-should-I-use-it-) per te. Scegli **Personalizza elenco** se si desidera selezionare le aree dell’elenco di siti da includere.

1. Dopo l’esportazione, l’elenco verrà visualizzato come file .txt nella cartella dei download del browser. Recuperarlo e [importare](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md) nella tua istanza Marketo come elenco statico.

   ![](assets/five.png)

   >[!TIP]
   >
   >Assicurati di assegnare un nome alla tua lista in modo da renderla facile da trovare.

   >[!CAUTION]
   >
   >Puoi ottenere una quantità limitata di queste campagne informative Posta in arrivo al mese. Per vedere quanti ne ottieni, guarda nel tuo 250ok **Impostazioni account**. Per ottenere di più, contatta il tuo rappresentante commerciale Marketo.

## Acquisizione di nuovi elenchi di siti {#acquiring-new-seedlists}

La tua lista dei semi può cambiare spesso come ogni mese. È importante accedere regolarmente a Email Deliverability Power Pack e controllare lo stato dell’elenco di seed. Quando vengono aggiunti nuovi indirizzi o è necessario un aggiornamento, viene visualizzato un avviso tramite l’interfaccia nella pagina Get Seedlist .

Dopo aver creato l’elenco statico in Marketo, puoi iniziare a inviarlo per testare il posizionamento della casella in entrata dell’e-mail.
