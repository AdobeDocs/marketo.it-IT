---
unique-page-id: 11385579
description: Creare modelli di contenuto - Documenti Marketo - Documentazione del prodotto
title: Creare modelli di contenuto
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Creare modelli di contenuto {#create-content-patterns}

Quando si impostano i pattern di contenuto, il contenuto viene rilevato automaticamente quando un visitatore web fa clic sulla pagina web di HTML relativa al pattern di contenuto. Viene utilizzato per aggiungere pagine di HTML (post di blog, comunicati stampa, articoli di news) come elementi di contenuto alla pagina Tutti i contenuti. Quando la ricerca automatica si basa su pattern di contenuto, rileva e traccia le pagine di HTML correlate al pattern URL definito quando un visitatore web visualizza o fa clic su un collegamento alla pagina. Questo contenuto (l’URL, il nome della pagina e i metadati, incluso l’URL e la descrizione dell’immagine) viene aggiunto alla pagina Tutto il contenuto per preparare il contenuto predittivo. Per la ricerca automatica di altri contenuti, come PDF e video incorporati, è necessario [abilita ricerca contenuti](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. Vai a **Impostazioni contenuto**.

   ![](assets/settings-dropdown-hand-2.png)

1. Fai clic su **Pattern di URL**.

   ![](assets/click-url-patterns-hand.png)

1. Fai clic sul pulsante **+** per aprire una riga in cui inserire le informazioni.

   ![](assets/content-settings-create-patterns-hand.png)

1. Aggiungi l’estensione URL del dominio in cui esiste la pagina web. Selezionare la categoria (ad esempio Blog, Articolo, Data Sheet, Press Release).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Gli elementi dell&#39;elenco a discesa a destra riflettono le categorie impostate quando si [categorie create](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. Fai clic su **+** per aggiungere un altro percorso.

   ![](assets/url-patterns-add2.png)

1. Aggiungi l’estensione e la categoria per il percorso aggiuntivo e fai clic su **Salva**.

   ![](assets/url-patterns-save.png)

## Regole del pattern di contenuto {#content-pattern-rules}

* È possibile utilizzare un carattere jolly in qualsiasi punto di un&#39;espressione (esempio: _domain.com/&#42;_, _domain.com/&#42;blog&#42;_)

* Si consiglia di utilizzare /&#42; alla fine di un&#39;espressione per continuare l&#39;individuazione dei pattern (Esempio: _domain.com/blog/&#42;_ rileva tutti i post nella cartella Blog)
* I pattern di contenuto non sono sensibili all’uso di maiuscole e minuscole (Esempio: _domain.com/Blog/&#42;_ rileva tutte le pagine HTML in _domain.com/Blog_ e _domain.com/blog_)

* I parametri URL non vengono rilevati (in questo modo si evita di individuare più elementi con lo stesso URL di contenuto ma diversi parametri)

## Esempi {#examples}

Per _domain.com_:

<table> 
 <tbody> 
  <tr> 
   <th>Pattern URL</th> 
   <th>Risultato</th> 
  </tr> 
  <tr> 
   <td>blog/*</td> 
   <td><p>Rileva tutto il contenuto che corrisponde al pattern domain.com/blog/:</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>articolo/2017/*</td> 
   <td><p>Rileva tutto il contenuto che corrisponde al pattern domain.com/article/2017/:</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td> 
   <td><p>Rileva qualsiasi URL contenente la parola "set di dati:"</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>comunicato stampa</td> 
   <td><p>Viene individuata una sola pagina HTML corrispondente esatta:</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>Se l’espressione URL è vuota, il pattern URL rileva solo la home page:</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
