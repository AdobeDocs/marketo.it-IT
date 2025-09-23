---
unique-page-id: 4719304
description: Azioni Salesforce implicite - Documentazione Marketo - Documentazione del prodotto
title: Azioni Salesforce implicite
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 27%

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
