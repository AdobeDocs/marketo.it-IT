---
unique-page-id: 4719304
description: Azioni Salesforce implicite - Documenti Marketo - Documentazione del prodotto
title: Azioni Salesforce implicite
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---

# Azioni Salesforce implicite {#implied-salesforce-actions}

Quando viene eseguito un passaggio di flusso specifico per Salesforce, a volte vengono eseguiti automaticamente passaggi aggiuntivi. Ecco le regole, quindi sai:

Queste regole verranno applicate quando la persona non si trova attualmente in [Salesforce.com](https://Salesforce.com){target="_blank"} come contatto o lead.

<table> 
 <thead> 
  <tr> 
   <th>Passaggio del flusso Marketo</th> 
   <th>Azione automatica</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aggiungi a campagna SFDC</td> 
   <td>Sincronizza persona con SFDC</td> 
  </tr> 
  <tr> 
   <td>Modifica stato in una campagna SFDC</td> 
   <td>Sincronizza persona con SFDC<br>Aggiungi a campagna SFDC</td> 
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

È possibile filtrare i record SFDC in un elenco avanzato utilizzando **[!UICONTROL Tipo SFDC]** Filtra con l’operatore impostato su &quot;non è vuoto&quot;. Tutti i record SFDC contengono un valore in questo campo.

Ricorda che queste azioni automatiche si verificano solo se il lead non è attualmente in [Salesforce.com](https://salesforce.com){target="_blank"}
