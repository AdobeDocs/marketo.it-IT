---
unique-page-id: 15695924
description: Classificazione e ottimizzazione della profilatura dell’account - Documentazione di Marketo - Documentazione del prodotto
title: Classificazione e tuning profilo account
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# Classificazione e tuning profilo account {#account-profiling-ranking-and-tuning}

La profilazione account identifica il profilo cliente ideale (ICP), classifica le aziende nel database in base all&#39;ICP e aggiunge i dati dell&#39;indicatore ICP agli account promossi come Account denominati.

## Risultati modello {#model-results}

I risultati mostrano tutti i tuoi account noti suddivisi per livello. A è il grado più alto, D è il più basso.

![](assets/results.png)

Anche se facoltativo, è consigliabile selezionare la casella di controllo Promuovi automaticamente in quanto consente di risparmiare molto tempo. Tuttavia, se desideri esaminare ogni account e [aggiungili manualmente](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts), lascia semplicemente deselezionata la casella.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Classifica</strong></td> 
   <td> 
    <div>
      Classificazione dell’account in base al profilo cliente ideale. A è la misura migliore, D è la misura minore. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Propensione</strong></td> 
   <td> 
    <div>
      Aumento stimato del tasso di conversione rispetto a una selezione di conti non basata su ICP. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Account (%)</strong></td> 
   <td> 
    <div>
      Percentuale di conti in input modello con questa classificazione. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>% della base del modello</strong></td> 
   <td> 
    <div>
      Percentuale di conti in base a modello che hanno questa classificazione. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Regolazione modello {#model-tuning}

Nella scheda Modello (Model), fate clic sul pulsante Ottimizza modello (Tune Model).

![](assets/two.png)

Sono disponibili diverse schede tra cui scegliere, che consentono una personalizzazione approfondita.

![](assets/tuning-page.png)

**Categorie indicatori**

<table> 
 <tbody> 
  <tr> 
   <td><strong>Conformità</strong></td> 
   <td> 
    <div>
      Certificazioni, posizioni relative alla conformità/assunzione. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Operazioni</strong></td> 
   <td> 
    <div>
      Posizioni/assunzioni legate alle operazioni. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>ORE</strong></td> 
   <td> 
    <div>
      Software HR o Payroll, posizioni/assunzioni relative alle risorse umane.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Progettazione</strong></td> 
   <td> 
    <div>
      Tecnologie, quadri di riferimento, posizioni/assunzioni correlate all'ingegneria. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Vendite</strong></td> 
   <td> 
    <div>
      Soluzioni e software per la vendita, posizioni di vendita/noleggio. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Intento</strong></td> 
   <td> 
    <div>
      Indicatori di intento. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      Soluzioni hardware e software, tecnologie, posizioni/assunzioni relative all'IT.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Finanza</strong></td> 
   <td> 
    <div>
      Software finanziario, posizioni finanziarie/assunzioni. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Marketing</strong></td> 
   <td> 
    <div>
      Tecnologie e software di marketing, posizioni di marketing/noleggio. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Aziende</strong></td> 
   <td> 
    <div>
      Inserzioni o partnership commerciali con Forbes o Inc. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Esperienza cliente e relazioni</strong></td> 
   <td> 
    <div>
      Posizioni/assunzioni relative a relazioni con i clienti e successo del cliente.
    </div></td> 
  </tr> 
 </tbody> 
</table>

Passa il cursore del mouse sulle descrizioni per visualizzare una descrizione di ciascuna colonna.

![](assets/tool-tip.png)

Fai clic sul menu a discesa Aggiungi indicatore ICP per inserire indicatori aggiuntivi nel modello.

![](assets/add-icp.png)

La selezione della casella Esporta consente di visualizzare l&#39;indicatore ICP nella pagina Dettagli conto denominato e di utilizzare l&#39;indicatore ICP selezionato come vincoli in [filtri account denominati](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>Gli indicatori ICP sono inclusi come vincoli in **Membro di account denominato** Filtri e trigger.

Ponderazione indicatore è ciò che controlla il livello di importanza che ogni indicatore riceve nel modello.

![](assets/weightage.png)

Fate clic su Aggiorna modello (Refresh Model) per rendere effettive le modifiche.

![](assets/refresh-button.png)

Al termine della messa a punto del modello (dopo averlo aggiornato), tornare alla scheda Risultati modello e fare clic su **Salva e applica le classificazioni**.

![](assets/ranks.png)
