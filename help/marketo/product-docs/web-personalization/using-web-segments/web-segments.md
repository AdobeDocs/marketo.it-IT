---
unique-page-id: 4719093
description: Segmenti web - Documentazione di Marketo - Documentazione del prodotto
title: Segmenti web
exl-id: ec62c1ae-579a-4753-9b2d-18c7c2fa1ff5
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1980'
ht-degree: 0%

---

# Segmenti web {#web-segments}

## Visualizza segmento {#view-segment}

![](assets/image2014-11-11-20-3a24-3a5.png)

Nella scheda Segmenti vengono visualizzati tutti i segmenti personalizzati definiti in base a vari attributi.  **Un segmento è una raccolta di visitatori che soddisfano i criteri specificati definiti nella pagina &quot;Imposta un segmento&quot;.** Un segmento può essere costituito da visitatori provenienti da un settore, una posizione o un&#39;attività in loco del visitatore.

In [!DNL Web Personalizatio] un visitatore può corrispondere a più segmenti. Ad esempio, se è presente un segmento per i visitatori negli Stati Uniti e un segmento per le società di servizi finanziari, un visitatore Web di Bank of America troverà **entrambi** il segmento per il visitatore negli Stati Uniti e il segmento per le società di servizi finanziari.

**GRAFICO:** La pagina Segmenti visualizza un grafico a barre dei segmenti selezionati in base al numero di visitatori dal segmento (asse y) e al nome del segmento (asse x).

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
   <td colspan="1" rowspan="1"><p><strong>Corrisponde a</strong></p></td>
   <td colspan="1" rowspan="1">Il numero di visitatori che soddisfano i criteri personalizzati e definiti del segmento</td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><strong>Imposta campagna</strong></td>
   <td colspan="1" rowspan="1">Consente di impostare una campagna CTA associata al termine di ricerca selezionato</td>
  </tr>
  <tr>
   <td colspan="1"><strong>Visitatori</strong></td>
   <td colspan="1">Anteprima della tabella dei visitatori associata al termine di ricerca selezionato</td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><strong>Clickstream</strong></td>
   <td colspan="1" rowspan="1">Visualizza una tabella dell’attività e del percorso URL del visitatore sul sito, con indicazione di quanto tempo ha visitato ciascuna pagina. </td>
  </tr>
 </tbody>
</table>

Consulta [come creare e visualizzare le etichette dei segmenti](/help/marketo/product-docs/web-personalization/using-web-segments/label-your-segment.md)

**Segmenti - Pannello di destra**

![](assets/image2014-11-12-10-3a46-3a32.png)

Selezionando un segmento nella tabella vengono visualizzati ulteriori dettagli sul segmento nel pannello di destra.

Tali dettagli includono:

* Nome del segmento
* Data di creazione del segmento
* Le campagne associate che mostrano le campagne che operano con il segmento. Facendo clic sul numero di reazioni si accede alla pagina delle campagne in cui è visualizzato il CTA della campagna (Call to action) per il segmento
* Il numero di corrispondenze (numero di visitatori che hanno soddisfatto i criteri del segmento) per il segmento e il numero di visitatori distinti (univoci) che hanno soddisfatto il segmento. Facendo clic sul collegamento visitatore univoco si accede alla pagina del visitatore che mostra i risultati del segmento
* Proprietario/creatore utente del segmento
* I siti di dominio associati al segmento
* Breve riepilogo dei criteri selezionati per il segmento

## Attivare o disattivare un segmento {#enable-or-disable-a-segment}

![](assets/image2014-11-12-10-3a48-3a9.png)

Per abilitare o disabilitare un segmento, selezionare la casella di controllo di tale segmento nella tabella e nella casella a discesa &quot;[!UICONTROL Choose Action]&quot; nella parte inferiore della tabella selezionare l&#39;azione &quot;[!UICONTROL Enable]&quot; o &quot;[!UICONTROL Disable]&quot;. Quando un segmento è disabilitato, la parola &quot;disable&quot; viene visualizzata nella colonna [!UICONTROL State].

## Creare segmenti {#create-segments}

Il segmento creato soddisfa i criteri specifici definiti nella pagina **[!UICONTROL Set Segment]**. Puoi personalizzare i segmenti anche in base a una combinazione di criteri, con targeting per un pubblico specifico nella campagna.

Per creare un nuovo segmento

Dalla pagina **[!UICONTROL Segments]**, fai clic su **[!UICONTROL Create New]** sotto il grafico. Viene visualizzata la seguente schermata.

![](assets/four.png)

Definisci i parametri generali per il segmento:

* **Nome:** Assegna un nome al segmento.
* **Descrizione:** Fornisci una spiegazione più dettagliata dei criteri del segmento.
* **Domini:** Selezionare i domini da includere nel segmento.
* **Logica regola segmento:** Seleziona una logica AND/OR per generare ciascun attributo di segmentazione
* **Tempistica:** definisci il livello di coinvolgimento dei visitatori desiderato nella campagna

   * **Alla voce**: la partecipazione del visitatore arriva al sito Web
   * **Dopo il 1° - 9° clic**: coinvolgi il visitatore dopo un numero specifico di clic sul sito Web

>[!TIP]
>
>**Logica regola segmento**
>
>Sono disponibili tre opzioni di filtro:
>
>1. Usa tutti i filtri (1, 2 e 3...)
>1. Utilizza qualsiasi filtro (1, 2 o 3...)
>1. Filtri avanzati (utilizzando espressioni e/o)
>
>    I filtri avanzati ti consentono di controllare la condizione del segmento. Immettere i numeri di filtro separati da &quot;and&quot; e &quot;or&quot;.
>
>    * 1, 2 e 3
>    * 1, 2 o 3
>
>    La miscelazione di &quot;and&quot; e &quot;or&quot; richiede parentesi per chiarire l&#39;intenzione logica. ad esempio, &quot;1 o 2 e 3&quot; devono essere scritti in uno dei seguenti modi:
>
>    * 1 e 2 o 3
>    * (1 e 2) o 3
>
>    Le parentesi nidificate sono accettate per una logica più complicata.es.
>
>    * (1 e 2) o (3 e 4)
>    * 1 e (2 o (3 e 4))
>
>    Controlla la logica dopo qualsiasi operazione di inserimento, eliminazione o riordinamento.

Trascina e rilascia gli attributi del segmento dalla colonna di destra all’editor segmento sul lato sinistro:

![](assets/five.png)

### Firmografica {#firmographics}

**Posizione**

Trascina **[!UICONTROL Location]** nell&#39;editor segmenti.

* Seleziona uno dei seguenti parametri:

   * **[!UICONTROL Include]** - Specificare se si desidera che la campagna includa o escluda una posizione.
   * **[!UICONTROL Select country to add]** - Selezionare il paese da includere nel segmento dalla casella a discesa. Il nome del paese appare a destra. Puoi scegliere più paesi.

Una volta aggiunto il paese, puoi specificare anche lo stato, la città e il codice postale del segmento.

* **[!UICONTROL Select State or Province to add]** - Dalla casella a discesa, selezionare lo stato degli Stati Uniti o la provincia canadese che si desidera includere. Puoi effettuare più selezioni.
* **[!UICONTROL Zip Code]** - Immetti il codice postale da includere nel segmento.
* **[!UICONTROL Cities]** - Immettere la città o le città da includere. Utilizzare un punto e virgola tra le città.

>[!TIP]
>
>**Quali sono le condizioni del segmento scelte? &#39;AND&#39; o &#39;OR&#39;?** OR funziona come opzione aggiuntiva all&#39;interno di ogni campo. I potenziali clienti devono soddisfare solo uno dei criteri multipli selezionati all’interno di ciascun campo per qualificarsi per il segmento. (Ad esempio, i potenziali clienti possono provenire dagli Stati Uniti *o* dall&#39;industria della difesa). AND funge da parametro obbligatorio aggiuntivo che deve essere soddisfatto per questo segmento. (Ad esempio, le prospettive devono provenire sia dagli Stati Uniti che dall&#39;industria della Difesa). All’interno di ciascun profilo di segmentazione, ogni campo separato può funzionare come entrambi, sia come &quot;AND&quot; che come &quot;OR&quot; a seconda della Condizione del segmento selezionata.

**Settori** Nella sezione **[!UICONTROL Profile Segmentation]**, seleziona la casella accanto a **[!UICONTROL Industry]**.

* Seleziona uno dei seguenti parametri:

   * **[!UICONTROL Includes]** - Selezionare se si desidera che il segmento includa o escluda un settore.
   * **[!UICONTROL Select Industries to add]** - Selezionare il settore da includere nel segmento. Il settore viene visualizzato sotto la casella a discesa. Puoi scegliere tra più settori.

**Gruppo organizzazione**

Nella sezione **[!UICONTROL Profile Segmentation]**, seleziona la casella accanto a **[!UICONTROL Organization Group].**

* Dalla casella di riepilogo a discesa, seleziona una delle seguenti opzioni:

   * Fortune 500 - Include solo le aziende Fortune 500 in questo segmento
   * Fortune 1000 - Include solo le aziende Fortune 1000 in questo segmento
   * Global 2000 - Include le aziende Global 2000 in questo segmento
   * Enterprise: include le organizzazioni con più di 1.000 dipendenti e ricavi superiori a 250 milioni di dollari
   * PMI: include solo le piccole e medie imprese in questo segmento

Account denominati **-**

**Organizzazioni**

* **Appartiene a queste società (nomi specifici)**

   * Seleziona la società di destinazione dal menu a discesa &quot;Seleziona la società da aggiungere&quot;.
   * Puoi digitare il nome esatto dell’organizzazione di destinazione. *Si consiglia _sempre_ di utilizzare gli Elenchi di account denominati invece di digitare manualmente i nomi per ottenere corrispondenze migliori (vedi sotto).

**Elenco account denominati**

Seleziona da un [elenco account denominati](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md) per segmentare gli account di destinazione chiave.

![](assets/image2015-5-27-17-3a14-3a8.png)

>[!NOTE]
>
>Il numero tra parentesi accanto al nome dell&#39;elenco di account denominati viene utilizzato come riferimento di indice per l&#39;elenco per Web Personalization [API di lettura](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/javascriptapi/web-personalization).

**Escludi ISP**

Esclude i provider di servizi Internet (ISP) dal segmento.

### Persone note {#known-people}

**[!UICONTROL Database]**

[!DNL Web Personalization] si integra con il tuo database Marketo, consentendoti di segmentare e personalizzare le campagne in base agli attributi e ai dati della persona nota.

Selezionare Database, quindi selezionare un campo dati persona dall&#39;elenco a discesa. Seleziona **+** per aggiungere campi dal menu a discesa.

![](assets/seven.png)

È possibile aggiungere o rimuovere campi dati persona da Impostazioni account > Database

>[!TIP]
>
>Crea i criteri di segmento in base a tutti i campi di dati relativi alle persone provenienti da Marketo, ad esempio Titolo mansione, Punteggio, Ruolo e così via.
>
>Esempio: &quot;Il titolo del lavoro è uguale a CMO&quot; e &quot;il punteggio è minore o uguale a 50&quot;

**[!UICONTROL Marketo Email Campaign]** Segmenta e personalizza le campagne tramite riferimento e-mail da parte di un visitatore che fa clic su un&#39;e-mail di Marketo e arriva sul sito. Segmentazione in base al nome del programma Marketo o al nome della campagna e continuazione della conversazione dall&#39;e-mail al Web. Seleziona il + per aggiungere campi dal menu a discesa.

![](assets/image2015-5-27-17-3a20-3a34.png)

**[!UICONTROL Status]**

Definisci il segmento in base allo stato di un potenziale cliente: noto o anonimo.

* Nota: seleziona questa opzione dall’elenco a discesa per i visitatori noti. Un visitatore è noto quando invia un modulo sul sito Web e viene visualizzato nella pagina [!DNL Web Personalization] [!UICONTROL People].
* Anonimo: seleziona questa opzione dall’elenco a discesa per i visitatori anonimi.

![](assets/image2015-5-27-17-3a23-3a2.png)

### Comportamento {#behavioral}

**[!UICONTROL Visits]-** Definisci il segmento in base al comportamento o all&#39;identificazione del visitatore.

* Numero di visite: seleziona questa opzione dalla casella a discesa per specificare il numero di visite per i potenziali clienti sul sito web.

   * Seleziona Uguale a, Uguale a o Maggiore di o Uguale a o Minore di dalla casella di riepilogo a discesa.

* Visite specifiche: seleziona questa opzione dalla casella a discesa per specificare un visitatore specifico.

   * Nella casella di testo a destra, immetti il numero del visitatore che desideri monitorare. Il numero di identificazione univoco del visitatore [!DNL Web Personalization] si trova quando si fa clic su un visitatore (nella pagina dei visitatori) e si imposta Campaign sul pannello laterale destro. L’ID visitatore si trova nella sezione Impostazioni avanzate. L’ID visitatore si trova anche nell’URL (ad esempio VISITOR=JZZJIFJNUI60PZ8Y97BHTY9BL8PKWS).

**Termini di ricerca** - Definisci un segmento in base ai termini di ricerca di un potenziale cliente.

* Il visitatore ha cercato: dall’elenco a discesa, seleziona i termini di cui vuoi tenere traccia dalla ricerca dei visitatori, oppure aggiungi i tuoi termini di ricerca. Non è necessario inserire il carattere jolly &#42; nei termini di ricerca perché è impostato come predefinito per includere frasi che contengono il termine di ricerca.

**[!UICONTROL Referrals]** - Aggiungi gli URL a cui il visitatore faceva riferimento.

* Seleziona i riferimenti da aggiungere: dall’elenco a discesa, seleziona i siti di riferimento di cui desideri tenere traccia o aggiungi un riferimento personalizzato. Una volta selezionati, i riferimenti verranno visualizzati nella casella sottostante. (L&#39;utilizzo di &#42; come carattere jolly è consentito)

**[!UICONTROL Include Pages]** - Tieni traccia di pagine specifiche potenziali visitate sul tuo sito Web.

* Corrispondenze URL: aggiungi l’URL di specifiche pagine web di cui desideri tenere traccia. È possibile aggiungere più URL separandoli con un punto e virgola. L&#39;utilizzo di &#42; come carattere jolly è consentito.

**[!UICONTROL Exclude Pages]** - Escludi le pagine specifiche alle quali non desideri trovare corrispondenza nel segmento. L&#39;utilizzo di &#42; come carattere jolly è consentito.

* URL non corrispondente - Aggiungi l’URL di specifiche pagine web da escludere dal tracciamento. È possibile aggiungere più URL separandoli con un punto e virgola

![](assets/segment-extra.png)

### Dispositivo/Browser {#device-browser}

**[!UICONTROL Mobile OS]**

Trascina e rilascia [!UICONTROL Mobile OS] nell&#39;editor segmenti

![](assets/image2015-5-27-17-3a45-3a3.png)

* **Tipo visitatore**<br />
  **[!UICONTROL Mobile OS]** - Dalla casella a discesa, selezionare uno o più sistemi operativi mobili elencati. Il sistema operativo mobile selezionato viene visualizzato di seguito.

   * Il visitatore sta utilizzando un dispositivo mobile
   * Il visitatore sta utilizzando questo dispositivo/sistema operativo specifico
   * Il visitatore non utilizza alcun dispositivo mobile

* **[!UICONTROL Device]** - Dall&#39;elenco a discesa, selezionare uno o più dispositivi (Apple, Samsung, LG, HTC, Nexus, Blackberry, ecc.). I dispositivi selezionati vengono visualizzati di seguito.

**Browser**

Puoi indirizzare l’attività a visitatori che utilizzano tipi e/o versioni specifici del browser.

* Tipo di browser: dalla casella a discesa, seleziona uno o più browser Internet. I browser selezionati vengono visualizzati di seguito.
* Versione browser: immetti la versione del browser da aggiungere al segmento. Puoi selezionare più versioni separandole con una virgola. L&#39;utilizzo di &#42; come carattere jolly è consentito.

### API {#api}

**Eventi dati** - Segmenta i visitatori che attivano eventi dati personalizzati specifici

Aggiungi il valore Evento di destinazione. Ad esempio da fonti di dati di terze parti.

**API contesto utente**

Chiamata API Web Personalization [ulteriori informazioni qui.](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/javascriptapi/web-personalization)

>[!TIP]
>
>**Utilizzo di caratteri jolly -** Quando si desidera includere qualsiasi termine di ricerca o URL che contiene un elemento, ad esempio &quot;[google.com](https://google.com)&quot; o &quot;prodotto del termine di ricerca&quot;, questo è un carattere jolly e deve essere inserito con un asterisco, questo piccolo tizio&#42;, su ogni estremità. Quindi tutto ciò che proviene da [google.com](https://google.com) deve essere immesso come &#42; [google.com](https://google.com)&#42;

## Modifica [!UICONTROL Segments] {#edit-segments}

Puoi modificare un segmento che è stato creato.

1. Per modificare un segmento, passa a **[!UICONTROL Segments]**.

   ![](assets/image2014-11-12-11-3a38-3a22.png)

1. Nella tabella **[!UICONTROL Segments]**, fare clic sull&#39;icona di modifica ( ![](assets/segment-edit.png)) del segmento che si desidera modificare. Viene aperta la pagina **[!UICONTROL Set Segment]** con il segmento selezionato.
1. Applica al segmento le modifiche che desideri apportare.
1. Fai clic su **[!UICONTROL Save]**.

## Eliminare segmenti {#delete-segments}

Puoi eliminare i segmenti creati.

1. Dalla pagina **[!UICONTROL Segments]** in alto, seleziona un segmento.
1. Fare clic sull&#39;icona Elimina ( ![](assets/segment-delete.png) ) del segmento che si desidera eliminare.
1. Viene visualizzato un messaggio di conferma che conferma l&#39;eliminazione del **segmento**.

>[!NOTE]
>
>Non puoi eliminare un segmento associato a una campagna. Devi innanzitutto eliminare la campagna e quindi il segmento.

Fantastico! Ora che conosci la sezione Segmenti, scopri le campagne.

>[!MORELIKETHIS]
>
>* [Crea un segmento Web di base](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)
>* [Crea una nuova campagna Web di dialogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [Crea una nuova campagna Web nell&#39;area](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [Crea una nuova campagna Web Widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
