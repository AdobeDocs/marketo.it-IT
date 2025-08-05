---
description: Note sulla versione corrente di Dynamic Chat - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione di Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
exl-id: 0a7e5cc9-f2a6-4721-bbdc-661249a2e2b6
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 3%

---

# Note sulla versione di Dynamic Chat {#dynamic-chat-release}

I rilasci di Adobe Dynamic Chat funzionano secondo un modello di distribuzione continua che consente un approccio più scalabile alla distribuzione delle funzioni. A volte ci sono più versioni in un mese, quindi controlla regolarmente per informazioni sempre aggiornate.

La pagina delle note sulla versione standard per Marketo Engage [ si trova qui](/help/marketo/release-notes/current.md){target="_blank"}.

## Versione di giugno 2025 {#june-2025-release}

### Rinnovo della logica di routing {#routing-logic-revamp}

Abbiamo rinnovato la logica di indirizzamento della chat in tempo reale in Dynamic Chat per garantire un comportamento di coinvolgimento più intelligente e prevedibile per tutti i tipi di indirizzamento (Account, Personalizzato, Team e Round Robin). La nuova logica semplifica i flussi di routing e migliora la gestione di fallback quando gli agenti non sono disponibili.

#### Miglioramenti chiave nel comportamento di indirizzamento

* **Fino a due tentativi di coinvolgimento per sessione**

   * Il sistema tenterà di connettersi con un massimo di due agenti (al massimo), ma rigorosamente all’interno della regola di routing principale.

   * Se un agente è disponibile ma non risponde (ad esempio, rifiuta o salta la chat), il sistema tenterà di connettersi a un altro agente dello stesso pool.

   * La logica di fallback (come Round Robin) viene attivata solo se non vengono trovati agenti idonei durante la risoluzione iniziale, per non riprovare dopo un coinvolgimento fallito.

* **Comportamento Specifico Della Regola Di Indirizzamento**

_&#x200B;**Indirizzamento account**&#x200B;_

Se il dominio e-mail di un visitatore è mappato su un account noto, l’agente mappato ha sempre la priorità.

Se l’agente è disponibile, la chat viene indirizzata direttamente a loro.

Se l&#39;agente non è disponibile, il sistema:

* Non tenta un altro agente, anche se Round Robin è abilitato come fallback.

* Invece:

   * Mostra il calendario della riunione dell&#39;agente mappato (se attivato).
-oppure-
   * Torna a un messaggio predefinito (caso peggiore).

La regola di routing a livello di scheda (ad esempio Team, Personalizzato) viene considerata solo se l’Instradamento account non è idoneo (nessun dominio o agente corrispondente).

_&#x200B;**Indirizzamento personalizzato/team**&#x200B;_

Queste regole possono restituire più agenti idonei.

Se il primo agente disponibile non si attiva, il sistema tenterà un altro agente dallo stesso elenco.

Il fallback Round Robin non viene attivato solo perché un agente non risponde.

Se nessuno dei due agenti si impegna:

* Il sistema visualizza il calendario del primo agente provato (se attivato).
-oppure-
* Visualizza il messaggio di fallback predefinito.

_&#x200B;**Routing Robin Round**&#x200B;_

Quando viene utilizzato come regola di instradamento principale, il sistema:

* Tenta di coinvolgere il primo agente disponibile dal pool round robin.

* Se il primo agente non risponde, tenta di nuovo con il migliore agente idoneo successivo.

Se Round Robin viene utilizzato come fallback, si attiva solo se non vengono risolti agenti dalla regola primaria.

_&#x200B;**Flusso esperienza visitatore**&#x200B;_

Il sistema controlla se è applicabile l&#39;Instradamento conto.

* Se sì e l’agente è disponibile, si connette immediatamente.

* Se l&#39;agente non è idoneo o non disponibile, passa alla regola di routing a livello di scheda.

Viene valutata la regola di routing a livello di scheda (Personalizzato, Team, Round Robin).

* Gli agenti idonei vengono verificati per la disponibilità (autorizzazioni, stato).

* Il sistema coinvolge un agente e, se necessario, tenta un secondo agente dalla stessa regola.

* Se il coinvolgimento non ha esito positivo, viene applicata la logica di fallback:

   * Fallback del calendario (se attivato),
-oppure-
   * Messaggio predefinito.

Il fallback Round Robin viene considerato solo quando non vengono trovati agenti idonei dalla regola di routing principale, non quando i singoli agenti non rispondono.

##### Casi d’uso {#use-cases}

_&#x200B;**Indirizzamento account**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Esempio</th>
    <th>Risultato</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideale</td>
    <td>Il dominio del visitatore è associato a un account; l’agente mappato ha una chat in tempo reale abilitata ed è disponibile</td>
    <td>La chat si connette direttamente all’agente mappato</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>L’agente mappato non è disponibile. Il fallback Round Robin è abilitato</td>
    <td>Il sistema seleziona un agente disponibile tramite Round Robin e li coinvolge </td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>L’agente mappato non è disponibile, nessun fallback Round Robin; la prenotazione della riunione è abilitata</td>
    <td>Il sistema mostra il calendario dell'agente mappato o visualizza un messaggio di fallback predefinito</td>
  </tr>
</tbody></table>

_&#x200B;**Routing personalizzato**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Esempio</th>
    <th>Risultato</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideale</td>
    <td>La logica personalizzata risolve un elenco di agenti; il primo agente è disponibile e accetta la chat.</td>
    <td>La chat si connette al primo agente.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>La regola personalizzata non risolve alcun agente; il fallback Round Robin è abilitato.</td>
    <td>Il sistema seleziona un agente disponibile tramite Round Robin e li coinvolge.</td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>Due agenti sono stati risolti; nessuno dei due accetta la chat e il fallback è impostato sul calendario della riunione.</td>
    <td>Viene visualizzato il calendario dell'agente provato per primo oppure il messaggio di fallback predefinito.</td>
  </tr>
</tbody></table>

_&#x200B;**Indirizzamento team**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Esempio</th>
    <th>Risultato</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideale</td>
    <td>Il team include agenti con chat in tempo reale; il primo agente disponibile accetta la chat.</td>
    <td>La chat si connette a tale agente.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Nessun agente team disponibile e il fallback Round Robin è abilitato.</td>
    <td>Il sistema seleziona e si connette con un agente del pool Round Robin.</td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>Due agenti disponibili, ma nessuno dei due è coinvolto; il fallback del calendario è abilitato.</td>
    <td>Viene visualizzato il calendario del primo agente provato oppure viene attivato il messaggio di fallback.</td>
  </tr>
</tbody></table>

_&#x200B;**Routing Robin Round**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Esempio</th>
    <th>Risultato</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideale</td>
    <td>Round Robin pool ha più agenti; secondo agente accetta chat dopo primo non lo fa.</td>
    <td>La chat si connette al secondo agente.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Nessun agente disponibile nel pool Round Robin. Il calendario della riunione è abilitato.</td>
    <td>Il calendario viene visualizzato per il primo agente nell’elenco (se configurato), oppure viene visualizzato il messaggio di fallback.</td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>Nessun agente disponibile; il fallback è disabilitato.</td>
    <td>Al visitatore viene mostrato un messaggio di fallback statico.</td>
  </tr>
</tbody></table>

### Notifica Pulse {#pulse-notification}

Ogni volta che un visitatore richiede di connettersi con un agente, forniamo all’agente una notifica in-app tramite browser. Ma a volte, gli agenti perdono queste chat.

Con questa versione, l’agente live può ricevere una notifica e-mail, Slack, in-app e browser quando un nuovo visitatore è interessato alla chat.

1. Nella home page di Adobe Experience Cloud, fai clic sull&#39;icona Account e seleziona **Preferenze**.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Scorri verso il basso fino a _Notifiche_ e seleziona il Dynamic Chat desiderato.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>Il contenuto di una notifica Pulse può essere lo stesso utilizzato per le notifiche in-app del browser.
