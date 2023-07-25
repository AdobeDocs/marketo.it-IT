---
unique-page-id: 11385579
description: Creare modelli di contenuto - Documenti Marketo - Documentazione del prodotto
title: Creare modelli di contenuto
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Creare modelli di contenuto {#create-content-patterns}

Quando imposti i pattern di contenuto, il contenuto viene individuato automaticamente quando un visitatore web fa clic sulla pagina web di HTML pertinente al pattern di contenuto. Viene utilizzato per aggiungere pagine HTML (post di blog, comunicati stampa, articoli di notizie) come parti di contenuto alla pagina Tutti i contenuti. Quando l’individuazione automatica si basa sui pattern di contenuto, rileva e tiene traccia delle pagine HTML correlate al pattern URL definito quando un visitatore web visualizza o fa clic su un collegamento alla pagina. Questo elemento di contenuto (l’URL, il nome della pagina e i metadati, inclusi l’URL e la descrizione dell’immagine) viene aggiunto alla pagina Tutto il contenuto per preparare contenuti predittivi. Per la ricerca automatica di altri contenuti, ad esempio PDF e video incorporati, è necessario [abilitare l’individuazione dei contenuti](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. Vai a **Impostazioni contenuto**.

   ![](assets/settings-dropdown-hand-2.png)

1. Clic **Pattern di URL**.

   ![](assets/click-url-patterns-hand.png)

1. Fai clic su **+** per aprire una riga in cui è possibile inserire le informazioni.

   ![](assets/content-settings-create-patterns-hand.png)

1. Aggiungi l’estensione URL del dominio in cui esiste la pagina web. Seleziona la categoria (ad esempio Blog, Articolo, Foglio dati, Comunicato stampa).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Gli elementi nell&#39;elenco a discesa a destra riflettono le categorie impostate quando [categorie create](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. Clic **+** per aggiungere un altro percorso.

   ![](assets/url-patterns-add2.png)

1. Aggiungi l’estensione e la categoria per il percorso aggiuntivo e fai clic su **Salva**.

   ![](assets/url-patterns-save.png)

## Regole per pattern di contenuto {#content-pattern-rules}

* È possibile utilizzare un carattere jolly in qualsiasi punto di un&#39;espressione (ad esempio: _domain.com/&#42;_, _domain.com/&#42;blog&#42;_)

* È consigliabile utilizzare /&#42; alla fine di un&#39;espressione per continuare l&#39;individuazione del pattern (esempio: _domain.com/blog/&#42;_ individua tutti i post nella cartella Blog)
* I modelli di contenuto non distinguono tra maiuscole e minuscole (esempio: _domain.com/Blog/&#42;_ rileva tutte le pagine html in _domain.com/Blog_ e _domain.com/blog_)

* I parametri URL non vengono rilevati (questo evita di individuare più elementi con lo stesso URL di contenuto ma diversi parametri)

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
   <td><p>Rileva qualsiasi URL contenente la parola "datasheets:"</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>comunicato stampa</td> 
   <td><p>Viene individuata una sola pagina HTML corrispondente:</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>Se l’espressione URL è vuota, il modello URL rileva solo la home page:</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
