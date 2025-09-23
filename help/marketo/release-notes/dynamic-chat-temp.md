---
description: Note sulla versione corrente di Dynamic Chat - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione di Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
exl-id: 0a7e5cc9-f2a6-4721-bbdc-661249a2e2b6
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 68%

---

# Note sulla versione di Dynamic Chat {#dynamic-chat-release}

Le versioni di Adobe Dynamic Chat funzionano su un modello di consegna continua che consente un approccio più scalabile all’implementazione delle funzioni. A volte ci sono più versioni in un mese, quindi controlla regolarmente per avere informazioni sempre aggiornate.

La pagina delle note sulla versione standard per Marketo Engage [si trova qui](/help/marketo/release-notes/current.md){target="_blank"}.

## Versione di giugno 2025 {#june-2025-release}

### Rinnovo della logica di indirizzamento {#routing-logic-revamp}

La logica di indirizzamento della chat in tempo reale in Dynamic Chat è stata rinnovata per garantire un comportamento di coinvolgimento più intelligente e prevedibile per tutti i tipi di indirizzamento (Account, Personalizzato, Team e Round Robin). La nuova logica semplifica i flussi di indirizzamento e migliora la gestione di fallback quando gli agenti non sono disponibili.

#### Miglioramenti chiave nel comportamento di indirizzamento

* **Fino a due tentativi di coinvolgimento per sessione**

   * Il sistema tenta di connettersi con un massimo di due agenti, ma rigorosamente all’interno della regola di routing principale.

   * Se un agente è disponibile ma non risponde (ad esempio, rifiuta o salta la chat), il sistema tenta di connettersi a un altro agente dello stesso pool.

   * La logica di fallback (come Round Robin) viene attivata solo se non vengono trovati agenti idonei durante la risoluzione iniziale, per non riprovare dopo un coinvolgimento fallito.

* **Comportamento specifico della regola di indirizzamento**

_&#x200B;**Indirizzamento account**&#x200B;_

Se il dominio e-mail di un visitatore è mappato su un account noto, l’agente mappato ha sempre la priorità.

Se l’agente è disponibile, la chat gli viene indirizzata direttamente.

Se l’agente non è disponibile, il sistema:

* Non fa un tentativo con un altro agente, anche se Round Robin è abilitato come fallback.

Invece:

* Mostra il calendario della riunione dell&#39;agente mappato (se attivato) oppure:
* Torna a un messaggio predefinito (caso peggiore).

La regola di routing a livello di scheda (ad esempio, Team, Personalizzato) viene considerata solo se l’Instradamento account non è idoneo (nessun dominio o agente corrispondente).

_&#x200B;**Indirizzamento personalizzato/team**&#x200B;_

Queste regole possono restituire più agenti idonei.

Se il primo agente disponibile non si attiva, il sistema tenta un altro agente dallo stesso elenco.

Il fallback Round Robin non viene attivato solo perché un agente non risponde.

Se nessuno dei due agenti risponde:

* Il sistema mostra il calendario del primo agente provato (se attivato).
-oppure-
* Mostra il messaggio di fallback predefinito.

_&#x200B;**Indirizzamento Round Robin**&#x200B;_

Quando viene utilizzato come regola di indirizzamento principale, il sistema:

* Tenta di coinvolgere il primo agente disponibile dal pool Round Robin.

* Se il primo agente non risponde, tenta di nuovo con il migliore agente idoneo successivo.

Se Round Robin viene utilizzato come fallback, si attiva solo se non vengono risolti agenti dalla regola primaria.

_&#x200B;**Flusso esperienza visitatore**&#x200B;_

Il sistema verifica se è applicabile l’indirizzamento dell’account.

* In caso positivo e se l’agente è disponibile, si connette immediatamente.

* Se l’agente è non idoneo o non disponibile, passa alla regola di indirizzamento a livello di scheda.

Sono state valutate le regole di indirizzamento a livello di scheda (Personalizzato, Team, Round Robin).

* Viene verificata la disponibilità (autorizzazioni, stato) degli agenti idonei.

* Il sistema coinvolge un agente e, se necessario, tenta un secondo agente dalla stessa regola.

* Se non viene completato alcun coinvolgimento, viene applicata la logica di fallback:

   * Fallback calendario (se attivato),
-oppure-
   * Messaggio predefinito.

Il fallback Round Robin viene considerato solo quando non vengono trovati agenti idonei dalla regola di indirizzamento principale, non quando i singoli agenti non rispondono.

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
    <td>Fallback (algoritmo Round Robin)</td>
    <td>L’agente mappato non è disponibile. Il fallback Round Robin è abilitato</td>
    <td>Il sistema seleziona un agente disponibile tramite Round Robin e li coinvolge </td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>L’agente mappato non è disponibile, nessun fallback Round Robin; la prenotazione della riunione è abilitata</td>
    <td>Il sistema mostra il calendario di un agente mappato o visualizza un messaggio di fallback predefinito</td>
  </tr>
</tbody></table>

_&#x200B;**Indirizzamento personalizzato**&#x200B;_

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
    <td>Fallback (algoritmo Round Robin)</td>
    <td>La regola personalizzata non risolve alcun agente. Il fallback Round Robin è abilitato.</td>
    <td>Il sistema seleziona un agente disponibile tramite Round Robin e li coinvolge.</td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>Due agenti sono stati risolti; nessuno dei due accetta la chat e il fallback è impostato sul calendario della riunione.</td>
    <td>Si è tentato di visualizzare il calendario dell'agente oppure il messaggio di fallback predefinito.</td>
  </tr>
</tbody></table>

_&#x200B;**Instradamento team**&#x200B;_

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
    <td>Fallback (algoritmo Round Robin)</td>
    <td>Nessun agente del team è disponibile e il fallback Round Robin è abilitato.</td>
    <td>Il sistema seleziona e si connette con un agente del pool Round Robin.</td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>Due agenti sono disponibili, ma nessuno dei due è coinvolto; il fallback del calendario è abilitato.</td>
    <td>Si è tentato prima di visualizzare il calendario dell’agente o di attivare un messaggio di fallback.</td>
  </tr>
</tbody></table>

_&#x200B;**Indirizzamento Round Robin**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Esempio</th>
    <th>Risultato</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideale</td>
    <td>Round Robin pool ha più agenti; il secondo agente accetta chat dopo il primo non lo fa.</td>
    <td>La chat si connette a un secondo agente.</td>
  </tr>
  <tr>
    <td>Fallback (algoritmo Round Robin)</td>
    <td>Nessun agente disponibile nel pool Round Robin. Il calendario della riunione è abilitato.</td>
    <td>Viene visualizzato il calendario per il primo agente nell’elenco (se configurato), oppure viene visualizzato il messaggio di fallback.</td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>Nessun agente disponibile; il fallback è disabilitato.</td>
    <td>Al visitatore viene mostrato un messaggio di fallback statico.</td>
  </tr>
</tbody></table>

### Notifica Pulse {#pulse-notification}

Ogni volta che un visitatore richiede di connettersi con un agente, forniamo una notifica in-app del browser all’agente. Ma a volte, gli agenti perdono queste chat.

Con questa versione, l’agente live può ricevere una notifica e-mail, Slack, in-app e su browser quando un nuovo visitatore è interessato a comunicare via chat.

1. Nella home page di Adobe Experience Cloud, fai clic sull’icona Account e seleziona **Preferenze**.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Scorri verso il basso fino a _Notifiche_ e seleziona la Dynamic Chat desiderata.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>Il contenuto di una notifica Pulse può essere lo stesso utilizzato per le notifiche in-app del browser.
