---
description: Criteri di pubblico - Documentazione di Marketo - Documentazione del prodotto
title: Criteri di audience
feature: Dynamic Chat
exl-id: 95c4558e-0c0c-4623-bb7d-b6ac2f455c01
source-git-commit: f5f93a993d5b13c1fda0b31172393eff0bc65fd4
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 1%

---

# Criteri di audience {#audience-criteria}

Analogamente agli elenchi avanzati dei Marketi Engage, gli attributi dei criteri di pubblico consentono di definire il pubblico di destinazione. Puoi eseguire il targeting di persone note o sconosciute utilizzando gli attributi dedotti, persona o azienda (o una combinazione di questi).

## Priorità {#priority}

La priorità determina quale finestra di dialogo riceve un lead nel caso in cui sia idoneo per più di una. Viene stabilito quando si inizia [creare la finestra di dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}. Per modificare la priorità di una finestra di dialogo esistente, aprila e vai a **[!UICONTROL Dettagli finestra di dialogo]** nella scheda Criteri del pubblico.

![](assets/audience-criteria-1.png)

## Eventi {#events}

Gli eventi consentono di indirizzare i visitatori in base al numero di scorrimento o alla durata della loro presenza sulla pagina/sito. Nell’esempio seguente, eseguiamo il targeting dei visitatori che si trovano su una pagina specifica da più di 20 secondi.

1. Acquisisci **[!UICONTROL Tempo sulla pagina]** e trascinarlo a destra.

   ![](assets/audience-criteria-3.png)

1. Impostare il tempo &quot;Maggiore di&quot; su 20 secondi.

   ![](assets/audience-criteria-4.png)

1. Aggiungi l’URL della pagina desiderata in [Target](#target) sezione.

   ![](assets/audience-criteria-5.png)

## Attributi {#attributes}

**Persone note**

Ci sono _molti_ combinazioni di attributi tra cui scegliere. Nell’esempio seguente, il targeting riguarda tutte le persone note in California che lavorano in un’azienda con più di 50 dipendenti.

1. Acquisisci **[!UICONTROL Stato della persona]** e trascinarlo verso destra.

   ![](assets/audience-criteria-7.png)

1. _È_ è impostato per impostazione predefinita. Nel campo Seleziona valori, digita in CA (puoi anche fare clic sull’elenco a discesa e selezionare dall’elenco).

   ![](assets/audience-criteria-8.png)

1. Acquisisci **[!UICONTROL Dimensioni società]** e trascinarlo nel punto in cui è indicato _trascina e rilascia qui un attributo_.

   ![](assets/audience-criteria-9.png)

   >[!NOTE]
   >
   >È inoltre possibile scegliere un attributo facendo clic sul relativo **+** icona.

1. Fai clic sul menu a discesa operatore e seleziona **[!UICONTROL Maggiore di]**.

   ![](assets/audience-criteria-10.png)

1. Digitare 50 e fare clic in un altro punto dello schermo per salvare.

   ![](assets/audience-criteria-11.png)

Ed è tutto!

**Persone anonime**

Esiste un modo semplice per eseguire il targeting specifico delle persone che non sono ancora presenti nel database. In questo esempio, il targeting riguarda tutte le persone anonime che si trovano nell&#39;area di New York.

1. Acquisisci **[!UICONTROL E-mail della persona]** e trascinarlo verso destra.

   ![](assets/audience-criteria-12.png)

1. Fai clic sul menu a discesa operatore e seleziona **[!UICONTROL È vuoto]**.

   ![](assets/audience-criteria-13.png)

1. Acquisisci **[!UICONTROL Stato dedotto]** e trascinarlo nel punto in cui è indicato _trascina e rilascia qui un attributo_.

   ![](assets/audience-criteria-14.png)

   >[!NOTE]
   >
   >Quando qualcuno visita il tuo sito web, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} li cookie e li inserisce nel sistema. Cerchiamo il loro IP in un database speciale e deduciamo tutti i tipi di buone informazioni.

1. _È_ è impostato per impostazione predefinita. Nel campo Seleziona valori, digita in NY (puoi anche fare clic sull’elenco a discesa e selezionare dall’elenco).

   ![](assets/audience-criteria-15.png)

## Iscrizione {#membership}

Utilizza gli elenchi avanzati di Marketo Engage per il pubblico di destinazione della finestra di dialogo.

>[!AVAILABILITY]
>
>Il membro di un elenco avanzato o il criterio del membro di un elenco richiede Dynamic Chat Prime. Per ulteriori informazioni, contatta l’Adobe Account Team (il tuo Account Manager).

1. In Iscrizione, accedi **[!UICONTROL Membro di elenco avanzato]** e lo rilasci sull&#39;area di lavoro.

   ![](assets/audience-criteria-15a.png)

1. Selezionare l&#39;elenco avanzato desiderato.

   ![](assets/audience-criteria-15b.png)

## Aggiungi gruppi {#add-groups}

Puoi anche raggruppare gli attributi, se desideri che siano tutti determinati attributi insieme a &quot;tutti o uno qualsiasi&quot; di altri. Puoi aggiungere più gruppi.

![](assets/audience-criteria-16.png)

![](assets/audience-criteria-17.png)

## Target {#target}

Immettere gli URL in cui si desidera visualizzare una finestra di dialogo specifica. Puoi anche aggiungere esclusioni.

Formati accettabili:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>L&#39;utilizzo di un asterisco funge da carattere jolly catch-all. Quindi `https://*.website.com` inserirebbe la finestra di dialogo in ogni pagina del sito, inclusi i sottodomini (ad esempio: `support.website.com`). E `https://website.com/folder/*` inserirebbe la finestra di dialogo in ogni pagina HTML nella cartella successiva (ad esempio, in questo caso diciamo che la cartella è &quot;sport&quot;, quindi: website.com/sports/baseball.html, website.com/sports/football.html, ecc.).

**Esclusioni**

Utilizza le esclusioni per assicurarti che la finestra di dialogo _non_ in una pagina o area specifica del sito. Le esclusioni seguono lo stesso formato delle inclusioni.

![](assets/audience-criteria-18.png)

>[!MORELIKETHIS]
>
>* [Creare una finestra di dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-dialogue.md){target="_blank"}
>* [Progettazione flussi](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}
