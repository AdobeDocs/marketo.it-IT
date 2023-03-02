---
unique-page-id: 2360309
description: Aree di lavoro e partizioni delle persone - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulle aree di lavoro e sulle partizioni delle persone
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
source-git-commit: 57b94e643154b1463d9fd65295a66f1a3286fd40
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Informazioni sulle aree di lavoro e sulle partizioni delle persone {#understanding-workspaces-and-person-partitions}

## Aree di lavoro {#workspaces}

>[!CAUTION]
>
>L’impostazione delle aree di lavoro può essere complessa. Contatto [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) per scoprire se sono giusti per te.

Le aree di lavoro sono aree separate in Marketo che contengono risorse di marketing come programmi, pagine di destinazione, e-mail e altro ancora. Possono essere utilizzati da più persone. Ogni utente ha accesso a una o più aree di lavoro.

>[!NOTE]
>
>**Esempio**
>
>Alcuni motivi per cui potresti utilizzare un’area di lavoro:
>
>* Geografia: i reparti marketing di Europa, Asia e Nord America dispongono ognuno di un’area di lavoro
>* Business Unit: Quicken, Quickbook e TurboTax ottengono ognuno un’area di lavoro
>
>In ogni caso, la separazione è dovuta al fatto che le risorse di marketing sono completamente diverse. Se condividono risorse di marketing, le aree di lavoro potrebbero non essere lo strumento giusto per te.

>[!NOTE]
>
>Scopri come creare [crea una nuova area di lavoro](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Condivisione tra aree di lavoro {#sharing-across-workspaces}

Ecco come condividere le risorse tra le aree di lavoro. Funziona allo stesso modo per qualsiasi elemento che desideri condividere; questo esempio mostra le segmentazioni.

>[!NOTE]
>
>La cartella principale contenente le risorse è l’unica cartella che può essere condivisa, non le cartelle secondarie.

1. Scegliere Database.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. Fai clic con il pulsante destro del mouse sulla cartella Segmentazione e fai clic su **Nuova cartella**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. Denomina la cartella e fai clic su **Crea**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. Sposta le risorse da condividere nella cartella.

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. Fare clic con il pulsante destro del mouse sulla cartella e selezionare **Condividi cartella**.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. Seleziona i workspace con cui vuoi condividere la cartella e fai clic su **Salva**. Nella finestra di dialogo Condividi cartella verranno visualizzate solo le aree di lavoro per le quali si dispone dell&#39;autorizzazione di visualizzazione.

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >La cartella di origine presenta ora una piccola freccia verde che indica che è stata condivisa. Nell’area di lavoro condivisa, la cartella avrà un lucchetto che indica la sola lettura.

È possibile condividere questi elementi tra aree di lavoro diverse.

* Modelli e-mail
* Modelli di pagina di destinazione
* Modelli
* Campagne intelligenti
* [Elenchi avanzati](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentazioni](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Snippet

## Clonazione in più aree di lavoro {#cloning-across-workspaces}

Per le risorse che non sono modelli, è consigliabile clonarle come risorse locali all’interno di un programma.  Con il livello di accesso appropriato, puoi trascinare queste risorse in un’altra area di lavoro:

* Programmi
* E-mail
* Pagine di destinazione
* Forms

>[!NOTE]
>
>Quando si clonano risorse con modelli, questi devono essere condivisi con l’area di lavoro di destinazione.

## Spostamento delle risorse in altre aree di lavoro {#moving-assets-to-other-workspaces}

Per spostare le risorse in una nuova area di lavoro, inseriscile in una cartella e trascina la cartella nell’altra area di lavoro.

>[!NOTE]
>
>Non è possibile spostare un programma che contiene membri da un&#39;area di lavoro a un&#39;altra.

## Partizioni della persona {#person-partitions}

Le partizioni delle persone si comportano come database separati. Ogni partizione ha le proprie persone che non si deduplicano o si mescolano con altre partizioni. Se ritieni di avere un caso d’uso aziendale che potrebbe richiedere la duplicazione dei documenti con lo stesso indirizzo e-mail, contatta [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

È possibile assegnare le partizioni persona a  [workspace](create-a-new-workspace.md) nelle seguenti configurazioni:

* partizione da un&#39;area di lavoro a una persona (1:1)
* da un&#39;area di lavoro a più partizioni persona (1:x)
* molte aree di lavoro in una partizione persona (x:1)

>[!NOTE]
>
>Motivi per cui si utilizza una partizione persona:
>
>* Le aree di lavoro non dispongono solo di risorse diverse, ma non condividono nemmeno altre persone
>* Si desiderano duplicati per altri motivi aziendali


>[!CAUTION]
>
>Le partizioni della persona non interagiscono tra loro, quindi fai attenzione quando le configuri.

>[!NOTE]
>
>Scopri come [creare una partizione persona](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
