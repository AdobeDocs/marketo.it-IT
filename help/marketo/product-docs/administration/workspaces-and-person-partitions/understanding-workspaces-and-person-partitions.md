---
unique-page-id: 2360309
description: Aree di lavoro e partizioni di persone - Documenti Marketo - Documentazione prodotto
title: Informazioni su aree di lavoro e partizioni di persone
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# Aree di lavoro e partizioni di persone {#understanding-workspaces-and-person-partitions}

## Aree di lavoro {#workspaces}

>[!CAUTION]
>
>Le aree di lavoro possono essere complesse da configurare.  Contattate il supporto [Marketo](http://support.marketo.com/) per sapere se è adatto a voi.

Le aree di lavoro sono aree separate in Marketo che contengono risorse di marketing come programmi, pagine di destinazione, e-mail e altro ancora. Possono essere utilizzati da più persone. Ogni utente ha accesso a una o più aree di lavoro.

>[!NOTE]
>
>**Esempio**
>
>Per alcuni motivi è possibile utilizzare un’area di lavoro:
>
>* Geografia: I reparti marketing Europa, Asia e America del Nord ottengono uno spazio di lavoro
>* Unità aziendale: Quickbook, Quickbook e TurboTax ottengono ciascuno un&#39;area di lavoro

>
>
In ogni caso, la separazione è dovuta al fatto che le risorse di marketing sono completamente diverse. Se condividono risorse di marketing, le aree di lavoro potrebbero non essere lo strumento adatto alle vostre esigenze.

>[!NOTE]
>
>**Tubo profondo**
>
>Scoprite come creare [una nuova area di lavoro](create-a-new-workspace.md).

## Condivisione tra aree di lavoro {#sharing-across-workspaces}

Di seguito viene illustrato come condividere risorse tra diverse aree di lavoro. Funziona allo stesso modo per qualsiasi cosa si desideri condividere; questo esempio mostra le segmentazioni.

>[!NOTE]
>
>La cartella principale contenente le risorse è l’unica cartella che può essere condivisa, non le cartelle figlie.

1. Create una nuova cartella.

   ![](assets/one.png)

1. Denominate la cartella da condividere.

   ![](assets/two.png)

1. Spostate le risorse da condividere nella cartella.

   ![](assets/three.png)

1. Fare clic con il pulsante destro del mouse sulla cartella e selezionare **Condividi cartella**.

   ![](assets/four.png)

1. Selezionate le aree di lavoro con cui desiderate condividere la cartella e fate clic su **Salva**. Nella finestra di dialogo Condividi cartella vengono visualizzate solo le aree di lavoro autorizzate.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >La cartella di origine ora avrà una freccia verde che indica che è stata condivisa. Nell’area di lavoro condivisa, la cartella avrà un lucchetto che indica la sola lettura.

Potete condividere questi elementi tra le diverse aree di lavoro.

* Modelli e-mail
* Modelli per pagine di destinazione
* Modelli
* Campagne intelligenti
* [Elenchi avanzati](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmenti](share-segmentations-across-workspaces-and-partitions.md)
* Snippet

## Clonazione tra aree di lavoro {#cloning-across-workspaces}

Per le risorse che non sono modelli, è consigliabile duplicarle come risorse locali all’interno di un programma.  Con il livello di accesso appropriato, potete trascinare queste risorse in un’altra area di lavoro:

* Programmi
* E-mail
* Pagine di destinazione
* Forms

>[!NOTE]
>
>Quando clonate risorse con modelli, questi modelli devono essere condivisi con l’area di lavoro di destinazione.

## Spostamento delle risorse in altre aree di lavoro {#moving-assets-to-other-workspaces}

Per spostare le risorse in una nuova area di lavoro, inseritele in una cartella e trascinatele sull’altra.

>[!NOTE]
>
>Non è possibile spostare un programma che contiene membri da un&#39;area di lavoro all&#39;altra.

## Partizioni di persona {#person-partitions}

Le partizioni delle persone si comportano come database separati. Ogni partizione ha le proprie persone che non disaccoppiano o si mescolano con altre partizioni. Se ritieni di avere un caso d&#39;uso aziendale che potrebbe richiedere la presenza di record duplicati con lo stesso indirizzo e-mail, contatta il [Supporto marketing](http://support.marketo.com).

È possibile assegnare partizioni di persona a [aree di lavoro](create-a-new-workspace.md) nelle seguenti configurazioni:

* un&#39;area di lavoro a una partizione personale (1:1)
* un&#39;area di lavoro a più partizioni (1:x)
* molte aree di lavoro a una partizione personale (x:1)

>[!NOTE]
>
>**Esempio**
>
>Motivi per cui si utilizzerebbe una partizione personale:
>
>* Le aree di lavoro non solo dispongono di risorse diverse, ma non condividono persone
>* Desideri duplicare per altri motivi aziendali

>



>[!CAUTION]
>
>Le partizioni di persona non interagiscono tra loro, quindi prestate attenzione quando le configurate.

>[!NOTE]
>
>**Tubo profondo**
>
> Scopri come [creare una partizione per persona](create-a-person-partition.md).

