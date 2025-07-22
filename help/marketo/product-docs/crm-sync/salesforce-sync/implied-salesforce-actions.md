---
unique-page-id: 4719304
description: Azioni Salesforce implicite - Documentazione Marketo - Documentazione del prodotto
title: Azioni Salesforce implicite
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 0%

---

# Azioni Salesforce implicite {#implied-salesforce-actions}

Quando viene eseguito un passaggio di flusso specifico di [!DNL Salesforce], a volte vengono eseguiti automaticamente passaggi aggiuntivi. Ecco le regole, quindi sai:

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
   <td>Aggiungi a SFDC Campaign</td> 
   <td>Sincronizza persona con SFDC</td> 
  </tr> 
  <tr> 
   <td>Modifica stato in SFDC Campaign</td> 
   <td>Sincronizza persona con SFDC<br>Aggiungi a SFDC Campaign</td> 
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

È possibile filtrare i record SFDC in un elenco smart utilizzando il filtro **[!UICONTROL SFDC Type]** con l&#39;operatore impostato su &quot;[!UICONTROL is not empty]&quot;. Tutti i record SFDC hanno un valore in questo campo.

Ricorda che queste azioni automatiche si verificano solo se il lead non si trova attualmente in [Salesforce.com](https://salesforce.com){target="_blank"}
