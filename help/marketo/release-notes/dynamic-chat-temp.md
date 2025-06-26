---
description: Note sulla versione corrente di Dynamic Chat - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione di Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: ce7142e471271dfb33b265e226b67bcc3b35594b
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 4%

---

# Note sulla versione di Dynamic Chat {#dynamic-chat-release}

I rilasci di Adobe Dynamic Chat funzionano secondo un modello di distribuzione continua che consente un approccio più scalabile alla distribuzione delle funzioni. A volte ci sono più versioni in un mese, quindi controlla regolarmente per informazioni sempre aggiornate.

La pagina delle note sulla versione standard per Marketo Engage [ si trova qui](/help/marketo/release-notes/current.md){target="_blank"}.

## Versione di giugno 2025 {#june-25-release}

### Rinnovo della logica di routing {#routing-logic-revamp}

Abbiamo rinnovato la logica di indirizzamento della chat in tempo reale in Dynamic Chat per garantire un comportamento di coinvolgimento più intelligente e prevedibile per tutti i tipi di indirizzamento (Account, Personalizzato, Team e Round Robin). La nuova logica semplifica i flussi di routing e migliora la gestione di fallback quando gli agenti non sono disponibili.

#### Miglioramenti chiave nel comportamento di indirizzamento

* **Fino a due tentativi di coinvolgimento per sessione**

   * Il sistema tenterà di connettersi con al massimo due agenti, ma rigorosamente all’interno della regola di routing principale.

   * Se un agente è disponibile ma non risponde (ad esempio, rifiuta o non risponde), il sistema tenterà un secondo agente dallo stesso pool.

   * La logica di fallback (come Round Robin) viene attivata solo se non vengono trovati agenti idonei durante la risoluzione iniziale, per non riprovare dopo un coinvolgimento fallito.

* **Comportamento Specifico Della Regola Di Indirizzamento**

_**Indirizzamento account**_

Se il dominio e-mail di un visitatore è mappato su un account noto, l’agente mappato ha sempre la priorità.

Se l’agente è disponibile, la chat viene indirizzata direttamente a loro.

Se l&#39;agente non è disponibile, il sistema:

Non tenta un altro agente, anche se Round Robin è abilitato come fallback.

Invece:

Mostra il calendario della riunione dell&#39;agente mappato (se attivato) oppure

Torna a un messaggio predefinito (caso peggiore).

La regola di routing a livello di scheda (ad esempio Team, Personalizzato) viene considerata solo se l’Instradamento account non è idoneo (nessun dominio o agente corrispondente).

_**Indirizzamento personalizzato/team**_

Queste regole possono restituire più agenti idonei.

Se il primo agente disponibile non si attiva, il sistema tenterà un altro agente dallo stesso elenco.

Il fallback Round Robin non viene attivato solo perché un agente non ha risposto.

Se nessuno dei due agenti si impegna:

Il sistema visualizza il calendario del primo agente provato (se attivato) oppure

Visualizza il messaggio di fallback predefinito.

_**Routing Robin Round**_

Quando viene utilizzato come regola di instradamento principale, il sistema:

Tenta di coinvolgere il primo agente disponibile dal pool round robin.

Se il primo non risponde, si tenta di nuovo con il migliore agente idoneo successivo.

Se Round Robin viene utilizzato come fallback, si attiva solo se non vengono risolti agenti dalla regola primaria.

**Flusso esperienza visitatore**

Il sistema controlla se l&#39;Instradamento conto è applicabile.

Se sì e l’agente è disponibile → si connette immediatamente.

Se non idoneo o agente non disponibile, → alla regola di routing a livello di scheda.

Viene valutata la regola di routing a livello di scheda (Personalizzato, Team, Round Robin).

Gli agenti idonei vengono verificati per la disponibilità (autorizzazioni, stato).

Il sistema coinvolge un agente e, se necessario, tenta un secondo agente dalla stessa regola.

Se non viene eseguito alcun coinvolgimento → viene applicata la logica di fallback:

Fallback del calendario (se attivato), oppure

Messaggio predefinito.

Il fallback Round Robin viene considerato solo quando non vengono trovati agenti idonei dalla regola di routing principale, non quando i singoli agenti non rispondono.

**Casi d&#39;uso**

Indirizzamento account

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

Routing personalizzato

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Esempio</th>
    <th>Risultato</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideale</td>
    <td>TESTO</td>
    <td>TESTO</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>TESTO</td>
    <td>TESTO</td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>TESTO</td>
    <td>TESTO</td>
  </tr>
</tbody></table>

Indirizzamento team

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Esempio</th>
    <th>Risultato</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideale</td>
    <td>TESTO</td>
    <td>TESTO</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>TESTO</td>
    <td>TESTO</td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>TESTO</td>
    <td>TESTO</td>
  </tr>
</tbody></table>

Routing Round robin

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Esempio</th>
    <th>Risultato</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideale</td>
    <td>TESTO</td>
    <td>TESTO</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>TESTO</td>
    <td>TESTO</td>
  </tr>
  <tr>
    <td>Nessun agente di fallback</td>
    <td>TESTO</td>
    <td>TESTO</td>
  </tr>
</tbody></table>

### Notifica Pulse {#pulse-notification}

Ogni volta che un visitatore richiede di connettersi con un agente, oggi forniamo in-app una notifica del browser all’agente, ma gli agenti spesso non dispongono di queste chat.

* Ora l’agente live riceve una notifica e-mail, Slack, Inapp, browser quando un nuovo visitatore è interessato alla chat

* Il contenuto per la notifica Pulse può essere lo stesso utilizzato oggi per la notifica in-app tramite browser

Il comportamento deve essere lo stesso dell&#39;agente corrente da accettare quando più agenti accettano.
