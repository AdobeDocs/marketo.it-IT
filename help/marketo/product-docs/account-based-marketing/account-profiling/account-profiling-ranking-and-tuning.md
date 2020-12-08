---
unique-page-id: 15695924
description: Ranking e Tuning del profilo dell'account - Marketo Docs - Documentazione del prodotto
title: Classificazione e ottimizzazione profilo account
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---


# Classificazione e ottimizzazione profilo account {#account-profiling-ranking-and-tuning}

Il profilo dell&#39;account identifica il profilo cliente ideale (ICP), classifica le società nel database in base all&#39;ICP e aggiunge i dati dell&#39;indicatore ICP agli account promossi come Account denominati.

## Risultati modello {#model-results}

I risultati mostrano tutti gli account noti suddivisi per grado. A è il grado più alto, D è il più basso.

![](assets/results.png)

Anche se opzionale, si consiglia di selezionare la casella di controllo Promuovi automaticamente, in quanto consente di risparmiare un sacco di tempo. Tuttavia, se desiderate esaminare ciascun account e [aggiungerlo manualmente](http://docs.marketo.com/display/DOCS/Discover+Accounts#DiscoverAccounts-DiscoverCRMAccounts), lasciate la casella deselezionata.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Classifica</strong></td> 
   <td> 
    <div>
      Classificazione account in base al profilo cliente ideale. A è la migliore, D è la meno adatta. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Propensità</strong></td> 
   <td> 
    <div>
      Incremento stimato del tasso di conversione rispetto a una selezione di conti non basata sull'ICP. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Account (%)</strong></td> 
   <td> 
    <div>
      Percentuale di conti in input modello con questo grado. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>% di base del modello</strong></td> 
   <td> 
    <div>
      Percentuale di conti in base al modello con questo grado. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Sintonizzazione modello {#model-tuning}

Nella scheda Modello, fare clic sul pulsante Regola modello.

![](assets/two.png)

Ci sono diverse schede tra cui scegliere, consentendo una personalizzazione approfondita.

![](assets/tuning-page.png)

Categorie indicatori

| **Conformità** | Certificazioni, posizioni/assunzioni relative alla conformità. |
|---|---|
| **Operazioni** | Posizioni/assunzioni relative alle operazioni. |
| **HR** | Software HR o Payroll, posizioni/assunzioni relative alle risorse umane. |
| **Progettazione** | Tecnologie, strutture, posizioni/assunzioni relative all&#39;ingegneria. |
| **Vendite** | Soluzioni e software per le vendite, posizioni/assunzioni relative alle vendite. |
| **Intento** | Indicatori di intento. |
| **IT** | Soluzioni hardware e software, tecnologie, posizioni/cablaggio IT. |
| **Finanza** | Software di finanziamento, posizioni finanziarie/assunzioni. |
| **Marketing** | Tecnologie e software di marketing, posizioni/assunzioni relative al marketing. |
| **Business** | Voci Forbes o Inc. o partnership aziendali. |
| **Esperienza cliente e relazioni** | Successo del cliente e posizioni/assunzioni nelle relazioni con i clienti. |

Passate il puntatore del mouse sulle descrizioni di ciascuna colonna.

![](assets/tool-tip.png)

Fate clic sul menu a discesa Aggiungi indicatore ICP per inserire altri indicatori nel modello.

![](assets/add-icp.png)

Selezionando la casella Esporta è possibile visualizzare l&#39;indicatore ICP nella pagina Dettagli conto denominato, nonché utilizzare l&#39;indicatore ICP selezionato come vincoli nei filtri [account](http://docs.marketo.com/display/DOCS/Account+Filters)denominati.

![](assets/export.png)

>[!NOTE]
>
>Gli indicatori ICP sono inclusi come vincoli in **Membro dei filtri e attivatori di conto** denominato.

Spessore indicatore è ciò che controlla il livello di importanza che ogni indicatore riceve nel modello.

![](assets/weightage.png)

Fate clic su Aggiorna modello per rendere effettive le modifiche.

![](assets/refresh-button.png)

Una volta sintonizzato il modello (dopo averlo aggiornato), tornare alla scheda Risultati modello e fare clic su **Salva e applica blocchi**.

![](assets/ranks.png)

