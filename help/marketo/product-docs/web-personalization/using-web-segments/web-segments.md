---
unique-page-id: 4719093
description: Segmenti Web - Documenti Marketo - Documentazione prodotto
title: Segmenti Web
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '2031'
ht-degree: 0%

---


# Segmenti Web {#web-segments}

## Visualizza segmento {#view-segment}

![](assets/image2014-11-11-20-3a24-3a5.png)

La scheda Segmenti visualizza tutti i segmenti definiti personalizzati che hai impostato in base a vari attributi.  **Un segmento è un insieme di visitatori che soddisfano i criteri specificati definiti nella pagina &quot;Imposta un segmento&quot;.**  Un segmento può essere rappresentato da visitatori provenienti da un settore specifico, da una posizione o in base all&#39;attività del visitatore sul posto.

In Personalizzazione Web, un visitatore può corrispondere a più segmenti. Ad esempio, se esiste un segmento per i visitatori statunitensi e un segmento per le società finanziarie, un visitatore Web della Bank of America corrisponderebbe a **sia** il segmento per il visitatore statunitense che il segmento per le società finanziarie.

**GRAFICO:**  Nella pagina Segmenti viene visualizzato un grafico a barre dei segmenti selezionati in base al numero di visitatori del segmento (asse y) e al nome del segmento (asse x).

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Nome</th> 
   <th colspan="1" rowspan="1">Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Nome</strong></td> 
   <td colspan="1" rowspan="1">Titolo del segmento</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Corrisponde</strong></p></td> 
   <td colspan="1" rowspan="1">Numero di visitatori che soddisfano i criteri definiti e personalizzati del segmento</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Imposta campagna</strong></td> 
   <td colspan="1" rowspan="1">Consente di impostare un CTA campagna associato al termine di ricerca selezionato</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Visitatori</strong></td> 
   <td colspan="1">Anteprima della tabella dei visitatori associata al termine di ricerca selezionato</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Clickstream</strong></td> 
   <td colspan="1" rowspan="1">Visualizza una tabella dell'attività e del percorso URL del visitatore sul sito e per quanto tempo ha visitato ogni pagina </td> 
  </tr> 
 </tbody> 
</table>

Vedere [come creare e visualizzare le etichette dei segmenti](/help/marketo/product-docs/web-personalization/using-web-segments/label-your-segment.md)

**Segmenti - Pannello a destra**

![](assets/image2014-11-12-10-3a46-3a32.png)

Quando si seleziona un segmento nella tabella, vengono visualizzati ulteriori dettagli sul segmento nel pannello a destra.

Tali dettagli comprendono:

* Nome del segmento
* Data di creazione del segmento
* Campagne associate che mostrano le campagne che operano con il segmento. Facendo clic sul numero di reazioni si passa alla pagina delle campagne in cui è visualizzato il CTA campagna (Invito all’azione) per il segmento
* Il numero di corrispondenze (quantità di visitatori che soddisfacevano i criteri del segmento) per il segmento e il numero di visitatori distinti (univoci) che corrispondevano al segmento. Facendo clic sul collegamento del visitatore univoco si passa alla pagina del visitatore in cui sono visualizzati i risultati del segmento
* Proprietario/creatore utente del segmento
* I siti di dominio associati al segmento
* Breve riepilogo dei criteri selezionati per il segmento

## Attivare o disattivare un segmento {#enable-or-disable-a-segment}

![](assets/image2014-11-12-10-3a48-3a9.png)

Per abilitare o disabilitare un segmento, seleziona la casella di controllo del segmento nella tabella e nella casella a discesa &quot;Scegli azione&quot; nella parte inferiore della tabella seleziona l’azione &quot;Abilita&quot; o &quot;Disattiva&quot;. Quando un segmento è disabilitato, sotto la colonna Stato viene visualizzata la parola &quot;disable&quot;.

## Crea segmenti {#create-segments}

Il segmento creato soddisfa i criteri specifici definiti nella pagina **Imposta segmento**. Puoi personalizzare i segmenti anche in base a una combinazione di criteri, con targeting per un&#39;audience specifica nella campagna.

Per creare un nuovo segmento

Dalla pagina **Segments**, fare clic su **Create New** sotto il grafico. Viene visualizzata la schermata seguente.

![](assets/four.png)

Definite i parametri generali per il segmento:

* **Nome:**  Denominate il segmento.
* **Descrizione:**  fornire una spiegazione più dettagliata dei criteri del segmento.
* **Domini:**  selezionare i domini che si desidera includere nel segmento.
* **Logica regola di segmento:**  selezionare una logica AND/OR per creare ogni attributo di segmentazione
* **Tempo:** definire il livello di coinvolgimento dei visitatori desiderato nella campagna

   * **All&#39;entrata**: Coinvolgi dall’arrivo del visitatore sul sito Web
   * **Dopo il 1°-9° clic**: Coinvolgi il visitatore dopo un numero specifico di clic sul sito Web

>[!TIP]
>
>**Logica regola segmento**
>
>Sono disponibili tre opzioni di filtro:
>
>1. Usa tutti i filtri (1, 2 e 3...)
>1. Usare eventuali filtri (1, 2 o 3...)
>1. Filtri avanzati (uso e/o espressioni)

   >
   >    
   I filtri avanzati consentono di controllare la condizione del segmento. Immettete i numeri del filtro separati da &quot;and&quot; e &quot;or&quot;.
   >
   >    
   * 1 e 2 e 3
   >    * 1 o 2 o 3

   >
   >    La combinazione di &quot;e&quot; e &quot;o&quot; richiede parentesi per chiarire le intenzioni logiche. ad esempio &quot;1 or 2 and 3&quot; deve essere scritto come segue:
   >
   >    
   * 1 e (2 o 3)
   >    * (1 e 2) o 3

   >
   >    Le parentesi nidificate sono accettate per logica più complessa, ad esempio
   >
   >    
   * (1 e 2) o (3 e 4)
   >    * 1 e 2 o 3 e 4)

   >
   >    Controllare la logica dopo qualsiasi inserimento, eliminazione o riordinamento.


Trascina gli attributi Segmento dalla colonna a destra all’editor segmenti a sinistra:

![](assets/five.png)

### Firmografia {#firmographics}

**Posizione**

Trascinare **Location** nell&#39;editor segmenti.

* Selezionate uno dei seguenti parametri:

   * **Includi** : consente di selezionare se la campagna deve includere o escludere una posizione.
   * **Selezionare il paese da aggiungere**  - Dalla casella a discesa, selezionare il paese che si desidera includere nel segmento. Il nome del paese viene visualizzato a destra. Potete scegliere più paesi.

Una volta aggiunto il paese, puoi specificare anche lo stato, la città e il codice postale del segmento.

* **Selezionare Stato o Provincia da aggiungere**  - Dalla casella a discesa, selezionare lo stato degli Stati Uniti o la Provincia canadese che si desidera includere. Potete effettuare più selezioni.
* **CAP** : immettete il codice postale da includere nel segmento.
* **Città**  - Entra nella città o nelle città che desideri includere. Usate il punto e virgola tra le città.

>[!TIP]
>
>**Quali sono le condizioni di segmento che scelgo? &quot;AND&quot; o &quot;OR&quot;?** OR funziona come un&#39;opzione aggiuntiva all&#39;interno di ciascun campo. Per qualificarsi per il segmento, le prospettive devono soddisfare solo uno dei criteri multipli selezionati all’interno di ciascun campo. Ad esempio, i potenziali possono provenire dagli Stati Uniti. *o* dall&#39;industria della difesa). E funziona come parametro obbligatorio aggiuntivo che deve essere soddisfatto per questo segmento. (Ad esempio, le prospettive devono provenire sia dagli Stati Uniti che dall&#39;industria della difesa). All&#39;interno di ciascun profilo di segmentazione, ogni campo separato può funzionare come entrambi, sia come &quot;AND&quot; che come &quot;OR&quot;, a seconda della condizione di segmento selezionata.

**** IndustrieNella sezione  **Segmentazione** profilo, selezionare la casella accanto a  **Industria**.

* Selezionate uno dei seguenti parametri:

   * **Include**  - Consente di specificare se il segmento deve includere o escludere un settore.
   * **Selezionate Settori da aggiungere**  - Selezionate il settore da includere nel segmento. Il settore viene visualizzato sotto la casella a discesa. Potete scegliere più settori.

**Gruppo organizzazione**

Nella sezione **Segmentazione profilo**, selezionare la casella accanto a **Gruppo organizzazione.**

* Dalla casella a discesa, selezionate una delle seguenti opzioni:

   * Fortune 500 - Include solo Fortune 500 aziende in questo segmento
   * Fortune 1000 - Include solo Fortune 1000 aziende in questo segmento
   * Globale 2000 - Include le aziende Global 2000 in questo segmento
   * Enterprise - Include organizzazioni con oltre 1.000 dipendenti e ricavi superiori a 250 milioni di dollari
   * PMI - Include solo piccole e medie imprese in questo segmento

**-Account denominati-**

**Organizzazioni**

* **Proviene da queste società (nomi specifici)**

   * Selezionate la società a cui rivolgervi dal menu a discesa &#39;Selezionate la società da aggiungere&#39;.
   * Puoi digitare il nome esatto dell&#39;organizzazione a cui vuoi indirizzare. *Si consiglia di utilizzare gli elenchi di account denominati invece di digitare manualmente i nomi per ottenere corrispondenze migliori (vedere di seguito).__

**Elenco account denominato**

Selezionare da un [Elenco account denominato](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md) per segmentare i principali account di destinazione.

![](assets/image2015-5-27-17-3a14-3a8.png)

>[!NOTE]
>
>Il numero tra parentesi accanto al nome dell&#39;elenco di account denominato viene utilizzato come riferimento di indice per l&#39;elenco per la personalizzazione Web [Leggi API](https://developers.marketo.com/documentation/websites/rtp-js-api/).

**Escludi ISP**

Esclude i provider di servizi Internet (ISP) dal segmento.

### Persone conosciute {#known-people}

**Database**

Web Personalization si integra con il database Marketo, consentendo di segmentare e personalizzare le campagne in base agli attributi e ai dati delle persone note.

Selezionare Database, quindi selezionare un campo dati persona dall&#39;elenco a discesa. Selezionare **+** per aggiungere i campi dall&#39;elenco a discesa.

![](assets/seven.png)

Puoi aggiungere o rimuovere i campi dati persona da Impostazioni account > Database

>[!TIP]
>
>Crea i criteri di segmento in base a tutti i campi di dati delle persone da Marketo, ad esempio Titolo processo; Punteggio; Ruolo; ecc...
>
>Esempio &quot;Titolo processo uguale a CMO&quot; e &quot;Valutazione minore o uguale a 50&quot;

**Invia per e-mail a** CampaignSegment e personalizza le campagne tramite e-mail di riferimento da un visitatore che fa clic su un&#39;e-mail di Marketo e arriva sul sito. Segmenta per Nome programma Marketo o Nome campagna e continua la conversazione dall’e-mail al Web. Selezionate il simbolo + per aggiungere i campi dall’elenco a discesa.

![](assets/image2015-5-27-17-3a20-3a34.png)

**Stato**

Definite il segmento in base allo stato di un potenziale: conosciuto o anonimo.

* Nota: selezionate questa opzione dalla casella a discesa per i visitatori noti. Un visitatore è noto quando invia un modulo sul sito Web e viene visualizzato nella pagina Persone di Web Personalization.
* Anonimo - Selezionate questa opzione dall&#39;elenco a discesa per i visitatori anonimi.

![](assets/image2015-5-27-17-3a23-3a2.png)

### Comportamento {#behavioral}

**Visite -** Definite il segmento in base al comportamento o all&#39;identificazione del visitatore.

* Numero di visite - Selezionate questa opzione dall&#39;elenco a discesa per specificare il numero di visite per i potenziali clienti sul sito Web.

   * Selezionare Uguale, Uguale o Superiore o Uguale o Inferiore a dalla casella a discesa.

* Visite specifiche - Selezionate questa opzione dalla casella a discesa per specificare un visitatore specifico.

   * Nella casella di testo a destra, inserite il numero del visitatore da monitorare. Il numero identificativo del visitatore di Web Personalization (Personalizzazione Web) univoco si trova quando si fa clic su un visitatore (nella pagina dei visitatori) e sul pannello di destra di Set Campaign. L’ID visitatore si trova nella sezione Impostazioni avanzate. L’ID visitatore si trova anche nell’URL (ad esempio, VISITOR=JZZJIFJNUI60PZ8Y97BHTY9BL8PKWS).

**Termini**  di ricerca - Consente di definire un segmento in base ai termini di ricerca di un potenziale.

* Il visitatore ricercato - Dall’elenco a discesa, selezionate i termini da monitorare dalla ricerca dei visitatori, o aggiungete i termini di ricerca personalizzati. (Non è necessario che il carattere jolly * nei termini di ricerca, in quanto è impostato come predefinito per includere frasi che contengono il termine di ricerca).

**Riferimenti**  - Aggiungete gli URL a cui ha fatto riferimento il visitatore.

* Seleziona i riferimenti da aggiungere: dall&#39;elenco a discesa, seleziona i siti di riferimento da tenere traccia o aggiungi un riferimento personalizzato. Una volta selezionati, i riferimenti vengono visualizzati nella casella sottostante. (L&#39;utilizzo di * come carattere jolly è consentito)

**Includi pagine**  - Consente di tenere traccia di pagine specifiche visitate sul sito Web.

* Corrispondenza URL - Aggiungete l&#39;URL di pagine Web specifiche da monitorare. Potete aggiungere più URL separandoli con un punto e virgola. (L&#39;utilizzo di * come carattere jolly è consentito).

**Escludi pagine**  - Escludi pagine specifiche per le quali non si desidera trovare una corrispondenza nel segmento. (L&#39;utilizzo di * come carattere jolly è consentito).

* URL non corrispondente - Aggiungete l’URL di pagine Web specifiche da escludere dal tracciamento. Potete aggiungere più URL separandoli con un punto e virgola

![](assets/segment-extra.png)

### Dispositivo/Browser {#device-browser}

**Sistema operativo mobile**

Trascinamento del sistema operativo mobile nell&#39;editor segmenti

![](assets/image2015-5-27-17-3a45-3a3.png)

* **Tipo di visitatore**<br />

   **Sistema operativo**  mobile: dalla casella a discesa, seleziona uno o più sistemi operativi mobili elencati. Il sistema operativo mobile selezionato viene visualizzato di seguito.

   * Il visitatore utilizza qualsiasi dispositivo mobile
   * Il visitatore utilizza questo dispositivo/sistema operativo specifico
   * Il visitatore non utilizza alcun dispositivo mobile

* **Dispositivo**   - Dall&#39;elenco a discesa, selezionare uno o più dispositivi (Apple, Samsung, LG, HTC, Nexus, Blackberry ecc.). I dispositivi selezionati vengono visualizzati di seguito.

**Browser**

Esegue il targeting dei visitatori che utilizzano tipi e/o versioni di browser specifici.

* Tipo di browser - Dalla casella a discesa, selezionare uno o più browser Internet. I browser selezionati vengono visualizzati di seguito.
* Versione browser - Immettere la versione del browser da aggiungere al segmento. Potete selezionare più versioni separandole con una virgola. (L&#39;utilizzo di * come carattere jolly è consentito).

### API {#api}

**Eventi**  di dati - Segmenti di visitatori che attivano eventi di dati personalizzati specifici

Aggiungete il valore Evento a cui desiderate destinare. Ad esempio, da origini dati di terze parti.

**API Context utente**

Chiamata API di personalizzazione Web [maggiori informazioni su di essa.](https://developers.marketo.com/documentation/websites/rtp-user-context-api/)

>[!TIP]
>
>**Utilizzo di caratteri jolly -** Quando si desidera includere qualsiasi termine di ricerca o URL che contenga elementi al suo interno, ad esempio &quot;[google.com](https://google.com)&quot; o &quot;search term product&quot;, lo chiamiamo un carattere jolly e dovrebbe essere inserito con un asterisco - questo piccolo ragazzo* - su ogni estremità. Pertanto, qualsiasi cosa proveniente da [google.com](https://google.com) deve essere inserita come * [google.com](https://google.com)*

## Modifica segmenti {#edit-segments}

Puoi modificare un segmento creato.

1. Per modificare un segmento, passare a **Segmenti**.

   ![](assets/image2014-11-12-11-3a38-3a22.png)

1. Nella tabella **Segments**, fare clic sull&#39;icona di modifica ( ![](assets/segment-edit.png)) del segmento da modificare. Viene aperta la pagina **Imposta segmento** con il segmento selezionato.
1. Applica le modifiche o le modifiche che desideri apportare al segmento.
1. Fare clic su **Salva**.

## Elimina segmenti {#delete-segments}

Puoi eliminare i segmenti creati.

1. Dalla pagina **Segments**, seleziona un segmento.
1. Fare clic sull&#39;icona di eliminazione ( ![](assets/segment-delete.png) ) del segmento da eliminare.
1. Viene visualizzato un messaggio di conferma che conferma l&#39;eliminazione del **Segment**.

>[!NOTE]
Non è possibile eliminare un segmento associato a una campagna. Prima è necessario eliminare la campagna e quindi il segmento.

Fantastico! Ora che hai compreso la sezione Segmenti, impariamo a conoscere le campagne.

>[!MORELIKETHIS]
* [Creare un segmento Web di base](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)
* [Creazione di una nuova finestra di dialogo Web Campaign](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
* [Creare una nuova campagna Web nella zona](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
* [Creare una nuova campagna Web Widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)

