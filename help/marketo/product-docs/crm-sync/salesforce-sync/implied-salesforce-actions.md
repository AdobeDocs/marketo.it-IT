---
unique-page-id: 4719304
description: Azioni Salesforce implicite - Documenti Marketo - Documentazione del prodotto
title: Azioni Salesforce implicite
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Azioni Salesforce implicite {#implied-salesforce-actions}

>[!NOTE]
>
>**FYI**
>
>Marketo sta ora standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che l&#39;iscrizione contenga lead/lead e la persona/persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

Quando viene eseguito un passaggio di flusso specifico di Salesforce, talvolta vengono eseguiti automaticamente passaggi aggiuntivi. Ecco le regole, quindi sapete:

Queste regole si applicano *quando la persona non è attualmente in [Salesforce.com](http://Salesforce.com)* come contatto o lead.

<table> 
 <thead> 
  <tr> 
   <th>Passaggio del flusso di Marketo</th> 
   <th>Azione automatica</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aggiungi a campagna SFDC</td> 
   <td>Sincronizza persona con SFDC</td> 
  </tr> 
  <tr> 
   <td>Modifica dello stato nella campagna SFDC</td> 
   <td>Sincronizza persona con<br>SFDCA per la campagna SFDC</td> 
  </tr> 
  <tr> 
   <td>Cambia proprietario</td> 
   <td><p>Sincronizza persona con SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Converti persona</td> 
   <td><p>Sincronizza persona con SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Crea attività</td> 
   <td>Sincronizza persona con SFDC</td> 
  </tr> 
 </tbody> 
</table>

È possibile filtrare i record SFDC in uno Smart List utilizzando il filtro Tipo **** SFDC con l&#39;operatore impostato su &quot;non è vuoto&quot;. Tutti i record della DSC hanno un valore in questo campo.

Ricordate, queste azioni automatiche si verificano solo se il lead non si trova attualmente in [Salesforce.com](http://Salesforce.com)

La sincronizzazione Salesforce è fantastica, giusto?
