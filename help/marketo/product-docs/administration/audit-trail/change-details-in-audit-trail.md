---
unique-page-id: 11379928
description: Modifica dei dettagli nella traccia di controllo - Documenti Marketo - Documentazione del prodotto
title: Modifica dettagli nella traccia di audit
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '1901'
ht-degree: 0%

---


# Modifica dettagli nella traccia di audit {#change-details-in-audit-trail}

Audit Trail offre una grande quantità di informazioni su chi sta facendo cosa nell&#39;abbonamento a Marketo. Ecco i dettagli.

## Percorso controllo risorse {#asset-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">Risorsa/Tipo</th> 
   <th colspan="1">Azione</th> 
   <th colspan="1">Dettagli modifica</th> 
  </tr> 
  <tr> 
   <td rowspan="15">Programma predefinito<br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>Crea</td> 
   <td>Tipo di canale "tipo di canale"<br><br>o "Clonato da "nome del programma"</td> 
  </tr> 
  <tr> 
   <td>Rinomina</td> 
   <td>Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato sull'area di lavoro "nome area di lavoro" <br>Posizione "cartella campagna" o "programma di coinvolgimento" Nome <br>del programma "nuovo nome"</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Modifica canale</td> 
   <td>Nuovo canale "nuovo nome canale" Vecchio canale "vecchio nome canale" </td> 
  </tr> 
  <tr> 
   <td>Modifica token programma</td> 
   <td>Aggiungi il valore "token name" del token "token value"</td> 
  </tr> 
  <tr> 
   <td>Modifica token programma</td> 
   <td>Modifica token "nome token" nuovo valore "nuovo valore" vecchio valore "vecchio valore"</td> 
  </tr> 
  <tr> 
   <td>Modifica token programma</td> 
   <td>Elimina token "nome token"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td>Aggiunta del comportamento di analisi "nome comportamento"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td><p>Modifica il comportamento di analisi "nome comportamento"</p><p>Vecchio comportamento "nome comportamento"</p></td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td>Elimina il comportamento di analisi "nome comportamento"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Valore costo periodo aggiunto "#" mese programma "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Costo del periodo di modifica Nuovo valore di costo "#", Nuovo mese programma "yyyy-mm", Vecchio valore di costo "#", Vecchio mese programma "yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Elimina il costo del periodo. Valore "#" mese programma "yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td>Esporta</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td rowspan="18">E-mail<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br></td> 
   <td>Crea</td> 
   <td>Creato utilizzando il modello "nome modello" <br>o <br>clonato da "nome risorsa"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Aggiornato "Da nome" a "nuovo da nome"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Aggiornato "Da E-mail" a "<a href="http://docs.marketo.com/cdn-cgi/l/email-protection">[email protected]</a>"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>"Rispondi a" aggiornato a "<a href="http://docs.marketo.com/cdn-cgi/l/email-protection">[protetto tramite e-mail]</a>"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Aggiornato "Oggetto" a "nuova riga oggetto"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Aggiunta segmentazione "segmentation_name"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Segmentazione rimossa</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Aggiunto snippet "snippet_name"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Snippet rimosso</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Modifiche e-mail interrotte dal modello "template_name" (NOTA: questo accade oggi se si modifica il codice direttamente)</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Rinomina</td> 
   <td>Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Nuova descrizione "nuova descrizione" Vecchia descrizione "vecchia descrizione"</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato su "Design studio" nella cartella "nome cartella" Nome risorsa <br>clonata "nome"<br><br>o "Attività di marketing" in "nome programma" Nome risorsa<br>clonata "nome"</td> 
  </tr> 
  <tr> 
   <td>Sposta</td> 
   <td>Spostato in "Design studio" nella cartella "nome cartella"<br><br>o spostato in "Attività di marketing" in "nome programma"</td> 
  </tr> 
  <tr> 
   <td>Approva</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Non approvare</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Bozza</td> 
   <td>L'e-mail è stata redatta perché lo snippet "snippet name" è stato<br><br>approvato o l'e-mail è stata compilata perché il modello "template name" è stato approvato</td> 
  </tr> 
  <tr> 
   <td rowspan="17">Programma e-mail</td> 
   <td>Crea</td> 
   <td>Tipo di canale "tipo di canale"<br><br>o "Clonato da "nome del programma"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Rinomina</td> 
   <td colspan="1">Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato sull'area di lavoro "nome dell'area di lavoro" <br>Posizione "Cartella campagna o programma di coinvolgimento" Nome del programma <br>clonato "nuovo nome"</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Interrompi</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Modifica canale</td> 
   <td>Nuovo canale "nuovo canale" Vecchio canale "vecchio canale"</td> 
  </tr> 
  <tr> 
   <td>Modifica token programma</td> 
   <td>Aggiungi il valore "token name" del token "token value"</td> 
  </tr> 
  <tr> 
   <td>Modifica token programma</td> 
   <td>Modifica token "nome token" Nuovo valore "nuovo valore" vecchio valore "vecchio valore"</td> 
  </tr> 
  <tr> 
   <td>Modifica token programma</td> 
   <td>Elimina token "nome token"</td> 
  </tr> 
  <tr> 
   <td>Modifica programma</td> 
   <td>Imposta l'inizio della pianificazione su "data di inizio, ora di inizio" e la fine su "data di fine, ora di fine"</td> 
  </tr> 
  <tr> 
   <td>Modifica programma</td> 
   <td>La pianificazione è stata modificata in "nuova data, nuova ora"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td>Aggiunta del comportamento di analisi "nome comportamento"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td>Modifica il comportamento di analisi "nome comportamento"<br>Vecchio comportamento "nome comportamento"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td>Elimina il comportamento di analisi "nome comportamento"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Valore costo periodo aggiunto "#" mese programma "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Costo del periodo di modifica Nuovo valore di costo "#", Nuovo mese programma "yyyy-mm", Vecchio valore di costo "#", Vecchio mese programma "yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Elimina il costo del periodo. Valore "#" mese programma "yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Modello e-mail</td> 
   <td>Crea</td> 
   <td>Vuoto o Clona da "nome modello"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Nuova descrizione "nuova descrizione", descrizione precedente "descrizione precedente"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>HTML Modificato</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Rinomina</td> 
   <td>Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato su "nome cartella" Nome risorsa <br> clonata "nome"</td> 
  </tr> 
  <tr> 
   <td>Approva</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Non approvare</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td rowspan="23">Programma di coinvolgimento</td> 
   <td>Crea</td> 
   <td>Tipo di canale "tipo di canale"<br> o<br> Clona da "nome del programma"</td> 
  </tr> 
  <tr> 
   <td>Rinomina</td> 
   <td>Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato sull'area di lavoro "nome dell'area di lavoro" <br>Posizione "Cartella campagna o programma di coinvolgimento" Nome del programma <br>clonato "nuovo nome"</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Modifica canale</td> 
   <td>Nuovo canale "nuovo canale" Vecchio canale "vecchio canale"</td> 
  </tr> 
  <tr> 
   <td>Modifica flusso di programmi</td> 
   <td><p>Aggiungi flusso</p><p>Nome "name" Posizionamento "#"</p></td> 
  </tr> 
  <tr> 
   <td>Modifica flusso di programmi</td> 
   <td><p>Modifica flusso</p><p>Nuovo nome flusso: "new name" Nome del flusso precedente: "old name"</p><p>Nuovo posizionamento: "nuovo #" Posizione precedente: "old #"</p></td> 
  </tr> 
  <tr> 
   <td>Modifica flusso di programmi</td> 
   <td>Elimina nome flusso "name"</td> 
  </tr> 
  <tr> 
   <td>Modifica flusso di programmi</td> 
   <td>Aggiungi<br>contentSteam name "stream name"<br>Tipo "Email" o "Program"<br>Nome "email name" o "program name"<br>Smart Campaign "smart campaign name"</td> 
  </tr> 
  <tr> 
   <td>Modifica flusso di programmi</td> 
   <td>Attivare il nome<br>contentStream "stream name" Nome<br>contenuto "email name" o "program name"</td> 
  </tr> 
  <tr> 
   <td>Modifica flusso di programmi</td> 
   <td>Disattiva il nome<br>contentStream "nome flusso" Nome<br>contenuto "nome e-mail" o "nome programma"</td> 
  </tr> 
  <tr> 
   <td>Modifica flusso di programmi</td> 
   <td>Rimuovi nome<br>contentStream "nome flusso" Nome<br>contenuto "nome e-mail" o "nome programma"</td> 
  </tr> 
  <tr> 
   <td>Modifica token programma</td> 
   <td>Aggiungi il valore "token name" del token "token value"</td> 
  </tr> 
  <tr> 
   <td>Modifica token programma</td> 
   <td>Modifica token "nome token" Nuovo valore "nuovo valore" vecchio valore "vecchio valore"</td> 
  </tr> 
  <tr> 
   <td>Modifica token programma</td> 
   <td>Elimina token "nome token"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td>Aggiunta del comportamento di analisi "nome comportamento"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td>Modifica il comportamento di analisi "nome comportamento"<br>Vecchio comportamento "nome comportamento"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td>Elimina il comportamento di analisi "nome comportamento"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td>Modificare lo stato del programma. Nuovo valore "on/off" Valore precedente "off/on"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Valore costo periodo aggiunto "#" mese programma "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Costo del periodo di modifica Nuovo valore di costo "#", Nuovo mese programma "yyyy-mm", Vecchio valore di costo "#", Vecchio mese programma "yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Elimina il costo del periodo. Valore "#" mese programma "yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td>Esporta</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td rowspan="18">Programma evento</td> 
   <td>Crea</td> 
   <td>Tipo di canale "tipo di canale"<br><br>o "Clonato da "nome del programma"</td> 
  </tr> 
  <tr> 
   <td>Rinomina</td> 
   <td>Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato sull'area di lavoro "nome area di lavoro" <br>Posizione "cartella campagna" o "programma di coinvolgimento" Nome <br>del programma "nuovo nome"</td> 
  </tr> 
  <tr> 
   <td>Modifica canale</td> 
   <td>Nuovo canale "nuovo canale" Vecchio canale "vecchio canale" </td> 
  </tr> 
  <tr> 
   <td>Modifica token programma</td> 
   <td>Aggiungi il valore "token name" del token "token value"</td> 
  </tr> 
  <tr> 
   <td>Modifica token programma</td> 
   <td>Modifica token "nome token" Nuovo valore "nuovo valore" vecchio valore "vecchio valore"</td> 
  </tr> 
  <tr> 
   <td>Modifica token programma</td> 
   <td>Elimina token "nome token"</td> 
  </tr> 
  <tr> 
   <td>Modifica programma</td> 
   <td>Imposta l'inizio della pianificazione su "data di inizio, ora di inizio" e la fine su "data di fine, ora di fine"</td> 
  </tr> 
  <tr> 
   <td>Modifica programma</td> 
   <td>La pianificazione è stata modificata in "nuova data, nuova ora"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td>Aggiunta del comportamento di analisi "nome comportamento"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td>Modifica il comportamento di analisi "nome comportamento"<br>Vecchio comportamento "nome comportamento"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione programma</td> 
   <td>Elimina comportamento analisi "nome comportamento"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Valore costo periodo aggiunto "#" mese programma "aaaa-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Costo del periodo di modifica Nuovo valore di costo "#", Nuovo mese programma "yyyy-mm", Vecchio valore di costo "#", Vecchio mese programma "yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Elimina il costo del periodo. Valore "#" mese programma "yyyy-mm"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica impostazione programma</td> 
   <td colspan="1">Aggiunto partner evento ‘partner_name’</td> 
  </tr> 
  <tr> 
   <td>Esporta</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td rowspan="5">Cartelle</td> 
   <td>Crea</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>È stato aggiunto il token "token_name", valore "value"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Token modificato "token_name" nuovo valore "token_value" valore precedente "old_token_value"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Token "token_name" eliminato</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Forms</td> 
   <td>Crea</td> 
   <td>Presto. Per saperne di più o per clic da "nome modulo"</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Rinomina</td> 
   <td>Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Nuova descrizione "nuova descrizione" Vecchia descrizione "vecchia descrizione"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Impostazioni del modulo modificate </td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Dettagli campo modificati</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato su "Design studio" nella cartella "nome cartella" Nome risorsa <br>clonata "nome"<br><br>o "Attività di marketing" in "nome programma" Nome risorsa<br>clonata "nome"</td> 
  </tr> 
  <tr> 
   <td>Sposta</td> 
   <td>Spostato in "Design studio" nella cartella "nome cartella"<br><br>o spostato in "Attività di marketing" in "nome programma"</td> 
  </tr> 
  <tr> 
   <td>Forms</td> 
   <td>Approva</td> 
   <td>Usato da # assets </td> 
  </tr> 
  <tr> 
   <td rowspan="9">Pagina di destinazione</td> 
   <td>Crea</td> 
   <td>Creato utilizzando il modello "nome modello" <br>o <br>clonato da "nome risorsa"</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Rinomina</td> 
   <td>Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Nuova descrizione "nuova descrizione" Precedente "descrizione precedente"</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato su "Design studio" nella cartella "nome cartella" Nome risorsa<br>clonata "nome" URL risorsa<br>clonata "www.url.com"<br><br>o "Attività di marketing" nel programma "nome programma" Nome risorsa <br>clonata "nome"URL risorsa<br>clonata "www.url.com"</td> 
  </tr> 
  <tr> 
   <td>Sposta</td> 
   <td>Spostato in "Design studio" nella cartella "nome cartella"<br> o<br> spostato in "Attività di marketing" in "nome programma"</td> 
  </tr> 
  <tr> 
   <td>Approva</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Bozza</td> 
   <td>La pagina di destinazione è stata creata perché il modello "nome modello" è stato approvato</td> 
  </tr> 
  <tr> 
   <td>Non approvare</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td rowspan="8">Modello pagina di destinazione</td> 
   <td>Crea</td> 
   <td><p>BlankorClonato da "nome risorsa"<br><br></p></td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Rinomina</td> 
   <td>Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Nuova descrizione "nuova descrizione" descrizione precedente "descrizione precedente"</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato su "nome cartella" Nome risorsa <br>clonata "nome"</td> 
  </tr> 
  <tr> 
   <td>Esporta</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Approva</td> 
   <td>Usato da # assets </td> 
  </tr> 
  <tr> 
   <td>Non approvare</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td rowspan="5">Elenco (statico)</td> 
   <td>Crea</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Esporta</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato su "Database Persona" nella cartella "nome cartella" Nome risorsa <br>clonato "nome"<br><br>o su "Attività marketing" in "nome programma" Nome risorsa<br>clonata "nome"</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Rinomina</td> 
   <td>Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td rowspan="12">Smart Campaign</td> 
   <td>Crea</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Activate</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Disattiva</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Interrompi</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Sposta</td> 
   <td>Spostato in "Programmi" nel programma "nome programma"<br><br>o spostato in "Cartelle" nella cartella "nome cartella"</td> 
  </tr> 
  <tr> 
   <td>Rinomina</td> 
   <td>Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Nuova descrizione "nuova descrizione" Precedente "descrizione precedente"</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato su "Programmi" nel programma "nome programma" Nome risorsa <br>clonata "nome"<br><br>o "Cartella" nella cartella "nome cartella" Nome risorsa<br>clonata "nome"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione elenco smart</td> 
   <td>Mostra lo stato corrente, inclusi nomi e valori di filtri e attivatori</td> 
  </tr> 
  <tr> 
   <td>Modifica pianificazione campagna</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Modifica azione passaggio flusso</td> 
   <td>Mostra lo stato corrente, inclusi i nomi e i valori di ogni passaggio di flusso</td> 
  </tr> 
  <tr> 
   <td rowspan="7">Smart List</td> 
   <td>Crea</td> 
   <td>Duplicato da "nome elenco avanzato"</td> 
  </tr> 
  <tr> 
   <td>Esporta</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Rinomina</td> 
   <td>Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Nuova descrizione "nuova descrizione" Precedente "descrizione precedente"</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato su "Database Persona" nella cartella "nome cartella" Nome risorsa <br>clonato "nome"<br><br>o su "Attività marketing" in "nome programma" Nome risorsa <br>clonata "nome"</td> 
  </tr> 
  <tr> 
   <td>Modifica impostazione elenco smart</td> 
   <td>Mostra lo stato corrente, inclusi nomi e valori di filtri e attivatori </td> 
  </tr> 
  <tr> 
   <td rowspan="11">Snippet</td> 
   <td>Crea</td> 
   <td><p><br><br>BlankorCloning from "snippet name"</p></td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Aggiunta segmentazione "segmentation_name"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Segmentazione rimossa</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Modificato</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Rinomina</td> 
   <td>Nuovo nome "nuovo nome", nome precedente "nome precedente"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Nuova descrizione "nuova descrizione" Precedente "descrizione precedente"</td> 
  </tr> 
  <tr> 
   <td>Clona</td> 
   <td>Clonato su "nome cartella" Nome frammento <br>clonato "nome"</td> 
  </tr> 
  <tr> 
   <td>Approva</td> 
   <td>Usato da # assets</td> 
  </tr> 
  <tr> 
   <td>Approva con No-Draft</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Non approvare</td> 
   <td><p>N/D</p></td> 
  </tr> 
 </tbody> 
</table>

## Barra di controllo amministratore {#admin-audit-trail}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Area amministratore</th> 
   <th>Azione</th> 
   <th>Dettagli modifica</th> 
  </tr> 
  <tr> 
   <td>Restrizioni IP</td> 
   <td>Modifica</td> 
   <td>Sono state modificate le restrizioni IP in base alle seguenti opzioni: Consentita/Bloccata "block", Indirizzo IP "#", Restrizioni IP disattivate ""</td> 
  </tr> 
  <tr> 
   <td rowspan="2">Partizione</td> 
   <td>Crea</td> 
   <td>Partizione creata con nome "nome partizione"</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>partizione "nome partizione" eliminata</td> 
  </tr> 
  <tr> 
   <td>Forza password</td> 
   <td>Modifica</td> 
   <td>La protezione della password è stata modificata in modello: Sicurezza standard, lunghezza minima: #, inferiore-superiore: #, numero: #, caso misto: # , Scadenza : #, timeout sessione: #</td> 
  </tr> 
  <tr> 
   <td rowspan="3">Ruolo<br><br></td> 
   <td>Crea</td> 
   <td>Ruolo creato con "nome ruolo" (NOTA: se avete bisogno di dettagli sulle autorizzazioni aggiunte, contattate il supporto) - <br>mostra un'istantanea delle autorizzazioni assegnate al ruolo</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>Ruolo "Nome ruolo" eliminato</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>Ruolo modificato da "nome precedente" a "nuovo nome" (NOTA: se avete bisogno di dettagli sulle autorizzazioni modificate, contattate il supporto) - <br>mostra un'istantanea delle autorizzazioni assegnate al ruolo<br></td> 
  </tr> 
  <tr> 
   <td>Report Smartlist</td> 
   <td>Modifica</td> 
   <td>SmarList modificato per l'accesso da scaricare: "true o false"</td> 
  </tr> 
  <tr> 
   <td rowspan="7">Utente<br><br><br><br></td> 
   <td>Crea (invito)</td> 
   <td>Utente invitato con: L'e-mail "indirizzo e-mail", il nome "nome e cognome", l'accesso scadrà "vuoto o con una data", l'utente API "vero o falso" - <br>mostra un'istantanea dei ruoli e delle aree di lavoro assegnati all'utente</td> 
  </tr> 
  <tr> 
   <td colspan="1">Elimina</td> 
   <td colspan="1">Nome utente eliminato</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>L'utente è stato rinominato da "nome vecchio" a "nuovo nome" con e-mail: "email", apiUser: L'accesso "true" o "false" scade: "vuoto o con una data"</td> 
  </tr> 
  <tr> 
   <td>Modifica</td> 
   <td>L’utente è stato modificato per e-mail: "email", apiUser: "true o false", l'accesso scade: "vuoto o con una data"</td> 
  </tr> 
  <tr> 
   <td colspan="1">Modifica</td> 
   <td colspan="1">Mostra lo stato corrente, compresi i ruoli e le aree di lavoro assegnati all'utente</td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>Licenza calendario rilasciata all'indirizzo e-mail: Nome "email dell'utente": "nome utente"</td> 
  </tr> 
  <tr> 
   <td>Reimposta</td> 
   <td>Ripristino password per nome "name" e e-mail "email"</td> 
  </tr> 
  <tr> 
   <td rowspan="2">Area di lavoro</td> 
   <td>Crea</td> 
   <td>Area di lavoro creata con il nome "nome area di lavoro"</td> 
  </tr> 
  <tr> 
   <td>Elimina</td> 
   <td>Area di lavoro "nome area di lavoro" eliminata</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>* [Filtro nella traccia di controllo](filtering-in-audit-trail.md)

>



