---
description: Comportamento Chatbot - Documentazione Marketo - Documentazione del prodotto
title: Comportamento del chatbot
exl-id: e91e7981-6617-42fe-8120-a7311a99cdfb
source-git-commit: 1803d6355747f4b6300509a3d361bf235dd56f44
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Comportamento del chatbot {#chatbot-behavior}

Di seguito sono riportati diversi scenari possibili che delineano il comportamento atteso del Chatbot da parte del visitatore in ciascuno di essi.

<table>
  <tbody>
    <tr>
      <th>Abbreviazione</th>
      <th>Dettagli</th>
    </tr>
    <tr>
      <td>D1, D2, D3, ecc.</td>
      <td>Rappresenta più finestre di dialogo in cui D1 è la finestra di dialogo 1</td>
    </tr>
    <tr>
      <td>P1, P2, P3, ecc.</td>
      <td>Rappresenta le priorità del dialogo in cui P1 è la priorità più alta</td>
    </tr>
    <tr>
      <td>WP1, WP2, WP3, ecc.</td>
      <td>Rappresenta più pagine web in cui WP1 è la prima pagina web</td>
    </tr>
    <tr>
      <td>V1, V2, V3, ecc.</td>
      <td>Rappresenta più visitatori della pagina web in cui V1 è visitatore uno</td>
    </tr>
   </tbody>
</table>

## Scenari {#scenarios}

<table>
  <tr>
      <th>Scenario</th>
      <th>Comportamento previsto Chatbot</th>
      <th>Azione back-end</th>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>V1 visita WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1 </p>
      </td>
      <td>Il numero di trigger per D1 verrà aumentato di 1</td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>V1 visita WP1</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1</p>
        <p>Dopo l'aggiornamento, D1 verrà nuovamente risolto</p>
      </td>
      <td>
        <p>Il numero di trigger per D1 verrà aumentato di 1</p>
        <p>Dopo l'aggiornamento, nessuna modifica al trigger D1 o al conteggio del coinvolgimento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 ma non risponde</p>
      </td>
      <td>D1 verrà risolto in V1</td>
      <td>
        <p>Il numero di trigger per D1 verrà aumentato di 1</p>
        <p>Nessuna modifica al conteggio del coinvolgimento D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 e fornisce la prima risposta</p>
      </td>
      <td>D1 verrà risolto in V1</td>
      <td>
        <p>Il numero di trigger per D1 verrà aumentato di 1</p>
        <p>Il conteggio del coinvolgimento per D1 verrà incrementato di 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 e fornisce la prima risposta</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1</p>
        <p>Dopo l'aggiornamento, D1 continuerà</p>
      </td>
      <td>
        <p>Il conteggio del trigger e il conteggio del coinvolgimento per D1 verranno incrementati di 1</p>
        <p>Dopo l'aggiornamento, nessuna modifica ad alcun conteggio</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1, si impegna con il chatbot e completa D1</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1</p>
        <p>Dopo l'aggiornamento, per V1 non verrà risolta alcuna finestra di dialogo o finestra di dialogo successiva</p>
      </td>
      <td>
        <p>Il conteggio del trigger, il conteggio del coinvolgimento e il conteggio completato per D1 verranno incrementati di 1</p>
        <p>Dopo l’aggiornamento, non verrà risolta alcuna finestra di dialogo o finestra di dialogo successiva</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1, WP2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 ma non risponde </p>
        <p>V1 visita WP2</p>
      </td>
      <td>
        <p>Visita di pagina WP1, D1 sarà risolto a V1</p>
        <p>Visita di pagina WP2, D1 sarà risolto a V2</p>
      </td>
      <td>
        <p>Il numero di trigger per D1 verrà aumentato di 1</p>
        <p>In WP2, nessuna modifica al conteggio dei trigger D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1, WP2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 e innestato</p>
        <p>V1 visita WP2</p>
      </td>
      <td>
        <p>Visita di pagina WP1, D1 sarà risolto a V1</p>
        <p>Visita di pagina WP2, D1 sarà risolto a V1</p>
      </td>
      <td>
        <p>Il conteggio del trigger e il conteggio del coinvolgimento per D1 verranno incrementati di 1</p>
        <p>In WP2, nessuna modifica ad alcun conteggio</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>D2 destinato solo a WP2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 e fornisce la prima risposta</p>
        <p>V1 visita WP2</p>
      </td>
      <td>
        <p>D1 verrà risolto con WP1</p>
        <p>D1 continuerà a V1 su WP2</p>
      </td>
      <td>
        <p>Il conteggio del trigger e il conteggio del coinvolgimento per D1 verranno incrementati di 1</p>
        <p>Nessuna modifica al trigger D2 o al conteggio del coinvolgimento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>D2 destinato solo a WP2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 ma non risponde </p>
        <p>V1 visita WP2</p>
      </td>
      <td>D1 verrà risolto con WP1<br/>
      D2 verrà risolto con WP2</td>
      <td>
        <p>Il numero di trigger per D1 verrà aumentato di 1</p>
        <p>Il numero di trigger per D2 verrà aumentato di 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>D2 destinato solo a WP2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 e completa D1</p>
        <p>V1 visita WP2</p>
      </td>
      <td>D1 sarà risolto su WP1 e su post-completamento<br/>D2 verrà risolto con WP2</td>
      <td>
        <p>Il conteggio del trigger, il conteggio del coinvolgimento e il conteggio completato per D1 verranno incrementati di 1</p>
        <p>Il numero di trigger per D2 verrà aumentato di 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>D2 destinato solo a WP2</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 e completa D1</p>
        <p>V1 visita WP2</p>
        <p>I clic V1 su D2 forniscono la prima risposta </p>
      </td>
      <td>D1 sarà risolto su WP1 e su post-completamento<br/>D2 verrà risolto con WP2</td>
      <td>
        <p>Il conteggio del trigger, il conteggio del coinvolgimento e il conteggio completato per D1 verranno incrementati di 1</p>
        <p>Il trigger e il conteggio del coinvolgimento per D2 saranno aumentati di 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 ma non risponde</p>
        <p>D1 non pubblicato</p>
      </td>
      <td>D1 verrà risolto in V1</td>
      <td>
        <p>Il numero di trigger per D1 verrà aumentato di 1</p>
        <p>Nessuna modifica al conteggio del coinvolgimento D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 ma non risponde</p>
        <p>D1 non pubblicato</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto per la prima volta a V1</p>
        <p>Dopo l’aggiornamento, non verrà risolta alcuna finestra di dialogo</p>
      </td>
      <td>
        <p>Il numero di trigger per D1 verrà aumentato di 1</p>
        <p>Nessuna modifica al conteggio del coinvolgimento D1</p>
        <p>Dopo l'aggiornamento, nessuna modifica al trigger D1 o al conteggio del coinvolgimento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 attivato con D1 </p>
        <p>D1 non pubblicato</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto in V1</p>
        <p>Dopo l'aggiornamento, D1 continuerà</p>
      </td>
      <td>
        <p>Il numero di trigger per D1 verrà aumentato di 1</p>
        <p>Il conteggio del coinvolgimento D1 verrà incrementato di 1</p>
        <p>Dopo l'aggiornamento, come D1 continuerà senza ulteriori modifiche per attivare o contare il coinvolgimento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 ma non risponde</p>
        <p>D1 viene pubblicato con nuove modifiche</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto per la prima volta a V1</p>
        <p>Dopo l’aggiornamento, verrà risolta la finestra di dialogo con le nuove modifiche</p>
      </td>
      <td>
        <p>Il numero di trigger per D1 verrà aumentato di 1</p>
        <p>Dopo l'aggiornamento, come D1 con nuove modifiche ma senza ulteriori modifiche per attivare il conteggio</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato solo a WP1</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>I clic V1 su D1 forniscono la prima risposta</p>
        <p>D1 viene pubblicato con nuove modifiche</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto per la prima volta a V1</p>
        <p>Dopo l’aggiornamento, la finestra di dialogo con le modifiche precedenti continuerà</p>
      </td>
      <td>
        <p>Il numero di trigger per D1 verrà aumentato di 1</p>
        <p>Il conteggio del coinvolgimento per D1 verrà incrementato di 1 </p>
        <p>Dopo l'aggiornamento, come il vecchio D1 apparirà in modo che nessuna modifica per attivare il conteggio</p>
      </td>
    </tr>
    <tr>
     <td>
        <p>D1 destinato al WP1 con 1 priorità</p>
        <p>D2 destinato al WP1 con 2 priorità</p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 ma non risponde</p>
        <p>D1 non pubblicato</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto per la prima volta a V1</p>
        <p>Dopo l'aggiornamento, D2 verrà risolto in V1</p>
      </td>
      <td>
        <p>Il numero di trigger per D1 verrà aumentato di 1</p>
        <p>Dopo l'aggiornamento, il conteggio degli attivatori per D2 verrà aumentato di 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato al WP1 con 1 priorità</p>
        <p>D2 destinato al WP1 con 2 priorità </p>
        <p>V1 visita WP1 per la prima volta</p>
        <p>V1 clicca su D1 e completa D1</p>
        <p>V1 aggiorna WP1 e vedi D2<br/>V1 clicca su D2 e completa D2</p>
        <p>L'addetto al marketing ha apportato modifiche a D1 e ha ripubblicato</p>
        <p>V1 aggiorna WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto per la prima volta a V1</p>
        <p>Dopo l'aggiornamento, D2 verrà risolto in V1</p>
        <p>Dopo aver completato D1 e D2, indipendentemente da quali modifiche o ripubblicato D1, D2 non verrà mostrato nuovamente a V1</p>
      </td>
      <td>
        <p>Il conteggio del trigger, il conteggio del coinvolgimento e il conteggio completato per D1 verranno incrementati di 1</p>
        <p>Aggiorna dopo il completamento di D2, nessuna azione da intraprendere</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato a WP1 con trigger "Time on Site" di 30 secondi</p>
        <p>V1 visita WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto ma non verrà attivato su V1</p>
        <p>Dopo 30 secondi, D1 verrà mostrato/attivato a V1</p>
      </td>
      <td>Il conteggio degli attivatori per D1 verrà aumentato di 1 solo dopo 30+ secondi trascorsi sulla pagina web</td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato a WP1, WP2 con innesco "Time on page" di 30 secondi</p>
        <p>V1 visita WP1, WP2</p>
      </td>
      <td>
        <p>D1 verrà risolto ma non verrà attivato su V1</p>
        <p>Dopo 30 secondi, D1 verrà mostrato/attivato a V1</p>
      </td>
      <td>Il conteggio degli attivatori per D1 verrà aumentato di 1 solo dopo 30+ secondi trascorsi sulla pagina web</td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato a WP1 con trigger di "percentuale di scorrimento" pari a 50</p>
        <p>V1 visita WP1</p>
      </td>
      <td>
        <p>D1 verrà risolto ma non verrà attivato su V1</p>
        <p>Dopo lo scorrimento del 50%, D1 verrà mostrato/attivato a V1</p>
      </td>
      <td>Il numero di trigger per D1 verrà aumentato di 1 solo dopo lo scorrimento del 50%</td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato a WP1 con 1 priorità e attivazione evento "Time on page" di 30 secondi</p>
        <p>D2 destinato a WP1 con 2 priorità e la "percentuale di scorrimento della pagina" dell'evento di 50</p>
        <p>V1 visita WP1, dopo 10 secondi V1 visita WP2, V1 visita WP1</p>
      </td>
      <td>
        <p>Su WP1, D1 verrà risolto ma non verrà attivato su V1</p>
        <p>Su WP2, D2 verrà risolto ma non verrà attivato su V1</p>
        <p>Su WP1, D1 verrà risolto e dopo 20 secondi D1 verrà attivato su V1</p>
      </td>
      <td>Il conteggio degli attivatori per D1 verrà aumentato di 1 solo dopo 30 secondi</td>
    </tr>
    <tr>
      <td>
        <p>D1 destinato a WP1 con trigger "Time on Site" di 1 minuto</p>
        <p>V1 visita WP1 per 1 minuto e viene mostrato D1 ma non si attiva</p>
        <p>V1 chiude il WP1 e ritorna al WP1 2 giorni dopo</p>
      </td>
      <td>
        <p>D1 verrà mostrato automaticamente a V1 in quanto hanno già soddisfatto i criteri di attivazione durante la sessione precedente</p>
        <p>La stessa logica si applica a "Time on Page" (Tempo sulla pagina) e a "page Scroll Percentuali" (Percentuale di scorrimento della pagina)</p>
      </td>
      <td>
        <p>Il numero di trigger per D1 verrà aumentato di 1</p>
        <p>Dopo il ritorno, nessuna azione da intraprendere</p>
      </td>
    </tr>
  </tbody>
</table>
