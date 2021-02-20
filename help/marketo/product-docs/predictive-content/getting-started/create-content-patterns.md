---
unique-page-id: 11385579
description: Creazione di modelli di contenuto - Documenti Marketo - Documentazione del prodotto
title: Creare pattern di contenuto
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---


# Creare pattern di contenuto {#create-content-patterns}

Quando impostate i pattern di contenuto, il contenuto viene rilevato automaticamente quando un visitatore Web fa clic sulla pagina Web HTML relativa al pattern di contenuto. Viene utilizzato per aggiungere alla pagina Tutti i contenuti delle pagine HTML (post di blog, comunicati stampa, articoli di notizie). Quando la funzione di individuazione automatica è basata su pattern di contenuto, rileva e tiene traccia delle pagine HTML correlate al pattern URL definito quando un visitatore Web visualizza o fa clic su un collegamento alla pagina. Questo contenuto (l’URL, il nome della pagina e i metadati, inclusi l’URL e la descrizione dell’immagine) viene aggiunto alla pagina Tutto il contenuto per preparare il contenuto predittivo. Per scoprire automaticamente altri contenuti, come PDF e video incorporato, è necessario [abilitare l&#39;individuazione del contenuto](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. Vai a **Impostazioni contenuto**.

   ![](assets/settings-dropdown-hand-2.png)

1. Fare clic su **Pattern URL**.

   ![](assets/click-url-patterns-hand.png)

1. Fare clic su **+** per aprire una riga in cui inserire le informazioni.

   ![](assets/content-settings-create-patterns-hand.png)

1. Aggiungete l’estensione URL del dominio in cui esiste la pagina Web. Selezionate la categoria (ad esempio Blog, Articolo, Data Sheet, Press Release).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Gli elementi nell&#39;elenco a discesa sulla destra riflettono le categorie configurate al momento della creazione di [categorie](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. Fare clic su **+** per aggiungere un altro percorso.

   ![](assets/url-patterns-add2.png)

1. Aggiungete l&#39;estensione e la categoria del percorso aggiuntivo e fate clic su **Salva**.

   ![](assets/url-patterns-save.png)

## Regole pattern contenuto {#content-pattern-rules}

* È possibile utilizzare un carattere jolly ovunque in un&#39;espressione (esempio: _domain.com/*_, _domain.com/*blog*_)

* È consigliabile utilizzare /* alla fine di un&#39;espressione per continuare l&#39;individuazione dei pattern (esempio: _domain.com/blog/*_ rileva tutti i post presenti nella cartella Blog)
* I pattern di contenuto non fanno distinzione tra maiuscole e minuscole (esempio: _domain.com/Blog/*_ rileva tutte le pagine HTML in _domain.com/Blog_ e _domain.com/blog_

* I parametri URL non vengono rilevati (in questo modo si evitano di rilevare più elementi con lo stesso URL di contenuto ma con parametri diversi)

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
   <td>article/2017/*</td> 
   <td><p>Rileva tutto il contenuto che corrisponde al pattern domain.com/article/2017/:</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="—"></td> 
   <td><p>Consente di individuare eventuali URL contenenti la parola "dataset heets:"</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>comunicato stampa</td> 
   <td><p>Viene rilevata una sola pagina HTML corrispondente:</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>Se l’espressione URL è vuota, il pattern URL rileva solo la pagina principale:</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
