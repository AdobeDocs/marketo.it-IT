---
description: Comportamento Chatbot - Documentazione di Marketo - Documentazione del prodotto
title: Comportamento chatbot
feature: Dynamic Chat
exl-id: e91e7981-6617-42fe-8120-a7311a99cdfb
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Comportamento chatbot {#chatbot-behavior}

Di seguito sono riportati diversi possibili scenari che descrivono il comportamento previsto di Chatbot per il visitatore in ciascuno di essi.

<table>
  <tbody>
    <tr>
      <th>Abbreviazione</th>
      <th>Dettagli</th>
    </tr>
    <tr>
      <td>D1, D2, D3, ecc.</td>
      <td>Rappresenta più finestre di dialogo in cui D1 è una finestra di dialogo</td>
    </tr>
    <tr>
      <td>P1, P2, P3, ecc.</td>
      <td>Rappresenta le priorità del dialogo in cui P1 è la priorità più alta</td>
    </tr>
    <tr>
      <td>WP1, WP2, WP3, ecc.</td>
      <td>Rappresenta più pagine Web in cui WP1 è la prima pagina Web</td>
    </tr>
    <tr>
      <td>V1, V2, V3, ecc.</td>
      <td>Rappresenta più visitatori di pagine Web, dove V1 è il visitatore uno</td>
    </tr>
   </tbody>
</table>

## Scenari {#scenarios}

<table>
  <tr>
      <th>Scenario</th>
      <th>Comportamento Chatbot previsto</th>
      <th>Azione back-end</th>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>V1 visita WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1</p>
      </td>
      <td>Il conteggio dei trigger per D1 verrà aumentato di 1</td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>V1 visita WP1</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1</p>
        <p>Dopo l'aggiornamento, D1 verrà risolto di nuovo</p>
      </td>
      <td>
        <p>Il conteggio dei trigger per D1 verrà aumentato di 1</p>
        <p>Dopo l'aggiornamento, nessun cambiamento al trigger D1 o al conteggio del coinvolgimento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 ma non risponde</p>
      </td>
      <td>D1 verrà risolto in V1</td>
      <td>
        <p>Il conteggio dei trigger per D1 verrà aumentato di 1</p>
        <p>Nessuna modifica al conteggio coinvolgimento D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 e fornisce la prima risposta</p>
      </td>
      <td>D1 verrà risolto in V1</td>
      <td>
        <p>Il conteggio dei trigger per D1 verrà aumentato di 1</p>
        <p>Il numero di impegni per D1 verrà aumentato di 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 e fornisce la prima risposta</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1</p>
        <p>Dopo l'aggiornamento, D1 continuerà</p>
      </td>
      <td>
        <p>Il conteggio dei trigger e del coinvolgimento per D1 verrà aumentato di 1</p>
        <p>Dopo l'aggiornamento, nessun cambiamento in alcun conteggio</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1, si impegna con il chatbot e completa D1</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1</p>
        <p>Dopo l’aggiornamento, per la versione 1 non verrà risolta alcuna finestra di dialogo o finestra di dialogo successiva</p>
      </td>
      <td>
        <p>Il conteggio dei trigger, il conteggio dei coinvolgimento e il conteggio dei completamenti per D1 verranno aumentati di 1</p>
        <p>Dopo l’aggiornamento, non verrà risolta alcuna finestra di dialogo né quella successiva</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1, WP2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 ma non risponde</p>
        <p>Visite V1 WP2</p>
      </td>
      <td>
        <p>La visita della pagina WP1, D1 verrà risolta in V1</p>
        <p>La visita della pagina WP2, D1 verrà risolta in V2</p>
      </td>
      <td>
        <p>Il conteggio dei trigger per D1 verrà aumentato di 1</p>
        <p>In WP2, nessun cambiamento al conteggio del trigger D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1, WP2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 ed è attivato</p>
        <p>Visite V1 WP2</p>
      </td>
      <td>
        <p>La visita della pagina WP1, D1 verrà risolta in V1</p>
        <p>La visita della pagina WP2, D1 verrà risolta in V1</p>
      </td>
      <td>
        <p>Il conteggio dei trigger e del coinvolgimento per D1 verrà aumentato di 1</p>
        <p>In WP2, nessun cambiamento per qualsiasi conteggio</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>D2 previsto solo per WP2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 e fornisce la prima risposta</p>
        <p>Visite V1 WP2</p>
      </td>
      <td>
        <p>D1 verrà risolto nel WP1</p>
        <p>D1 continuerà a V1 su WP2</p>
      </td>
      <td>
        <p>Il conteggio dei trigger e del coinvolgimento per D1 verrà aumentato di 1</p>
        <p>Nessun cambiamento al trigger D2 o al conteggio del coinvolgimento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>D2 previsto solo per WP2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 ma non risponde</p>
        <p>Visite V1 WP2</p>
      </td>
      <td>D1 verrà risolto nel WP1<br/>
      D2 verrà risolto nel WP2</td>
      <td>
        <p>Il conteggio dei trigger per D1 verrà aumentato di 1</p>
        <p>Il conteggio dei trigger per D2 verrà aumentato di 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>D2 previsto solo per WP2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 e completa D1</p>
        <p>Visite V1 WP2</p>
      </td>
      <td>D1 verrà risolto nel WP1 e dopo il completamento<br/>D2 verrà risolto nel WP2</td>
      <td>
        <p>Il conteggio dei trigger, il conteggio dei coinvolgimento e il conteggio dei completamenti per D1 verranno aumentati di 1</p>
        <p>Il conteggio dei trigger per D2 verrà aumentato di 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>D2 previsto solo per WP2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 e completa D1</p>
        <p>Visite V1 WP2</p>
        <p>I clic V1 su D2 forniscono la prima risposta</p>
      </td>
      <td>D1 verrà risolto nel WP1 e dopo il completamento<br/>D2 verrà risolto nel WP2</td>
      <td>
        <p>Il conteggio dei trigger, il conteggio dei coinvolgimento e il conteggio dei completamenti per D1 verranno aumentati di 1</p>
        <p>Il conteggio di trigger e coinvolgimento per D2 verrà aumentato di 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 ma non risponde</p>
        <p>Pubblicazione D1 annullata</p>
      </td>
      <td>D1 verrà risolto in V1</td>
      <td>
        <p>Il conteggio dei trigger per D1 verrà aumentato di 1</p>
        <p>Nessuna modifica al conteggio coinvolgimento D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 ma non risponde</p>
        <p>Pubblicazione D1 annullata</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1 per la prima volta</p>
        <p>Dopo l’aggiornamento, non verrà risolta alcuna finestra di dialogo</p>
      </td>
      <td>
        <p>Il conteggio dei trigger per D1 verrà aumentato di 1</p>
        <p>Nessuna modifica al conteggio coinvolgimento D1</p>
        <p>Dopo l'aggiornamento, non viene apportata alcuna modifica al trigger D1 o al conteggio del coinvolgimento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 inserita con D1</p>
        <p>Pubblicazione D1 annullata</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1</p>
        <p>Dopo l'aggiornamento, D1 continuerà</p>
      </td>
      <td>
        <p>Il conteggio dei trigger per D1 verrà aumentato di 1</p>
        <p>Il conteggio del coinvolgimento D1 verrà aumentato di 1</p>
        <p>Dopo l’aggiornamento, come D1 continuerà senza ulteriori modifiche per l’attivazione o il conteggio dei engagement</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 ma non risponde</p>
        <p>D1 viene pubblicato con nuove modifiche</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1 per la prima volta</p>
        <p>Dopo l’aggiornamento, la finestra di dialogo con le nuove modifiche verrà risolta</p>
      </td>
      <td>
        <p>Il conteggio dei trigger per D1 verrà aumentato di 1</p>
        <p>Dopo l’aggiornamento, come D1 con nuove modifiche ma senza ulteriori modifiche per il conteggio dei trigger</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto solo per WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>I clic V1 su D1 forniscono la prima risposta</p>
        <p>D1 viene pubblicato con nuove modifiche</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1 per la prima volta</p>
        <p>Dopo l’aggiornamento, la finestra di dialogo con le modifiche precedenti continua</p>
      </td>
      <td>
        <p>Il conteggio dei trigger per D1 verrà aumentato di 1</p>
        <p>Il numero di impegni per D1 verrà aumentato di 1</p>
        <p>Dopo l'aggiornamento, poiché la vecchia D1 viene visualizzata senza che sia necessario modificare il conteggio dei trigger</p>
      </td>
    </tr>
    <tr>
     <td>
        <p>D1 previsto per WP1 con priorità 1</p>
        <p>D2 previsto per WP1 con priorità 2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 ma non risponde</p>
        <p>Pubblicazione D1 annullata</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1 per la prima volta</p>
        <p>Dopo l'aggiornamento, D2 verrà risolto in V1</p>
      </td>
      <td>
        <p>Il conteggio dei trigger per D1 verrà aumentato di 1</p>
        <p>Dopo l'aggiornamento, il conteggio dei trigger per D2 verrà aumentato di 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto per WP1 con priorità 1</p>
        <p>D2 previsto per WP1 con priorità 2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 fa clic su D1 e completa D1</p>
        <p>V1 aggiorna WP1 e consulta D2<br/>V1 fa clic su D2 e completa D2</p>
        <p>L’addetto al marketing ha apportato modifiche a D1 e ripubblicato</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1 per la prima volta</p>
        <p>Dopo l'aggiornamento, D2 verrà risolto in V1</p>
        <p>Dopo aver completato D1 e D2, indipendentemente dalle modifiche o dalla ripubblicazione di D1, D2 non verrà più visualizzato in V1</p>
      </td>
      <td>
        <p>Il conteggio dei trigger, il conteggio dei coinvolgimento e il conteggio dei completamenti per D1 verranno aumentati di 1</p>
        <p>Aggiorna dopo il completamento del D2, nessuna azione da intraprendere</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto per WP1 con trigger "Time on Site" (Tempo sul sito) di 30 secondi</p>
        <p>V1 visita WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto ma non verrà attivato nella versione V1</p>
        <p>Dopo 30 secondi, D1 verrà mostrato/attivato a V1</p>
      </td>
      <td>Il conteggio dei trigger per D1 verrà aumentato di 1 solo dopo 30+ secondi trascorsi sulla pagina web</td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto per WP1, WP2 con trigger "Time on page" di 30 secondi</p>
        <p>V1 visita WP1, WP2</p>
      </td>
      <td>
        <p>D1 verrà risolto ma non verrà attivato nella versione V1</p>
        <p>Dopo 30 secondi, D1 verrà mostrato/attivato a V1</p>
      </td>
      <td>Il conteggio dei trigger per D1 verrà aumentato di 1 solo dopo 30+ secondi trascorsi sulla pagina web</td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto per WP1 con trigger "percentuale di scorrimento" di 50</p>
        <p>V1 visita WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto ma non verrà attivato nella versione V1</p>
        <p>Dopo uno scorrimento del 50%, D1 verrà visualizzato/attivato nella versione V1</p>
      </td>
      <td>Il conteggio dei trigger per D1 verrà aumentato di 1 solo dopo lo scorrimento del 50%</td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto per WP1 con priorità 1 e attivazione evento "Tempo sulla pagina" di 30 secondi</p>
        <p>D2 previsto per WP1 con priorità 2 e "percentuale di scorrimento pagina" evento di 50</p>
        <p>V1 visita WP1, dopo 10 secondi V1 visita WP2, V1 visita WP1</p>
      </td>
      <td>
        <p>Nel WP1, D1 verrà risolto ma non attivato in V1</p>
        <p>In WP2, D2 verrà risolto ma non verrà attivato in V1</p>
        <p>Al WP1, D1 verrà risolto e dopo 20 secondi D1 verrà attivato a V1</p>
      </td>
      <td>Il conteggio del trigger per D1 verrà aumentato di 1 solo dopo 30 secondi</td>
    </tr>
    <tr>
      <td>
        <p>D1 previsto per WP1 con trigger "Time on Site" di 1 minuto</p>
        <p>V1 visita WP1 per 1 minuto e viene visualizzato D1 ma non coinvolge</p>
        <p>V1 chiude WP1 e torna a WP1 2 giorni dopo</p>
      </td>
      <td>
        <p>D1 verrà mostrato automaticamente alla V1 poiché ha già soddisfatto i criteri di attivazione durante la sessione precedente</p>
        <p>La stessa logica si applica a "Tempo sulla pagina" e "Percentuale di scorrimento delle pagine"</p>
      </td>
      <td>
        <p>Il conteggio dei trigger per D1 verrà aumentato di 1</p>
        <p>Dopo il ritorno, non deve essere intrapresa alcuna azione</p>
      </td>
    </tr>
  </tbody>
</table>
