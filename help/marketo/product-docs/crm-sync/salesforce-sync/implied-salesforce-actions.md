---
unique-page-id: 4719304
description: Scopri quali passaggi del flusso di Salesforce attivano la sincronizzazione automatica da persona a SFDC o altre azioni. Scopri le regole per Aggiungi a campagna, Cambia proprietario, Crea attività e Converti persona.
title: Azioni Salesforce implicite
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 23%

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
   <td>Aggiungere a campagna SFDC</td>
   <td>Sincronizzare persona con SFDC</td>
  </tr>
  <tr>
   <td>Modificare lo stato nella campagna SFDC</td>
   <td>Sincronizza persona con SFDC<br>Aggiungi a SFDC Campaign</td>
  </tr>
  <tr>
   <td>Modificare proprietario</td>
   <td><p>Sincronizzare persona con SFDC</p></td>
  </tr>
  <tr>
   <td>Convertire persona</td>
   <td><p>Sincronizzare persona con SFDC</p></td>
  </tr>
  <tr>
   <td>Creare attività</td>
   <td>Sincronizzare persona con SFDC</td>
  </tr>
 </tbody>
</table>

È possibile filtrare i record SFDC in un elenco smart utilizzando il filtro **[!UICONTROL SFDC Type]** con l&#39;operatore impostato su &quot;[!UICONTROL is not empty]&quot;. Tutti i record SFDC hanno un valore in questo campo.

Ricorda che queste azioni automatiche si verificano solo se il lead non si trova attualmente in [Salesforce.com](https://salesforce.com){target="_blank"}
